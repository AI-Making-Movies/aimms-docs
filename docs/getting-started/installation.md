# Installation Guide

## Download and Installation

AIMMS is distributed as a standalone application:

### Step 1: Download

1. Visit the official AIMMS website *(coming soon)*
2. Download the latest version for your platform
3. Choose the appropriate file for your operating system:
   - **Windows**: `aimms_windows_x64.zip`
   - **Linux**: `aimms_linux_x64.tar.gz`
   - **macOS**: `aimms_macos_x64.dmg`

### Step 2: Extract Files

1. **Windows**: Extract the ZIP file to your desired location
2. **Linux**: Extract the tar.gz file using `tar -xzf aimms_linux_x64.tar.gz`
3. **macOS**: Open the DMG file and drag AIMMS to your Applications folder

### Step 3: Launch Application

1. **Windows**: Double-click `main-aimms_qt.exe`
2. **Linux**: Run `./aimms` from the extracted directory
3. **macOS**: Launch from Applications folder or extracted location

### Step 4: License Activation

1. On first launch, you'll be prompted for a license key
2. Enter your email and license key when prompted *(recieved on purchase)*
3. The application will validate and activate

*NOTE: Your license key for AIMMS version 1.0 is associated to your email address, keep it safe. After validation it will be stored in a file on your system.*

## System Requirements

### Minimum Requirements

- **Operating System**: Windows 10, Linux (Ubuntu 18.04+), macOS 10.14+
- **Processor**: 2 GHz dual-core processor
- **RAM**: 4GB
- **Storage**: 1GB free space for the application
- **Graphics**: OpenGL 3.3+ compatible graphics card

### Recommended Requirements

- **Operating System**: Latest version of Windows 10/11, Linux, or macOS
- **Processor**: 2.5 GHz quad-core processor or better recommended
- **RAM**: 8GB or more recommended
- **Storage**: SSD with 1GB free space for application
- **Graphics**: graphics cards capable of using ffmpeg and ffprobe *(NOTE: a GPU with VRAM is not necessary)*

*NOTE: Projects will grow as large as you make them and remain seperate to the functioning of the application itself. For example, a 600 shot, 21K take project was over 25GB in file size and stored on an external SSD. The size of the project had minimal impact on the application, though larger projects need to manage cache loading on previews for image and video files, this has been streamlined in the code.*

## First-Time Setup

### Initial Configuration

1. **Enter License Key**: On starting the application for the first time. Email address and valid license key.
2. **Default Project Location**: Choose where to save your project, or open and validate an existing AIMMS project *(subject to version control and migration)*.


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
**Problem**: License key not accepted

**Solutions**:

- Verify the license key is entered correctly
- Check you recieved a license key on purchase *(associated to email address)*
- Contact support if the issue persists
- You do not need to be online to activate the license

#### Missing Dependencies
**Problem**: Error about missing libraries or dependencies

**Solutions**:

- Ensure you downloaded the correct version for your platform
- Check that all files were extracted properly
- Try re-downloading from the official website
- On Linux and OSX you will need to install ffmpeg and ffprobe seperately *(On Windows, ffmpeg and ffprobe are bundled with the application)*

#### Performance Issues
**Problem**: Application runs slowly or lags

**Solutions**:

- Check your system resources
- Confirm you have current version of ffmpeg and ffprobe
- Ensure you have sufficient free disk space *(including swap files)*
- Update your graphics drivers
- Large projects *(e.g. 600 shots with 20K takes)* can cause a few seconds delay during opening of projects and page changes, as they reload and manage cached image and video previews.
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

#### macOS
- **Gatekeeper**: If blocked by Gatekeeper, right-click and select "Open"
- **Permissions**: Grant necessary file system permissions when prompted
- **Rosetta**: On Apple Silicon Macs, ensure Rosetta is installed if needed

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
- [**Documentation**](https://ai-making-movies.github.io/aimms-docs/): Comprehensive user guides and tutorials
- **Community Forum**: User discussions and support *(planned)*
- [**Video Tutorials**](https://www.youtube.com/@markdkberry): Step-by-step video guides

### Support Contact
- **Email Support**: *coming soon*
- **Bug Reports**: *coming soon*
- **Feature Requests**: *coming soon*

## Next Steps

After successful installation:

1. **Create Your First Project**: Follow the Quick Start Guide
2. **Explore the Interface**: Familiarize yourself with the main modules
3. **Import Existing Data**: Use CSV import if you have existing shot lists
4. **Customize Settings**: Adjust to your preferences
5. **Learn the Workflow**: Understand the complete AIMMS workflow

Your AIMMS installation is now ready for professional storyboard management!