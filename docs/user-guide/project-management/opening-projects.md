# Opening Projects

## Overview

Opening an existing project in AIMMS allows you to continue working on your storyboard from where you left off. This guide covers different methods to open projects and troubleshoot common issues.

## Methods to Open Projects

### Method 1: Using the Menu

1. **Access Open Project**
   - Click **File** in the main menu
   - Select **Open Project** from the dropdown
   - Or use the keyboard shortcut `Ctrl+O`

2. **Browse for Project**
   - Navigate to your project folder location
   - Select the project folder (not individual files)
   - Click **Open** to load the project

### Method 2: Using Recent Projects

1. **Access Recent Projects**
   - Click **File** in the main menu
   - Select **Recent Projects** from the dropdown
   - Choose from the list of recently opened projects

2. **Project Selection**
   - Projects are listed by name and location
   - Recently used projects appear at the top
   - Click any project to open it immediately

### Method 3: Using Project Browser

1. **Open Project Browser**
   - Click **File** → **Project Browser**
   - The project browser shows all available projects

2. **Select and Open**
   - Browse your project registry
   - Click any project to open it
   - Use search to find specific projects

### Method 4: Direct Folder Access

1. **Locate Project Folder**
   - Navigate to your project folder in file explorer
   - Ensure the folder contains the complete project structure

2. **Open via AIMMS**
   - Launch AIMMS
   - Use File → Open Project to select the folder
   - AIMMS will validate and load the project

## Project Validation Process

When opening a project, AIMMS performs several validation checks:

### Database Validation
- **File Integrity**: Checks if `shots.db` is present and valid
- **Schema Compatibility**: Verifies database schema matches AIMMS version
- **Corruption Detection**: Identifies any database corruption issues

### File Structure Validation
- **Required Files**: Ensures all required project files are present
- **Folder Structure**: Validates the project directory structure
- **Permissions**: Checks file system permissions

### Project Integrity Checks
- **Media Files**: Verifies media file references are valid
- **Asset Files**: Checks asset file accessibility
- **Configuration**: Validates project configuration files

## Project Loading Process

### Loading Sequence

1. **Project Discovery**
   - AIMMS scans the project folder
   - Identifies project files and structure
   - Validates project integrity

2. **Database Loading**
   - Opens and reads the SQLite database
   - Loads shot, take, and asset data
   - Establishes database connections

3. **Media Indexing**
   - Scans media folders for files
   - Creates thumbnail cache if needed
   - Indexes media files for quick access

4. **Interface Initialization**
   - Loads project settings and preferences
   - Initializes module interfaces
   - Applies theme and appearance settings

### Loading Indicators

- **Progress Bar**: Shows loading progress
- **Status Messages**: Displays current loading stage
- **Estimated Time**: Shows expected completion time
- **Error Messages**: Alerts for any loading issues

## Troubleshooting Project Opening

### Common Issues

#### Project Won't Open
**Problem**: Project fails to load or shows error messages
**Solutions**:
1. **Check Project Structure**: Ensure all required files are present
2. **Verify Permissions**: Check file system read/write permissions
3. **Disk Space**: Ensure sufficient free space on the drive
4. **Database Issues**: Check for database corruption or locking

#### Slow Loading
**Problem**: Project takes a long time to load
**Solutions**:
1. **Project Size**: Large projects may take longer to load
2. **Storage Speed**: Use SSD storage for faster loading
3. **System Resources**: Close other applications to free memory
4. **Thumbnail Cache**: Allow time for thumbnail generation

#### Missing Media Files
**Problem**: Images or videos don't appear after loading
**Solutions**:
1. **File Paths**: Check if media files were moved or deleted
2. **Permissions**: Verify media file access permissions
3. **Refresh**: Press `F5` to refresh the media gallery
4. **Recovery**: Use media recovery tools if files are missing

#### Database Errors
**Problem**: Database-related error messages
**Solutions**:
1. **Backup Restore**: Restore from backup if available
2. **Validation**: Run project validation to check integrity
3. **Recovery**: Use File → Project Recovery tools
4. **Support**: Contact support with error details

### Advanced Troubleshooting

#### Project Corruption
**Symptoms**: Project won't open, data appears missing
**Recovery Steps**:
1. **Check Backups**: Look for backup files in `project_root/data/backup/`
2. **CSV Recovery**: Use CSV export files to recover data
3. **Manual Recovery**: Restore individual files from backups
4. **Support Assistance**: Contact support for advanced recovery

#### Permission Issues
**Symptoms**: Access denied errors, files can't be read/written
**Solutions**:
1. **File Permissions**: Check and adjust file system permissions
2. **Administrator Rights**: Run AIMMS as administrator
3. **Antivirus**: Check if antivirus is blocking file access
4. **Network Issues**: For network storage, check network permissions

#### Compatibility Issues
**Symptoms**: Project created in older version won't open
**Solutions**:
1. **Version Check**: Verify AIMMS version compatibility
2. **Migration**: Use migration tools if available
3. **Export/Import**: Export data and import to new project
4. **Support**: Contact support for version-specific issues

## Project Management Features

### Project Switching
- **Quick Switch**: Use File → Switch Project for fast switching
- **Recent Projects**: Access recently used projects from the menu
- **Project Browser**: Browse and manage multiple projects

### Project Information
- **Project Details**: View project metadata and statistics
- **File Locations**: Access project file paths and locations
- **Database Info**: View database status and information

### Project Maintenance
- **Validation**: Regularly validate project integrity
- **Backup**: Create regular backups of project data
- **Cleanup**: Remove unused files and optimize project size

## Best Practices

### Project Organization
- **Consistent Structure**: Maintain consistent project folder structure
- **Backup Strategy**: Implement regular backup procedures
- **Version Control**: Consider version control for project files
- **Documentation**: Document project-specific settings and workflows

### Performance Optimization
- **Storage Location**: Use fast storage (SSD) for better performance
- **Project Size**: Consider splitting very large projects
- **Media Management**: Organize media files efficiently
- **Regular Maintenance**: Perform regular project maintenance

### Security and Access
- **File Permissions**: Set appropriate file system permissions
- **Backup Security**: Secure backup files appropriately
- **Access Control**: Control access to project files
- **Data Protection**: Implement data protection measures

## Next Steps After Opening

Once your project is successfully opened:

1. **Verify Data**: Check that all shots, media, and assets are present
2. **Update Settings**: Review and update project settings if needed
3. **Continue Work**: Resume your storyboard management workflow
4. **Regular Maintenance**: Perform regular project maintenance tasks

Your project is now ready for continued storyboard management in AIMMS!