# Project Structure

## Overview

Understanding AIMMS project structure is essential for effective project management and organization. This guide explains the folder organization, file types, and data relationships within an AIMMS project.

## Project Directory Structure

When you create a new AIMMS project, it automatically generates this organized folder structure:

```
project_name/
├── data/                     # Database and data files
│   ├── shots.db             # Main SQLite database
│   ├── csv/                 # Exported CSV files
│   ├── backup/             # Database backups
│   └── saves/              # Media relationship backups
├── media/                   # Shot media files
│   ├── 1/                  # Shot 1 folder
│   ├── 2/                  # Shot 2 folder
│   ├── 3/                  # Shot 3 folder
│   └── ...                 # Additional shot folders
├── assets/                  # Project assets
│   ├── references/         # Reference images and materials
│   ├── audio/              # Audio files and sound effects
│   ├── documents/          # PDFs, scripts, and documentation
│   └── 3d_models/          # 3D models and textures
├── logs/                    # Project and application logs
│   ├── project_log.log     # Main project activity log
│   ├── system.log          # System and application logs
│   ├── error.log           # Error-specific logs
│   └── backup/             # Archived log files
└── project_config.json     # Project-specific configuration
```

## Core Components

### Data Directory (`data/`)

**shots.db**
- **Purpose**: Main SQLite database containing all project data
- **Contents**: Shots, takes, assets, metadata, and project settings
- **Importance**: Critical file - do not delete or modify manually
- **Backup**: Automatically backed up by AIMMS

**csv/** 
- **Purpose**: Exported data in CSV format for backup and sharing
- **Contents**: Separate CSV files for shots, takes, assets, and metadata
- **Naming**: Timestamped files (e.g., `shots_20251221_143045.csv`)
- **Usage**: Import/export, backup, analysis, and sharing

**backup/**
- **Purpose**: Automatic database backup files
- **Contents**: Compressed backup files with timestamps
- **Frequency**: Automatic backups during operations
- **Recovery**: Used for project recovery and restoration

**saves/**
- **Purpose**: Media relationship backup files
- **Contents**: JSON files mapping media files to database records
- **Function**: Ensures media files stay properly linked to shots
- **Recovery**: Used to restore media relationships if needed

### Media Directory (`media/`)

**Shot Organization**
- **Structure**: Each shot has its own numbered folder
- **Naming**: Folders use shot ID numbers (1, 2, 3, etc.)
- **Content**: Contains all media files for that specific shot
- **Types**: Images, videos, and workflow files

**Media File Types**
- **Images**: PNG, JPG, JPEG, WebP formats
- **Videos**: MP4, WebM, MKV, GIF formats
- **Workflow Files**: PNG files containing workflow data
- **Metadata**: Embedded in media files and database

**Take Management**
- **Naming Convention**: `base_01`, `base_02` for images; `video_01`, `video_02` for videos
- **UUID System**: Each take has a unique identifier
- **Relationship**: Takes linked to shots via database relationships
- **Starred System**: Favorite takes marked with star status

### Assets Directory (`assets/`)

**Reference Materials**
- **Images**: Mood boards, location photos, character designs
- **Organization**: Categorized by type and purpose
- **Metadata**: Detailed information about each asset
- **Integration**: Linked to shots and projects as needed

**Audio Files**
- **Types**: Sound effects, music, voiceovers, ambient sounds
- **Formats**: MP3, WAV, FLAC, OGG, AAC
- **Usage**: Reference, integration, or final production
- **Metadata**: Duration, format, and usage information

**Documents**
- **Types**: Scripts, storyboards, technical docs, PDFs
- **Organization**: By category and relevance
- **Integration**: Linked to shots or used as references
- **Searchability**: Full-text search capabilities

**3D Models and Technical**
- **Types**: OBJ, FBX, STL, GLTF files
- **Usage**: Reference, integration, or workflow
- **Metadata**: Technical specifications and usage notes
- **Compatibility**: Format-specific handling

### Logs Directory (`logs/`)

**Log Types**
- **Project Activity**: Shot creation, media operations, user actions
- **System Events**: Application startup, database operations, errors
- **Validation**: Project validation results and migration reports
- **Performance**: System performance and resource usage

**Log Management**
- **Rotation**: Automatic log rotation when files get too large
- **Archiving**: Old logs moved to backup folder
- **Search**: Filter and search capabilities
- **Export**: Export logs for analysis or support

## Database Structure

### Core Tables

**shots**
- **Purpose**: Main shot information and metadata
- **Key Fields**: shot_id (primary key), shot_name, order_number, section
- **Relationships**: Links to takes and assets
- **Features**: Modern architecture with shot_id-based system

**takes**
- **Purpose**: Media files associated with shots
- **Key Fields**: take_id (UUID), shot_id, file_path, take_type
- **Types**: Images (base), videos (video), masks (mask)
- **Features**: Flexible take management with UUID system

**assets**
- **Purpose**: Project assets and reference materials
- **Key Fields**: asset_id, asset_name, file_path, category
- **Types**: References, audio, documents, 3D models
- **Features**: Comprehensive asset management

**meta**
- **Purpose**: Project metadata and configuration
- **Key Fields**: key, value, data_type
- **Contents**: Project settings, preferences, configuration
- **Features**: Flexible key-value storage

**deleted_shots**
- **Purpose**: Deleted shot tracking for recovery
- **Key Fields**: shot_id, deletion_date, recovery_data
- **Function**: Enables shot recovery from deletion
- **Features**: Safe deletion with recovery capability

### Data Relationships

**Shot-to-Take Relationship**
- **One-to-Many**: One shot can have multiple takes
- **Types**: Image takes, video takes, mask takes
- **Management**: Easy take addition, replacement, deletion
- **Starred System**: Favorite take selection per shot

**Shot-to-Asset Relationship**
- **Many-to-Many**: Shots can reference multiple assets
- **Types**: Reference images, audio files, documents
- **Integration**: Seamless asset-shot linking
- **Organization**: Categorized asset management

**Project Hierarchy**
- **Project Level**: Overall project settings and metadata
- **Shot Level**: Individual shot information and organization
- **Take Level**: Specific media file management
- **Asset Level**: Supporting material organization

## File Management

### Automatic Organization

**Media File Handling**
- **Automatic Sorting**: Files automatically organized by shot
- **Take Numbering**: Sequential take numbering system
- **UUID Generation**: Unique identifiers for each take
- **Relationship Tracking**: Database maintains file relationships

**Backup System**
- **Automatic Backups**: Regular database and relationship backups
- **CSV Exports**: Regular data exports for additional backup
- **Recovery Options**: Multiple recovery mechanisms
- **Data Integrity**: Comprehensive validation and recovery

### File Naming Conventions

**Shot Folders**
- **Format**: Numeric folders (1, 2, 3, etc.)
- **Purpose**: Organize media by shot ID
- **Benefits**: Prevents naming conflicts, easy organization

**Take Files**
- **Images**: `base_01.png`, `base_02.jpg`, etc.
- **Videos**: `video_01.mp4`, `video_02.webm`, etc.
- **Masks**: `mask_01.png`, `mask_02.png`, etc.
- **Workflow**: `workflow_01.png` for video workflow data

**Backup Files**
- **Format**: Timestamped with project name
- **Types**: Database backups, relationship backups, CSV exports
- **Organization**: Automatic organization by date and type

## Best Practices

### Project Organization

**Consistent Structure**
- Maintain the standard AIMMS project structure
- Don't manually modify database files
- Use AIMMS tools for file management
- Regularly backup project data

**File Management**
- Use descriptive shot names
- Organize assets by category
- Maintain consistent naming conventions
- Regularly clean up unused files

**Data Integrity**
- Don't move files outside AIMMS
- Use AIMMS for all file operations
- Regular validation checks
- Maintain backup procedures

### Performance Optimization

**Storage Considerations**
- Use SSD storage for better performance
- Ensure adequate free disk space
- Organize projects by size and complexity
- Consider project splitting for very large projects

**File Management**
- Optimize media file sizes
- Use appropriate file formats
- Regular cleanup of unused files
- Efficient asset organization

## Troubleshooting

### Common Structure Issues

**Missing Files**
- Check file system permissions
- Verify project wasn't moved or corrupted
- Use backup recovery if needed
- Contact support for advanced recovery

**Database Problems**
- Don't manually edit database files
- Use AIMMS recovery tools
- Restore from backup if necessary
- Contact support for database issues

**Media Organization**
- Don't manually move media files
- Use AIMMS for file operations
- Check file permissions
- Verify project structure integrity

Understanding the AIMMS project structure helps you work more efficiently and maintain data integrity throughout your project lifecycle.