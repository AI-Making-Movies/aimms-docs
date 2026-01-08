# Frequently Asked Questions

## Overview

This section contains answers to frequently asked questions about AIMMS.

## General Questions

### What is AIMMS?

AIMMS (Artificial Intelligent Movie Making Systems) is a professional storyboard management application designed for AI filmmakers. It provides comprehensive tools for organizing and managing shots, images, videos, and assets in a structured, efficient way.

### What platforms does AIMMS support?

AIMMS supports Windows 10, Linux, and macOS. It's distributed as a standalone application that requires no installation.

### Is AIMMS free to use?

AIMMS requires a license for full functionality.

## Installation and Setup

### How do I install AIMMS?

AIMMS is distributed as a standalone application that requires no installation. Simply download the appropriate version for your platform, extract the files, and run the executable.

### What are the system requirements?

- **Operating System**: Windows 10, Linux (Ubuntu 18.04+), macOS 10.14+
- **Processor**: 2 GHz dual-core processor
- **RAM**: 4GB minimum, 8GB recommended
- **Storage**: 1GB free space
- **Graphics**: OpenGL 3.3+ compatible graphics card *(GPU not required. `ffmpeg` and `ffprobe` are bundled with Windows version, Linux and OSX require them installed seperately)*

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

1. Navigate to the **Shots** page (Ctrl+1)
2. Click **Add New Shot**
3. Fill in shot details (shot name, description, prompts, etc...)
4. Click **Save**


### Can I import existing shot lists?

Yes, AIMMS supports CSV import for shots.

1. Navigate to the **Shots** page (Ctrl+1)
2. Click **Import CSV**
3. Locate a valid csv containing required columns
4. Click **Validate** and then **Import**

### How do I add images and videos to existing shots?

1. Navigate to **Images** (Ctrl+2) or **Videos** (Ctrl+3) page
2. Select your shot
3. Click on **View Media** to open the Takes popup modal
4. Click **Add Take** to add more empty placeholders
5. Click **Replace** to replace empty placeholders with valid media 
5. Browse and select your media file

## Technical Questions

### What file formats are supported?

**Images**: PNG

**Videos**: MP4, MKV

**Assets**: Image or 3D Model formats including PNG, GLB, FBX

### How does AIMMS organize project files?

AIMMS automatically organizes files in a structured folder system:
```
project_root/
├── data/          # Database and backup data files
├── media/         # Shot media files
├── logs/          # Project and application logs
└── project_config.json
```

### Can I work on multiple projects?

Yes, you can create and switch between multiple projects. Use **File** → **Open Project** to change projects. This will require a restart of the application.

### How do I backup my project?

AIMMS provides several backup options under the File menu:

1. **Archive Project**: Archive a complete project folder to a time-stamped `.zip` file *(For large projects this might be best done manually with the AIMMS application closed)*
2. **Backup Database**: Run File → Backup Database at regular intervals to provide roll-back options. These will be automatically stored in the `project\data\backup` folder as time-stamped `.db` files and can be used to manually replace a corrupt `project\data\shots.db`. Manually remove old ones as you see fit.
3. **CSV export**: Use File → Export CSV at regular intervals. This will make time-stamped csv entries under `project\data\csv` for each of the `shots.db` tables. Manually remove these as you see fit.
4. **Routing relationships**: Use File → Save to create regular saves of the routing relationship between the `shots.db` and the `project\media` files. This will be useful in case of complete loss of `shots.db` to rebuild the database. The information is saved to the `project\save` folder as `.aimms` in JSON format. This can also be used to rename `project\media\{shot_id}` folders to `{shot_name}` for migration of media for use in alternative applications.


## Troubleshooting

For detailed instructions, see the [Troubleshooting Guide](../getting-started/troubleshooting.md).


## Advanced Features

### Can I integrate AIMMS with other tools?

Version 1.0 is a passive storyboard management system but future versions will integrate with tools such as ComfyUI and LLMs via API.

The `project\data\shots.db` is SQLite3 and can be accessed using python code. However, to avoid corruption be certain to keep regular backups and only access the database as read-only.

`.aimms` file is provided in the `\project\data\saves` folder and updated using File → Save. This is a JSON format file which can be used to rename the `media\{shot_id}` folders for migration out of AIMMS project structure. This file is provided to keep a record of the relationships structure between media folders (named using `shot_id`) and `shot_names`.

An inbound migration tool is on [github](https://github.com/mdkberry/migrating-to-aimms) for importing media into AIMMS from other platform. It provides the current version project folder structure and database schema, and is open to the public for code development to enable further integration.


### How do I use the starred system?

The starred system helps you mark favorite takes:

- Click the star icon in any shot in the image, or video storyboard popup take modal
- Only one item per shot can be starred and it will appear in the preview card for that shot
- Use stars to prioritize your best takes

### What is the routing matrix?

The routing matrix is for checking at a glance the health of media and database relationships. A green tick shows both are present. A red X means either the database or the media folder is missing an entry or has corrupted data.

Fixing orphan issues in either direction is done through further analysis in the Unused page to assess what the problem is and tidy up orphan entries.

## Getting Help

### Where can I find more help?

- [Getting Started](../getting-started/) - Comprehensive documentation on use
- [Troubleshooting Guide](../getting-started/troubleshooting.md) - Problem-solving help

### How do I report a bug?

Please log bugs on the [github issues](https://github.com/AI-Making-Movies/aimms-docs/issues) page, and be sure to include:

- AIMMS version
- Operating system
- Steps to reproduce the issue
- Any error messages

We cannot promise instant support but issues will be tended to in as timely a manner as possible.

## Licensing and Support

### How do I activate my license?

1. Launch AIMMS
2. Enter your license key and email when prompted

### What if my license doesnt work?

Check the [Troubleshooting Guide](../getting-started/troubleshooting.md)

If that does not resolve your issue then contact point of sale with your details of purchase.

You will always be to access your projects manually.

### Is there a community or forum?

Check the [website](https://markdkberry.com/software/) for community forums, user groups, and additional resources.
