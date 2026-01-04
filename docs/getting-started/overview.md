# AIMMS Overview

## What is AIMMS?

AIMMS (Artificial Intelligent Movie Making Systems) is a professional storyboard management application designed for AI filmmakers. It provides a comprehensive solution for organizing and managing your shots, images, videos, and assets in a structured, efficient way.

**AIMMS Version 1.0 (StorM)** is a passive storyboard management system. Future versions will integrate with AI systems using API and batch workflow processing.

## Key Concepts

### Projects
A project in AIMMS represents your entire film or video production. Each project contains:

- **Shots**: Individual shot list; csv column styled database of shot information.
- **Images**: Base images for each shot containing workflow metadata.
- **Videos**: Final video outputs for each shot with associated workflow metadata png files.
- **Assets**: Characters, locations, and other asset types (images and 3d models).

### Shots
Shots are the fundamental building blocks of your project. Each shot contains:

- **Order Number**: Sequence position in your storyboard
- **Shot Name**: Descriptive identifier (e.g., "INT_OFFICE_DAY_001")
- **Section**: Grouping for organization (e.g., "Act 1", "Opening Scene")
- **Description**: Brief explanation of what happens in the shot
- **Prompts**: AI prompts for generating images and videos
- **Metadata**: Location, time of day, color scheme, etc.

### Storyboards

There are two seperate storyboards but they share the same shot name database entries.

- **"Image Storyboard"**
- **"Video Storyboard"**

The storyboards should be treated as seperate entities used at different stages of a project's development.

The Image storyboard is used to develop the planning stages of a film project, and the video storyboard is used when working toward the final cut for clip takes.

### Takes
Each shot can have multiple "takes", i.e. different versions of the same shot:

- **Image Storyboard Takes**: Different base images for the same shot
- **Video Storyboard Takes**: Different final videos for the same shot with matching workflow metadata png file
- **Starred Takes**: Your favorite version of each shot

### Assets
Assets are non-shot images that will be used in the production:

- **Characters**: Images of characters you plan to use in the project.
- **Locations**: Images of locations you plan to use in the project.
- **Other**: Any other asset images.

    - **3D Models**: 3d model file types (glb, fbx) feature in a lot of AI video production work and have been included in AIMMS version 1.0 along with a previewer in the Assets page.

## System Requirements

*NOTE: a GPU is not required for AIMMS Version 1.0*

- **Operating System**: Windows 10, Linux, or macOS
- (**Python**: 3.12 included in standalone build. You will need **ffmpeg, ffprobe** if not running on Windows.)
- **RAM**: 4GB minimum, 8GB recommended
- **Storage**: 1GB free space for application + project storage as needed *(For example: a 600 shot project with 21K takes exceeded 25GB in file size, but the application has been designed to be able to work with small or large projects with minimal impact on system resources)*

## Application Architecture

AIMMS uses a modular, tabbed interface with 8 main modules:

1. **Shots**: Manage your shot list and details *(sqlite3 database)*
2. **Image Storyboard**: View and manage base images for each shot
3. **Video Storyboard**: View and manage final video clips for each shot
4. **Assets**: Manage asset images & 3D models *(locations, characters, other)*
5. **Unused**: Clean up unused placeholder files and find media orphans
6. **Settings**: Configure project settings
7. **Logs**: View application and project logs
8. **Routing**: Routine matrix connectivity health *(between media files and database)*

## Project Organization

AIMMS automatically organizes your project files in a structured folder system which is located on a drive of your choosing and external to the application:

```
project_root/
├── data/
│   ├── shots.db              # Main database (sqlite3)
│   ├── csv/                  # Exported CSV files
│   ├── backup/              # Database backups
│   └── saves/               # Media relationship backups (.aimms)
├── media/                   # Shot media files
│   ├── 1/                   # Shot 1 folder (shot_id not shot_name)
│   ├── 2/                   # Shot 2 folder
│   └── ...                  # Additional shot folders
├── assets/
│   ├── characters/          # character assets
│   ├── locations/           # location assets
│   └── other/               # other assets
├── logs/                    # Project and application 
└── project_config.json      # Project config info
```

## Workflow Integration

AIMMS is designed to manage administration of your AI generated content on a per project basis:

- **Prompt & Metadata Management**: Store and organize AI prompts and metadata for images and videos
- **Media Organization**: Automatically organize generated content by shot in two storyboard types
- **Quality Control**: Compare different takes and select the best versions
- **Export Options**: Export your storyboard for sharing or further processing

## Getting Started

To begin using AIMMS:

1. **Create a New Project**: Start with File → New Project
2. **Add Shots**: Create your shot list with descriptions and prompts (or import a csv containing a prepared shot list)
3. **Import Media**: Use your AI tools to create images and videos then import the results as shot/takes into AIMMS.
4. **Organize**: Star your favorites and organize your project visually.
5. **Export**: Share your storyboard and content or export workflows to work on further.

## Next Steps

- **Installation**: Learn how to install and set up AIMMS
- **First Project**: Follow our step-by-step guide to create your first project
- **User Guide**: Explore detailed guides for each module
- **Troubleshooting**: Find solutions to common issues