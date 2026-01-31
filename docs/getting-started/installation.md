# Installation Guide

## Download and Installation

AIMMS is distributed as a standalone application:

### Step 1: Download

1. Visit the [official AIMMS portal](https://markdkberry.com/software/)
2. Download the latest version for your platform
3. Choose the appropriate file for your operating system:
   - **Windows**: `AIMMS_v1.0.0_Win64.zip`
   - **Linux**: `AIMMS_v1.0.0_Linux.tar.gz`
   - **macOS**: *(planned future release)*

### Step 2: Extract Files

1. **Windows**: Extract the ZIP file to a suitable location, then double click `AIMMS.exe` and follow the instructions.

2. **Linux**: Extract the tar.gz file into a suitable folder then do the following:

   ```
   tar -xzvf AIMMS_v1.0.0_Linux.tar.gz
   cd AIMMS_v1.0.0_Linux
   ./main-aimms_qt.bin
   ```

### Step 3: Launch Application

1. **Windows**: Double-click `AIMMS.exe` from the extracted directory
2. **Linux**: Run `./main-aimms_qt.bin` from the extracted directory

On first launch you will be asked to choose a valid project or setup a new one. It's recommended to preface project names with `project_` or something you can easily recognise as AIMMS project folders in the future.

The AIMMS software will suggest a local `AIMMS Project` location but you can choose anywhere you like.

Once completed a restart of the application is necessary. This is common between projects to protect the database integrity and ensure a defined moat between projects.

You will also notice a console window is present as well as the application on the task bar. Future versions will provide the ability to disable the console window but for v1.0.0 it will help with debugging any issues that arise.

### Step 4: License Activation

1. After setting up a project, on the next launch you'll be prompted for a license.
2. Enter your email address to start a one-time 30 day trial.
3. Alternatively you can purchase a .lic license file via the online store and load it into the browser then activate it.
3. The application will validate then activate the license, and either the trial countdown will begin, or the license will engage giving you permanent use of vrs 1.x.

Note: The 30 day trial is one-time only and after that a license should be purchased.

Note: Your .lic license file for AIMMS version 1.x will work in perpetuity. It is associated with your email address. Please keep a copy of the file somewhere safe. If you lose it contact the point of purchase. Once validated, the license file is stored in the `\licensing` folder on your system.

You may install and use AIMMS on more than one of your own devices for personal use, including across supported platforms (Windows and Linux (OSX on release)).

## System Requirements

### Minimum Requirements

- **Operating System**: Windows 10, Linux (Ubuntu 18.04+)
- **Processor**: 2 GHz dual-core processor
- **RAM**: 4GB
- **Storage**: at least 1.5GB free space for the application
- **Graphics**: OpenGL 3.3+ compatible graphics card

### Recommended Requirements

- **Operating System**: Latest version of Windows 10/11, Linux
- **Processor**: 2.5 GHz quad-core processor or better recommended
- **RAM**: 8GB or more recommended
- **Storage**: SSD with 1.5GB free space for application
- **Graphics**: graphics cards capable of using ffmpeg and ffprobe *(NOTE: a GPU with VRAM is not necessary)*

*NOTE: Projects will grow as large as you make them and remain seperate to the functioning of the application itself. For example, a 600 shot, 21K take project was over 25GB in file size and stored on an external SSD.*

*The size of the project has minimal impact on the application, though larger projects need to manage cache loading on previews for image and video files, this has been streamlined in the code.*


## Troubleshooting Installation

### Common Issues

#### Application Won't Launch

**Problem**: AIMMS fails to start

**Solutions**:

- Check that your system meets minimum requirements
- Ensure you have extracted all files from the archive
- Try running as administrator (Windows)
- Check antivirus software isn't blocking the application

#### License Activation Problems
**Problem**: License file not accepted

**Solutions**:

- Verify the license file is valid *(.lic with json format information)*
- Check you recieved a license file on purchase *(associated to email address)*
- Contact support if the issue persists
- You do not need to be online to activate the license

#### Missing Dependencies
**Problem**: Error about missing libraries or dependencies

**Solutions**:

- Ensure you downloaded the correct version for your platform
- Check that all files were extracted properly
- Try re-downloading from the official website
- On Linux you will need to install ffmpeg and ffprobe seperately *(On Windows, ffmpeg and ffprobe are bundled with the application)*

#### Performance Issues
**Problem**: Application runs slowly or lags

**Solutions**:

- Check your system resources
- Confirm you have current version of ffmpeg and ffprobe
- Ensure you have sufficient free disk space *(including swap files)*
- Update your graphics drivers
- Large projects *(e.g. 600 shots with 21K takes)* can cause a few seconds delay during opening of projects and page changes, as they reload and manage cached image and video previews.
- Run *"Analyze Zeroed-Out Takes"* from the *Unused* page and confirm the placeholder media files are safe to delete. Excessive numbers of empty take placeholders may slow down the caching system on large projects.

### Platform-Specific Issues

#### Windows
- **UAC Issues**: Run as administrator if you encounter permission errors
- **Antivirus**: Add AIMMS to your antivirus exclusion list
- **Graphics**: Ensure your graphics drivers are up to date

#### Linux
- **Permissions**: Make the executable file executable: `chmod +x aimms`
- **Dependencies**: Install required libraries if prompted
- **Desktop Integration**: Create desktop shortcuts for easier access

## Post-Installation Verification

### Verify Installation
1. Launch AIMMS successfully
2. Create a test project
3. Verify all modules load correctly
4. Test basic functionality (add shot, import image)
5. Check that settings are saved properly

### Update Check
1. AIMMS will require manual checks for updates
2. Download updates as they become available *(standalone package)*
3. Ensure you have a copy of your license key and email
4. Rename the old version folder
5. Download and extract the new version
6. Test the new version before deleting the old version

## Getting Help

### Built-in Help
- **Documentation**: Access via Help → Documentation *(This website)*


### Online Resources
- [**Official Website**](https://markdkberry.com/software/): Visit for latest downloads and news
- [**Patreon (Free tier)**](https://www.patreon.com/c/AIMakingMovies): For latest updates and information
- [**Documentation**](https://ai-making-movies.github.io/aimms-docs/): Comprehensive user guides
- [**Video Tutorials**](https://www.youtube.com/playlist?list=PLVCJTJhkunkRutnutiP9dgd6crw8MWEHN): Step-by-step video guides
- [**Github Issues**](https://github.com/AI-Making-Movies/aimms-docs/issues): Report bugs, suggest improvements. *(There is no guaranteed support or response time. Issues will be addressed when time permits.)*

## Next Steps

After successful installation:

*While this site is in development it is recommended you check the [**Video Tutorials**](https://www.youtube.com/playlist?list=PLVCJTJhkunkRutnutiP9dgd6crw8MWEHN) for the most up to date information on use. - Jan 2026*

1. **Create Your First Project**: Follow the Quick Start Guide
2. **Explore the Interface**: Familiarize yourself with the main modules
3. **Import Existing Data**: Use CSV import if you have existing shot lists
4. **Customize Settings**: Adjust to your preferences
5. **Learn the Workflow**: Understand the complete AIMMS workflow

Your AIMMS installation is now ready for professional storyboard management!