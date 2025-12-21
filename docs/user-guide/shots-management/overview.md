# Shots Management Overview

## Introduction

The Shots Management module is the heart of AIMMS. It's where you create, organize, and manage all the shots in your project. This module provides a comprehensive table view of all your shots with powerful search, filtering, and editing capabilities.

## Understanding the Shots Table

The shots table displays all shots in your project in a spreadsheet-like format. Each row represents a shot, and each column contains specific information about that shot.

### Column Descriptions

| Column | Description | Example |
|--------|-------------|---------|
| **Shot ID** | Unique identifier for the shot (auto-generated) | 1, 2, 3 |
| **Order** | The sequence number of the shot | 1, 2, 3, 10 |
| **Shot Name** | Descriptive name for the shot | INT_OFFICE_DAY_001 |
| **Section** | Group shots by scenes or acts | Act 1, Opening, Climax |
| **Description** | Brief description of the shot | "Hero enters office" |
| **Image Prompt** | AI prompt for generating base image | "A man sitting at a desk..." |
| **Color Scheme** | Color palette for the shot | "Warm tones" |
| **Time of Day** | When the shot takes place | "Day", "Night", "Dawn" |
| **Location** | Where the shot takes place | "Office", "Street", "Home" |
| **Country** | Country setting for the shot | "USA", "France", "Japan" |
| **Year** | Time period for the shot | "2024", "1980s", "Future" |
| **Video Prompt** | AI prompt for generating final video | "A man walks into an office..." |

### Table Features

- **Sorting**: Click any column header to sort by that column
- **Search**: Use the search box to find shots by any column
- **Selection**: Click rows to select them for batch operations
- **Context Menu**: Right-click any shot for quick actions

## Key Features

### Shot Creation and Management

**Adding New Shots**
- Create shots with all necessary metadata
- Add shots relative to existing shots for proper sequencing
- Import multiple shots via CSV for bulk operations

**Editing Shot Information**
- Modify any shot details including prompts and metadata
- Batch edit multiple shots simultaneously
- Real-time updates across all modules

**Shot Organization**
- Group shots by sections for better organization
- Sort and filter shots by any criteria
- Search across all shot information

### Search and Filtering

**Quick Search**
- Search across all columns simultaneously
- Real-time results as you type
- Keyboard navigation through results

**Column-Specific Search**
- Focus search on specific columns
- Combine multiple search criteria
- Save frequently used search combinations

**Section Filtering**
- View shots by section (Act 1, Act 2, etc.)
- Focus on specific parts of your project
- Toggle between all sections and filtered views

### Import and Export

**CSV Import**
- Import shot lists from spreadsheets
- Validate data before importing
- Handle large datasets efficiently

**CSV Export**
- Export all shot data for backup or sharing
- Timestamped export files
- Multiple export formats available

### Media Integration

**Image and Video Links**
- Direct links to associated media in other modules
- Quick navigation between shots and media
- Visual indicators for media availability

**Take Management**
- View and manage multiple takes per shot
- Star favorite takes for easy identification
- Replace takes while preserving shot information

## Workflow Integration

### Cross-Module Navigation

The shots module integrates seamlessly with other AIMMS modules:

**Image Storyboard**
- Navigate directly to image gallery for any shot
- View all image takes for selected shots
- Star favorite images that influence shot quality

**Video Storyboard**
- Jump to video gallery for shot-specific videos
- Manage video takes and workflow files
- Link video prompts back to shot information

**Assets Management**
- Associate relevant assets with specific shots
- View asset references in shot details
- Maintain organized asset-shot relationships

### Project Organization

**Section Management**
- Create logical groupings of shots
- Organize by acts, scenes, or locations
- Filter views by section for focused work

**Shot Sequencing**
- Maintain proper shot order through numbering
- Reorder shots as needed
- Automatic renumbering when shots are moved

**Metadata Management**
- Comprehensive shot information storage
- Customizable metadata fields
- Integration with AI generation workflows

## Best Practices

### Shot Naming Conventions

**Consistent Naming**
- Use descriptive but concise shot names
- Include location and key action
- Maintain consistent format across project

**Examples of Good Shot Names**
- `INT_OFFICE_DAY_001` (Interior Office Day Shot 1)
- `EXT_STREET_NIGHT_002` (Exterior Street Night Shot 2)
- `INT_CAR_DAY_003` (Interior Car Day Shot 3)

### Organization Strategies

**Section Usage**
- Group related shots by section
- Use sections for acts, locations, or themes
- Filter by section for focused work sessions

**Metadata Completeness**
- Fill in all relevant shot information
- Use prompts that are specific and actionable
- Include location and time details for context

### Workflow Efficiency

**Batch Operations**
- Use multi-selection for bulk edits
- Apply changes to multiple shots simultaneously
- Leverage search and filter for quick navigation

**Integration Benefits**
- Use cross-module navigation for efficiency
- Maintain consistent information across modules
- Leverage starred system for quality control

## Advanced Features

### Custom Workflows

**Shot Templates**
- Create templates for similar shot types
- Standardize metadata for consistency
- Speed up shot creation process

**Automation Features**
- Batch import from external sources
- Automated metadata population
- Integration with external tools

### Data Management

**Backup and Recovery**
- Regular CSV exports for backup
- Database backup integration
- Recovery options for data loss

**Data Validation**
- Built-in validation for data integrity
- Error checking for incomplete information
- Warning system for potential issues

The Shots Management module provides the foundation for your entire AIMMS workflow. Mastering this module ensures efficient organization and management of your storyboard project.