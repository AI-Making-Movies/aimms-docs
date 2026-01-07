# Troubleshooting Guide

## Common Issues and Solutions

This guide covers common problems you might encounter while using AIMMS and provides step-by-step solutions.

### Installation and Launch Issues

#### Application Won't Start

**Problem**: AIMMS fails to launch or crashes immediately

**Solutions**:

1. **Check System Requirements**: Ensure your system meets minimum requirements
2. **Extract All Files**: Verify all files were extracted from the archive
3. **Run as Administrator**: Right-click and select "Run as administrator" (Windows)
4. **Antivirus**: Check if antivirus software is blocking the application
5. **Graphics Drivers**: Update your graphics drivers to the latest version

#### License Activation Problems

**Problem**: License key not accepted or validation fails

**Solutions**:

*Licensing is done offline and does not require an internet connection*

1. **Verify License Key**: Double-check the license key for typos and confirm your email address was the one used at purchase.
2. **Too Many Installations**: There is a timed limit restricting maximum installations to prevent pirating. If you experience this problem contact your seller. Old, unused installations i.e. old computers you migrated away from, will expire their limit when not used for a reasonable amount of time.
3. **Pirated copies**: Certain features are implemented to dissuade piracy and if you have bought or downloaded from an untrusted source then this might have triggered the issue.
4. **Copying the folder to a new machine**: You will need to install the application from the download on a new machine and re-apply the license key that way. Don't copy the entire folder to a new machine. This is implemented to discourage piracy, but there should not be a problem for a legitimate user installing on multiple machines within a fair limit.

If you experience problems, contact the point of sale.

#### Missing Dependencies

**Problem**: Error messages about missing libraries or dependencies

Windows comes bundled with all dependencies, but Linux and OSX will need ffmpeg and ffprobe installed seperately. In most cases you will likely already have them installed and working.

**Solutions**:

1. **Download Again**: Re-download from the official website
2. **Extract Properly**: Ensure all files are extracted correctly
3. **Platform Match**: Verify you downloaded the correct version for your OS
4. **System Updates**: Ensure your operating system is up to date

### Project and File Issues

#### Project Won't Open

**Problem**: Existing project fails to load or shows corruption errors

**Solutions**:

1. **Check File Permissions**: Ensure AIMMS has read/write access to project folder
2. **Disk Space**: Verify sufficient free space on your drive
3. **File Integrity**: Check if project files are corrupted
4. **Validation Logs**: Logs provide extensive information on validation fails. Check for "Error" messages specifically and resolve them. "Warning" messages will not fail at open, but "Error" messages will. 

> [completed to here]

#### Database Corruption

**Problem**: Database errors or inability to save changes

Multiple rescue solution methods are provided for as long as the user regularly uses the save, backup, and archive features in the File dropdown menu.

**Solutions**:

1. **Backup Restore**: Restore from the latest backup in `project_root/data/backup/`
2. **Validation**: Run File → Project Recovery → Validate Project
3. **Manual Recovery**: Use CSV export/import to recover data
4. **Support**: Contact support with error logs for assistance

#### Media Files Not Loading

**Problem**: Images or videos don't appear in the gallery

**Solutions**:

1. **File Format**: Ensure files are in supported formats (PNG, JPG, MP4, etc.)
2. **File Size**: Check files aren't too large (images < 100MB, videos < 500MB)
3. **File Paths**: Verify files haven't been moved or deleted
4. **Refresh**: Press `F5` to refresh the gallery view

### Performance Issues

#### Slow Application Response

**Problem**: AIMMS is slow to respond or lags during operation

**Solutions**:

1. **Close Other Apps**: Free up system memory and CPU
2. **Reduce Quality**: Lower thumbnail quality in Settings
3. **Clear Cache**: Clear thumbnail cache if corrupted
4. **Project Size**: Consider splitting very large projects

#### High Memory Usage

**Problem**: AIMMS uses excessive memory or causes system slowdown

**Solutions**:

1. **Memory Settings**: Adjust memory usage in Settings
2. **Close Projects**: Close projects you're not actively using
3. **System Resources**: Ensure adequate RAM and available memory
4. **Background Processes**: Close unnecessary background applications

#### Slow Media Loading

**Problem**: Images and videos take a long time to load

**Solutions**:

1. **File Optimization**: Use optimized file formats and sizes
2. **Storage Speed**: Use SSD storage for faster file access
3. **Network Issues**: If using network storage, check connection speed
4. **Cache Management**: Clear and rebuild thumbnail cache

### Import and Export Issues

#### CSV Import Fails

**Problem**: CSV file won't import or shows validation errors

**Solutions**:

1. **File Format**: Ensure CSV follows the required format
2. **Required Columns**: Verify all required columns are present
3. **Data Validation**: Check for empty shot names or invalid data
4. **File Encoding**: Use UTF-8 encoding for the CSV file

#### Export Problems

**Problem**: Export functions don't work or produce incomplete files

**Solutions**:

1. **Write Permissions**: Ensure write access to export directory
2. **Disk Space**: Check available disk space for export files
3. **File Locks**: Ensure files aren't locked by other applications
4. **Export Settings**: Verify export settings are configured correctly

### Display and Interface Issues

#### UI Elements Not Visible

**Problem**: Interface elements are missing or not displaying properly

**Solutions**:

1. **Screen Resolution**: Adjust screen resolution or scaling settings
2. **Theme Issues**: Try switching to a different theme
3. **Graphics Settings**: Update or adjust graphics driver settings
4. **Reset Layout**: Reset interface layout in Settings

#### Text Display Problems

**Problem**: Text appears garbled, too small, or unreadable

**Solutions**:

1. **Font Settings**: Adjust font size in Settings
2. **Display Scaling**: Check system display scaling settings
3. **Theme Compatibility**: Try a different theme
4. **System Fonts**: Ensure system fonts are properly installed

### Module-Specific Issues

#### Shots Module Problems

**Problem**: Shot management functions not working properly

**Solutions**:

1. **Database Lock**: Check for database locks from other processes
2. **Permissions**: Verify write permissions to project database
3. **Corruption**: Run database validation and repair if needed
4. **Memory**: Ensure sufficient memory for large shot lists

#### Media Module Issues

**Problem**: Image or video gallery not working correctly

**Solutions**:

1. **File Associations**: Check file type associations
2. **Codec Issues**: Install appropriate codecs for video playback
3. **Thumbnail Generation**: Allow time for thumbnail generation
4. **File Integrity**: Verify media files aren't corrupted

#### Asset Management Problems

**Problem**: Asset management functions not working

**Solutions**:

1. **File Paths**: Check asset file paths are accessible
2. **Permissions**: Verify read/write permissions for asset files
3. **File Types**: Ensure asset files are in supported formats
4. **Storage Space**: Check available storage for asset files

### Network and Integration Issues

#### ComfyUI Integration Problems

**Problem**: ComfyUI integration not working or connection fails

**Solutions**:

1. **Server Status**: Verify ComfyUI server is running
2. **URL Configuration**: Check ComfyUI URL settings in Project Settings
3. **Network Access**: Ensure network access to ComfyUI server
4. **Firewall**: Check firewall settings for blocked connections

#### Cloud Storage Issues

**Problem**: Cloud backup or sync not working

**Solutions**:

1. **Internet Connection**: Verify stable internet connection
2. **Account Status**: Check cloud storage account status
3. **Permissions**: Ensure AIMMS has necessary cloud storage permissions
4. **Storage Limits**: Check available cloud storage space

### Error Messages and Logs

#### Understanding Error Messages

When you encounter an error:

1. **Read Carefully**: Note the exact error message
2. **Take Screenshot**: Capture the error for reference
3. **Check Logs**: Review logs in the Logs module for details
4. **Document Steps**: Note what you were doing when the error occurred

#### Using Logs for Troubleshooting

1. **Access Logs**: Go to Logs module (Ctrl+7)
2. **Filter by Time**: Focus on recent log entries
3. **Search for Errors**: Look for ERROR or WARNING level messages
4. **Export Logs**: Export relevant logs for support analysis

### When to Contact Support

Contact AIMMS support when:
- Issues persist after trying troubleshooting steps
- You encounter critical errors that prevent using the application
- You need help with data recovery or migration
- You have questions about advanced features or workflows

### Before Contacting Support

Prepare this information:
1. **Error Details**: Exact error messages and when they occur
2. **System Information**: Operating system, AIMMS version, hardware specs
3. **Steps to Reproduce**: Detailed steps to recreate the issue
4. **Log Files**: Relevant log entries from the Logs module
5. **Screenshots**: Visual documentation of the problem

### Preventive Measures

To minimize issues:
1. **Regular Backups**: Export CSV files regularly
2. **Software Updates**: Keep AIMMS and system software updated
3. **System Maintenance**: Regular system cleanup and optimization
4. **Proper Shutdown**: Always close AIMMS properly before shutting down
5. **Documentation**: Keep notes on your workflow and configurations

Remember: Most issues can be resolved with the steps above. If you're still experiencing problems, don't hesitate to reach out to our support team with detailed information about your issue.