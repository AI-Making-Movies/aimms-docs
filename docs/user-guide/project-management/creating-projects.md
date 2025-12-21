# Creating Projects

## Overview

Creating a new project in AIMMS is the first step in organizing your storyboard. This guide will walk you through the process of setting up a new project with proper configuration.

## Step-by-Step Project Creation

### Method 1: Using the Menu

1. **Launch AIMMS**
   - Open the AIMMS application
   - Wait for the main interface to load

2. **Access New Project**
   - Click **File** in the main menu
   - Select **New Project** from the dropdown
   - Or use the keyboard shortcut `Ctrl+N`

3. **Configure Project Details**
   - **Project Name**: Enter a descriptive name for your project
   - **Project Location**: Choose where to save your project files
   - **Project Type**: Select project template (if available)

4. **Create Project**
   - Click **Create** to initialize the project
   - AIMMS will create the project structure automatically
   - The new project will open and be ready for use

### Method 2: Using the Project Browser

1. **Open Project Browser**
   - Click **File** → **Project Browser**
   - Or use the project browser shortcut if configured

2. **Create New Project**
   - Click the **New Project** button
   - Follow the same configuration steps as Method 1

## Project Structure

When you create a new project, AIMMS automatically generates this folder structure:

```
project_name/
├── data/
│   ├── shots.db              # Main database file
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

### Understanding the Structure

**Data Directory (`data/`)**
- **shots.db**: SQLite database containing all project data
- **csv/**: Directory for exported CSV files
- **backup/**: Automatic database backups
- **saves/**: Media relationship backup files

**Media Directory (`media/`)**
- Organized by shot ID (numeric folders)
- Each shot has its own folder for media files
- Automatic organization prevents file conflicts

**Assets Directory (`assets/`)**
- Stores project reference materials
- Organized by asset type and category
- Supports various file formats

**Logs Directory (`logs/`)**
- Application and project activity logs
- Error logs and system events
- Performance monitoring data

## Project Configuration Options

### Project Metadata

During creation, you can configure:

- **Project Name**: Descriptive project identifier
- **Author**: Your name or team name
- **Description**: Project purpose and scope
- **Created Date**: Automatically set to current date

### Advanced Settings

For advanced users:

- **Database Settings**: Custom database configuration
- **Media Settings**: Default media processing options
- **Backup Settings**: Backup frequency and retention
- **Integration Settings**: External tool configurations

## Best Practices for Project Creation

### Naming Conventions

- **Use Descriptive Names**: Choose names that clearly identify the project
- **Include Project Type**: Add project type if helpful (e.g., "Short Film", "Commercial")
- **Version Numbers**: Include version if applicable (e.g., "Project_v1.0")
- **Avoid Special Characters**: Stick to letters, numbers, and underscores

### Project Organization

- **Dedicated Folder**: Create projects in a dedicated workspace folder
- **Backup Strategy**: Plan your backup and version control strategy
- **Team Collaboration**: Consider team access and sharing requirements
- **Storage Planning**: Ensure adequate storage space for media files

### Project Templates

If available, use project templates for:

- **Standardized Setup**: Consistent project structure
- **Pre-configured Settings**: Optimized defaults for your workflow
- **Asset Libraries**: Pre-loaded reference materials
- **Workflow Integration**: Ready-to-use integration settings

## Post-Creation Setup

### Initial Configuration

After creating your project:

1. **Set Project Preferences**
   - Configure default settings in Project Settings
   - Set up theme and appearance preferences
   - Configure keyboard shortcuts if needed

2. **Import Existing Data**
   - Use CSV import if you have existing shot lists
   - Import reference assets and materials
   - Set up project templates if available

3. **Customize Workflow**
   - Configure integration with external tools
   - Set up backup and recovery procedures
   - Establish naming conventions and organization standards

### First Project Actions

Recommended first steps:

1. **Create Shot List**: Start building your storyboard
2. **Add Reference Materials**: Import assets and references
3. **Configure Settings**: Customize to your workflow
4. **Test Workflow**: Verify all integrations work correctly

## Troubleshooting Project Creation

### Common Issues

**Project Won't Create**
- Check write permissions to the selected location
- Ensure sufficient disk space is available
- Verify the project name doesn't contain invalid characters
- Try creating in a different location

**Project Structure Missing**
- Verify AIMMS has proper file system permissions
- Check if antivirus software is interfering
- Try running AIMMS as administrator
- Re-create the project if structure is incomplete

**Database Creation Failed**
- Check if another AIMMS instance is running
- Verify database file isn't locked by another process
- Ensure the location allows database file creation
- Check available disk space

### Recovery Options

If project creation fails:

1. **Check Logs**: Review error messages in the Logs module
2. **Manual Cleanup**: Remove any partial project files
3. **Retry Creation**: Attempt creation again with corrected settings
4. **Support Contact**: Contact support if issues persist

## Project Management Tips

### Organization Strategies

- **Consistent Naming**: Use consistent naming across all projects
- **Template Usage**: Create and use project templates for efficiency
- **Regular Backups**: Establish regular backup procedures
- **Documentation**: Document project-specific settings and workflows

### Performance Optimization

- **Storage Location**: Use fast storage (SSD) for better performance
- **Project Size**: Consider splitting very large projects
- **Media Management**: Organize media files efficiently
- **Regular Maintenance**: Perform regular project maintenance

### Collaboration Features

For team projects:

- **Shared Storage**: Use network storage for team access
- **Version Control**: Implement version control for project files
- **Access Control**: Set appropriate permissions for team members
- **Communication**: Establish clear communication about project changes

## Next Steps

After creating your project:

1. **Explore the Interface**: Familiarize yourself with the main modules
2. **Add Your First Shot**: Start building your storyboard
3. **Import Assets**: Add reference materials and assets
4. **Configure Workflow**: Set up your preferred workflow

Your new AIMMS project is now ready for professional storyboard management!