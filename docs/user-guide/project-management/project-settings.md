# Project Settings

## Overview

The Project Settings module allows you to configure and manage your project's metadata, preferences, and system settings. This module provides access to essential project information and enables you to customize AIMMS behavior for your specific workflow.

## Accessing Project Settings

### Methods to Open Project Settings

**Method 1: Menu Navigation**
- Click **Project** in the main menu
- Select **Project Settings** from the dropdown
- Or use the keyboard shortcut `Ctrl+6`

**Method 2: Direct Access**
- Navigate to the **Settings** tab in the main interface
- The project settings panel will be displayed

**Method 3: Context Menu**
- Right-click in any module
- Select **Project Settings** from the context menu

## Project Metadata Management

### Viewing Project Information

The Project Settings module displays comprehensive information about your current project:

**Project Details**
- **Project Path**: Location of your project files
- **Database Location**: Path to the shots.db file
- **Schema Version**: Database structure version
- **App Version**: AIMMS version used with this project

**Project Timeline**
- **Created**: When the project was first created
- **Shots**: Date range of shot creation
- **Takes**: Date range of media take creation
- **Assets**: Date range of asset additions

### Editing Project Metadata

#### Author Information
1. Click in the **Author** field to edit
2. Enter or update the project author name
3. Click **Save** to apply changes
4. This information appears in exports and reports

#### Project Description
1. Edit the **Description** field
2. Add a comprehensive project description
3. Include project goals, scope, and notes
4. Save changes to update project metadata

#### Project Information
1. Use the **Project Info** text area for detailed information
2. Add project notes, requirements, or documentation
3. Support for multi-line text and formatting
4. This field is ideal for project documentation

## Database Information

### Database Overview

The database information section shows key details about your project's data:

**Database Statistics**
- **Total Shots**: Number of shots in the project
- **Total Takes**: Number of media takes (images/videos)
- **Total Assets**: Number of project assets
- **Database Size**: Storage space used by the database

**Data Integrity**
- **Schema Version**: Ensures compatibility with AIMMS version
- **Last Modified**: When database was last updated
- **Backup Status**: Information about recent backups

### Database Health Monitoring

**Validation Status**
- Check database integrity
- Monitor for corruption or issues
- View validation history

**Performance Indicators**
- Database size trends
- Query performance metrics
- Optimization recommendations

## ComfyUI Integration Settings

### ComfyUI Configuration

ComfyUI integration settings are available for future workflow automation:

**Output Path Configuration**
- **ComfyUI Output Path**: Directory where ComfyUI saves generated files
- **Path Validation**: Ensures the path is accessible and valid
- **Default Paths**: Platform-appropriate default paths

**URL Configuration**
- **ComfyUI URL**: Address of your ComfyUI server
- **Connection Testing**: Verify ComfyUI server accessibility
- **Default URL**: Standard localhost URL (http://127.0.0.1:8188/)

### Future Integration Features

**Workflow Automation**
- Direct integration with ComfyUI workflows
- Automatic prompt generation and execution
- Seamless media file transfer

**Advanced Settings**
- Custom workflow templates
- Batch processing configurations
- Quality and format preferences

## Theme and Appearance Settings

### Theme Management

While theme selection is handled through the main application menu, project settings can influence appearance:

**Project-Specific Themes**
- Default theme for this project
- Custom color schemes
- Font size preferences

**Display Preferences**
- Thumbnail quality settings
- Gallery layout preferences
- Interface element visibility

### Accessibility Settings

**High Contrast Mode**
- Enhanced visibility options
- Color scheme adjustments
- Text size and spacing

**Keyboard Navigation**
- Enhanced keyboard shortcuts
- Navigation preferences
- Accessibility feature configuration

## Project Preferences

### Default Settings

Configure default behaviors for your project:

**Shot Creation Defaults**
- Default section for new shots
- Default take numbering
- Default metadata templates

**Media Processing Defaults**
- Default image quality settings
- Default video processing options
- File naming conventions

**Export Preferences**
- Default export formats
- Export quality settings
- File organization preferences

### Workflow Customization

**Custom Workflows**
- Define project-specific workflows
- Create custom processing chains
- Set up automated tasks

**Integration Preferences**
- External tool configurations
- File association settings
- Plugin preferences

## File System Organization

### Project Structure Overview

Understanding your project's file organization:

```
project_root/
├── data/
│   ├── shots.db              # Main database
│   ├── csv/                  # Exported CSV files
│   ├── backup/              # Database backups
│   └── saves/               # Media relationship backups
├── media/                   # Shot media files
│   ├── 1/                   # Shot 1 folder
│   ├── 2/                   # Shot 2 folder
│   └── ...                  # Additional shot folders
├── assets/                  # Project assets
├── logs/                    # Project and application logs
└── project_config.json      # Project-specific configuration
```

### File Management Settings

**Backup Configuration**
- Automatic backup frequency
- Backup file retention
- Backup location settings

**File Organization**
- Media file naming conventions
- Folder structure preferences
- File cleanup settings

## Advanced Configuration

### Database Optimization

**Performance Settings**
- Database cache size
- Query optimization preferences
- Index management

**Maintenance Schedules**
- Automatic cleanup tasks
- Database optimization timing
- Backup verification

### Security and Permissions

**Access Control**
- Project locking settings
- Multi-user access configuration
- Permission management

**Data Protection**
- Encryption settings (if available)
- Backup security
- Access logging

## Troubleshooting Project Settings

### Common Issues

**Settings Not Saving**
- Check file permissions
- Verify project isn't locked
- Ensure sufficient disk space
- Try restarting AIMMS

**Invalid Configuration**
- Validate file paths
- Check URL formats
- Verify database connections
- Review permission settings

**Performance Problems**
- Reduce database cache size
- Optimize backup frequency
- Clean up old log files
- Check disk space

### Recovery Options

**Reset to Defaults**
- Restore default project settings
- Clear custom configurations
- Revert to factory settings

**Configuration Backup**
- Export current settings
- Create settings snapshots
- Document custom configurations

## Best Practices

### Project Organization

**Consistent Naming**
- Use consistent project naming
- Standardize file naming conventions
- Maintain organized folder structure

**Regular Maintenance**
- Review and update project metadata
- Clean up old backup files
- Monitor database performance
- Update configuration as needed

**Documentation**
- Document custom settings
- Record workflow preferences
- Maintain project notes
- Track configuration changes

### Security Considerations

**File Permissions**
- Set appropriate file permissions
- Protect sensitive project data
- Secure backup files
- Monitor access logs

**Data Integrity**
- Regular backup verification
- Database integrity checks
- File system monitoring
- Corruption prevention

## Integration with Other Modules

### Settings Synchronization

Project settings affect all modules:

**Shots Module**
- Default shot creation settings
- Metadata templates
- Workflow preferences

**Media Modules**
- Default quality settings
- File processing options
- Organization preferences

**Asset Management**
- Default asset categories
- Organization schemes
- Integration settings

### Cross-Module Consistency

**Theme Consistency**
- Uniform appearance across modules
- Consistent color schemes
- Standardized interface elements

**Workflow Integration**
- Seamless module transitions
- Consistent file handling
- Unified metadata management

## Advanced Features

### Custom Configuration

**Project Templates**
- Create project-specific templates
- Standardize project setup
- Share configurations across projects

**Automation Settings**
- Configure automated tasks
- Set up workflow triggers
- Customize processing chains

### Monitoring and Analytics

**Usage Statistics**
- Track project usage patterns
- Monitor module usage
- Analyze workflow efficiency

**Performance Metrics**
- Database performance monitoring
- File system performance
- Application responsiveness

Project settings are essential for customizing AIMMS to your specific workflow and ensuring optimal performance for your storyboard management needs.