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

*Licensing does not require an internet connection. Purchasing version 1 license key entitles you to all future versions of 1.x*

1. **Verify License Key**: Double-check the license key for typos and confirm your email address was the one used at purchase.
2. **Too Many Installations**: There is a timed limit restricting maximum installations to dissuade pirating. If you experience this problem contact your seller. Old, unused installations i.e. old computers you migrated away from, will expire their limit when not used for a reasonable period of time.
3. **Pirated copies**: Certain features are implemented to dissuade piracy and if you have bought or downloaded from an untrusted source then this might have triggered the issue.
4. **Don't copy the folder to a new machine**: You will need to install the application from the original download on a new machine and re-apply the license key before use. Don't copy the entire folder to a new machine. This is implemented to discourage piracy, but there should not be a problem for a legitimate user installing on multiple machines within a fair limit.

If you experience problems, contact the point of sale.

#### Missing Dependencies

**Problem**: Error messages about missing libraries or dependencies

Windows comes bundled with all dependencies, but Linux and OSX will need `ffmpeg` and `ffprobe` installed seperately. In most cases you will likely already have them installed and working if you have used your device for viewing media files.

**Solutions**:

1. **Download Again**: Download latest version 1.x from the official website
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
5. **Corrupt config.json**: If the project still wont open try renaming the `config.json` in the application root folder *(NOTE: Do not delete any `config.json` files found under your project folders)*. The application root level `config.json` will be recreated at run-time allowing you to create a new project or open an existing one.

#### Database & File Corruption

**Problem**: Database errors or file corruption

Multiple rescue methods are provided for, as long as the user regularly uses the save, backup, export, and archive features found in the File dropdown menu.

Applying save and backup at the end of each session will ensure rollback is always possible. Manual tending to the backup folders to remove older backups will be required.

A complete snapshot backup of the entire project is provided by the File → Archive Project option. However, if your projects become large (e.g. 25 GB) then manual archiving of the project folder is a more suitable approach, done when the application is closed.

**Solutions**:

1. **Archive Restore**: Archive a complete project folder to a time-stamped `.zip` using the File → Archive Project feature. This enables a project snapshot to be stored anywhere you like. Restoring an archive will require manually unpacking the `.zip` and then opening the project folder from within AIMMS. 
2. **Database backup**: Run File → Backup Database at regular intervals to provide roll-back options. These will be automatically stored in the `project\data\backup` folder as time-stamped `.db` files and can be used to manually replace a corrupt `project\data\shots.db`. Manually remove old ones as you see fit.
3. **CSV export**: Use File → Export CSV at regular intervals. This will make time-stamped csv entries under `project\data\csv` for each of the `shots.db` tables. Manually remove these as you see fit.
4. **Routing relationships**: Use File → Save to create regular saves of the routing relationship between the `shots.db` and the `project\media` files. This will be useful in case of complete loss of `shots.db` to rebuild the database. The information is saved to the `project\save` folder as `.aimms` in JSON format. This can also be used to rename `project\media\{shot_id}` folders to `{shot_name}` for migration of media to alternative applications.


#### Media Files Not Loading

**Problem**: Images or videos don't appear in the gallery

**Solutions**:

1. **File Format**: Ensure files are in supported formats (PNG, MP4, MKV etc.)
2. **File Paths**: Verify files haven't been moved or deleted. Confirm folders have not been accidentally moved changing the generic project folder structure.
3. **Refresh**: Press `F5` to refresh the gallery view
4. **Restart**: Restart the application then check the Logs and use options on the Unused page to locate any orphan entries and the Routing Matrix page to confirm entries are all valid. Anything without a green tick in the routing matrix will need investigating. *(Note: Characters, Locations, and Other folder for assets can be empty, other media folders should probably not be)*

### Performance Issues

#### Slow Application Response

**Problem**: AIMMS is slow to respond or lags during operation

**Solutions**:

1. **Close Other Apps**: Free up system memory and CPU to test.
2. **File sizes**: Check for overly large image or video files. It's recommended to work with reasonably sized images and video clips, though edited sequences have been tested over 1 minute long, they can add relative lag to the loading times at larger file size. The `.png` files are almost always loaded with workflow metadata which means >5mb is not uncommon as an average size. AI video clips tend to be only a few seconds long and AIMMS application version 1.0 has been designed around that assumption.
3. **Automatic Caching**: Large projects will use the advanced caching system which may cause storyboard pages to reload on page change *(1 to 2 seconds is possible for large file projects on the video projects page as it caches 50 previews per page, though the caching is designed around using `video_workflow_xx.png` files for previews, not the video files themselves)*
4. **Storage type**: Projects should reside on SSD drives for faster access times. SATA drives are likely to experience slower load times, and external USB drives are recommended for archiving only, not for loading live projects.
4. **Project Size**: The maximum project test size before product launch was 600 shots with 21,000 takes at 23 GB total project size. The advanced caching system is designed to handle any size, in theory.

#### High Memory Usage

**Problem**: AIMMS uses excessive memory or causes system slowdown

**Solutions**:

1. **Memory**: Use a process analyser to confirm what is using the memory. AIMMS is a media package which has some overhead but the image, video and 3d model previewer features are designed with low system ram in mind. In pre-launch tests AIMMS ran on a 4GB ram laptop without a GPU without problems.
2. **Close Other Applications**: Test AIMMS with all other applications especially browser windows closed.
3. **System Resources**: Excessive background processes could hog system resources causing slow down.
4. **Anti-virus software**: Try white-listing the AIMMS and project folders temporarily, especially during large project caching.
5. **Confirm disk health**: Confirm the read-write health of the drive with the AIMMS application, and the drive with the project media files.

#### Slow Media Loading

**Problem**: Images and videos take a long time to load

**Solutions**:

1. **Storage Speed**: Use SSD storage for faster file access for projects in particular. The application is less in need of it, but it will help if your main application drive is SSD not SATA for disk read-write speeds. Try to avoid using older USB external drives for working on projects live. Copy them to your fastest drive and then archive them back is best practise.
2. **Network Issues**: If using network storage, check connection speed
3. **Cache Management**: The cache system is automatic and you do not need to touch it. It may take a moment settling in on initial start and navigation of large projects.
4. **Confirm disk health**: Confirm the read-write health of the drive with the AIMMS application, and the drive with the project media files.

### Import and Export Issues

#### CSV Import Fails

**Problem**: CSV file won't import or shows validation errors

**Solutions**:

1. **File Format**: Ensure CSV follows standard format. Use UTF-8 encoding is recommended.
2. **Required Columns**: Verify all required columns are present and spelt correctly, e.g `shot_names` *(all headings use lower-case and underscores or hyphens, and not capitals or white space)* 
3. **White space after headings**: Check column headers don't have white space at the end or start of column titles. This will cause columns not to be imported.
4. **Data Validation**: Check for empty `shot_names` or invalid data used in fields of the csv. All required data columns must be present, but most fields can be empty except for `shot_names`.
5. **Testing first**: If you plan on importing a large csv to an existing project try importing it to a new project first to confirm it works. This way you can delete the new project once valid importing of the csv data is confirmed.

#### Export/Save/Backup/Archive Problems

**Problem**: Export functions don't work or produce incomplete files

**Solutions**:

1. **Write Permissions**: Ensure write access to export directory
2. **Disk Space**: Check available disk space for export files especially when archiving projects off as `.zip` files *(a 25gb project is best archived manually)*
3. **File Locks**: Ensure files aren't locked by other applications or after crashes

### Display and Interface Issues

#### UI Elements Not Visible

**Problem**: Interface elements are missing or not displaying properly

**Solutions**:

1. **Screen Resolution**: Adjust screen resolution
2. **Theme Issues**: Try switching to a different theme
3. **Graphics Card Settings**: Update or adjust graphics driver settings


#### Text Display Problems

**Problem**: Text appears garbled, too small, or unreadable

**Solutions**:

1. **Font Settings**: Adjust font size in OS system settings
2. **Display Scaling**: Check system display scaling settings for the OS
3. **System Fonts**: Ensure system fonts are properly installed in your OS

### Page Specific Issues

#### Shots Page Problems

**Problem**: Shot management functions not working properly

**Solutions**:

1. **Database Lock**: Check for database locks from other processes
2. **Permissions**: Verify write permissions to project database
3. **Corruption**: Run database validation and manually repair from backups if needed *(it is recommended you duplicate a project before doing this to enable rollback)*
4. **Memory**: Ensure sufficient memory and disk space for large media projects

#### Media Page Issues

**Problem**: Image or video storyboards not working correctly

**Solutions**:

1. **Folder locations**: Check folder structure of the `project` has not been accidentally changed. The folder structure follows strict generic layout to ensure compatibility between AIMMS users.
2. **Codec Issues**: Install appropriate codecs for video playback (`ffmpeg`, `ffprobe`). For Windows they come bundled with the application but Linux and OSX require them installed seperately
3. **Thumbnails & Previews**: Images are also used for thumbnail previews so if they are very large it might slow down preview refreshes on a page. In video storyboard the associated `.png` files are used for previews (`video_workflow_xx.png`)
4. **File Integrity**: Verify media files aren't corrupted
5. **Database Integrity**: Check the Routing matrix and the Unused page features to confirm project integrity with the `shots.db` has not become corrupted.

#### Asset Management Problems

**Problem**: Asset management functions not working

The assets page is image based only and named folders and files for assets are located under `project\media\characters`, `project\media\locations`, and `project\media\other`

Additionally the assets page has a 3d model preview feature, which includes a thumbnail creation option after loading up a 3d model (fbx, glb). The user must manually create the first thumbnail view. If no thumbnail is created or thumbnails have been cleared down, 3d model previews may show a blank or default preview card and require manual setting again. These thumbnail previews will be stored under the relevant asset folder name.

**Solutions**:

1. **File Paths**: Check asset file paths are accessible
2. **Permissions**: Verify read/write permissions for asset files
3. **File Types**: Ensure asset files are in supported formats (png, glb, fbx)
4. **File names**: Assets dont have their file names changed on loading in the same way images and videos do. This may present issues on Windows for long filenames. Rename the asset media file to something shorter before uploading.
4. **Storage Space**: Check available storage for media files

### Error Messages and Logs

#### Understanding Error Messages

When you encounter an error:

1. **Read Carefully**: Note the exact error message
2. **Take Screenshot**: Capture the error for reference
3. **Check Logs**: Review logs in the Logs page for details (timestamps should be in UTC)
4. **Document Steps**: Note what you were doing when the error occurred

#### Using Logs for Troubleshooting

1. **Access Logs**: Go to Logs page (Ctrl+7)
2. **Filter by Time**: Focus on recent log entries (timestamps should be in UTC)
3. **Search for Errors**: Look for ERROR or WARNING level messages. WARNING messages are notification only, but ERROR messages will need to be addressed.
4. **Export Logs**: Export relevant logs for support analysis. Logs are in text file format and will open from the Logs page using your default text editor, so can be saved externally.

### If Requiring Support

Prepare this information:

1. **Error Details**: Exact error messages and when they occur
2. **System Information**: Operating system, AIMMS version, hardware specs
3. **Steps to Reproduce**: Detailed steps to recreate the issue
4. **Log Files**: Relevant log entries from the Logs module
5. **Screenshots**: Visual documentation of the problem

### Preventive Measures

To minimize issues:

1. **Regular Backups**: Save, Backup, Export, Archive regularly
2. **Software Updates**: Keep AIMMS and system software updated to latest version
3. **System Maintenance**: Regular system cleanup and optimization using Unused page features and Routing Matrix checks
4. **Proper Shutdown**: Always close AIMMS properly before shutting down
5. **Documentation**: Keep notes on your workflow process and configurations

Remember: Most issues can be resolved with the steps above. If you're still experiencing problems, contact the developer. AIMMS does not offer instant support at this time, however we will endeavour to address any concerns as quickly as possible.
