# Frequently Asked Questions

## Overview

This section contains answers to frequently asked questions about AIMMS. If you don't find your question here, please check our [Support](../support/index.md) section for additional help.

## General Questions

### What is AIMMS?

AIMMS (Artificial Intelligent Movie Making Systems) is a professional storyboard management application designed for AI filmmakers. It provides comprehensive tools for organizing and managing shots, images, videos, and assets in a structured, efficient way.

### What platforms does AIMMS support?

AIMMS supports Windows 10, Linux, and macOS. It's distributed as a standalone application that requires no installation.

### Is AIMMS free to use?

AIMMS requires a license for full functionality. Trial versions may be available for evaluation purposes.

## Installation and Setup

### How do I install AIMMS?

AIMMS is distributed as a standalone application that requires no installation. Simply download the appropriate version for your platform, extract the files, and run the executable.

### What are the system requirements?

- **Operating System**: Windows 10, Linux (Ubuntu 18.04+), macOS 10.14+
- **Processor**: 2 GHz dual-core processor
- **RAM**: 4GB minimum, 8GB recommended
- **Storage**: 1GB free space
- **Graphics**: OpenGL 3.3+ compatible graphics card

### I'm having trouble installing AIMMS. What should I do?

Please refer to our [Installation Guide](../getting-started/installation.md) for detailed installation instructions and troubleshooting tips.

## Using AIMMS

### How do I create a new project?

1. Launch AIMMS
2. Click **File** → **New Project** (or press `Ctrl+N`)
3. Enter a project name and location
4. Click **Create**

For detailed instructions, see our [First Steps Guide](../getting-started/first-steps.md).

### How do I add shots to my project?

1. Navigate to the **Shots** module (Ctrl+1)
2. Click **Add New Shot**
3. Fill in shot details (order, name, description, prompts)
4. Click **Save**

For comprehensive shot management, see our [Shots Management Guide](../user-guide/shots-management/).

### Can I import existing shot lists?

Yes, AIMMS supports CSV import for shots. See our [Importing Shots Guide](../user-guide/shots-management/importing-shots.md) for details.

### How do I add images and videos to shots?

1. Navigate to **Images** (Ctrl+2) or **Videos** (Ctrl+3) module
2. Select your shot
3. Click **Add Take**
4. Browse and select your media file
5. Click **Add**

For detailed instructions, see our [Image Storyboard](../user-guide/image-storyboard/) and [Video Storyboard](../user-guide/video-storyboard/) guides.

## Technical Questions

### What file formats are supported?

**Images**: PNG, JPG, JPEG, WebP, BMP, TIFF
**Videos**: MP4, WebM, MKV, GIF
**Assets**: Various formats including PDF, DOC, MP3, WAV, and more

### How does AIMMS organize project files?

AIMMS automatically organizes files in a structured folder system:
```
project_root/
├── data/          # Database and data files
├── media/         # Shot media files
├── assets/        # Project assets
├── logs/          # Project and application logs
└── project_config.json
```

### Can I work on multiple projects?

Yes, you can create and switch between multiple projects. Use **File** → **Switch Project** to change projects.

### How do I backup my project?

AIMMS automatically creates backups, but you can also:
1. Use **File** → **Export CSV** for data backup
2. Manually copy your project folder
3. Use cloud storage for additional backup

## Troubleshooting

### AIMMS won't start

- Check system requirements
- Ensure you have extracted all files from the archive
- Try running as administrator (Windows)
- Check antivirus software isn't blocking the application

### Project won't open

- Check file permissions
- Verify project files aren't corrupted
- Ensure sufficient disk space
- Try project recovery tools

### Media files not loading

- Check file format is supported
- Verify file size limits aren't exceeded
- Ensure files haven't been moved or deleted
- Try refreshing the gallery (F5)

### Performance issues

- Close other applications to free memory
- Reduce thumbnail quality in settings
- Clear thumbnail cache if corrupted
- Check available disk space

## Advanced Features

### Can I integrate AIMMS with other tools?

Yes, AIMMS supports integration with various tools including:
- ComfyUI for AI workflow integration
- Project management tools
- Cloud storage services
- Custom integrations via API

### How do I use the starred system?

The starred system helps you mark favorites:
- Click the star icon on any shot, image, or video
- Only one item per category can be starred
- Starred items are highlighted for easy identification
- Use stars to prioritize your best work

### What is the routing matrix?

The routing matrix is an advanced feature for managing complex workflows. It helps you organize and track media files through different processing stages.

## Getting Help

### Where can I find more help?

- [User Guide](../user-guide/) - Comprehensive documentation
- [Features](../features/) - Feature-specific guides
- [Troubleshooting Guide](../getting-started/troubleshooting.md) - Problem-solving help
- [Support](../support/) - Contact information and resources

### How do I report a bug?

Please contact our support team through the [Support](../support/) section with details about the issue, including:
- AIMMS version
- Operating system
- Steps to reproduce the issue
- Any error messages

### Can I suggest new features?

Yes, we welcome feature suggestions! Please contact our support team with your ideas.

## Licensing and Support

### How do I activate my license?

1. Launch AIMMS
2. Enter your license key when prompted
3. Or use **Help** → **License** to enter or manage your license

### What if my license expires?

Contact our sales team to renew your license. You may still be able to access your projects in read-only mode.

### Is there a community or forum?

Check our website for community forums, user groups, and additional resources.

If you have additional questions not covered here, please visit our [Support](../support/) section for more assistance.