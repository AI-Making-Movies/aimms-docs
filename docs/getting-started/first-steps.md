# First Steps with AIMMS

## Welcome to AIMMS!

This guide will help you get started with AIMMS and create your first project in just a few minutes.

## Your First Project

### Step 1: Create a New Project

1. **Launch AIMMS**:
    
    - Double-click the AIMMS application
    - Wait for the application to load completely

2. **Create New Project**:

    - Click **File** → **New Project** (or press `Ctrl+N`)
    - Enter a project name (e.g., "My Short Film")
    - Choose a location to save your project
    - Click **Create**

3. **Project Structure Created**:

   - AIMMS automatically creates this structure:

        ```
        Your_Project/
        ├── data/
        │   ├── shots.db
        │   ├── csv/
        │   ├── backup/
        │   └── saves/
        ├── media/
        ├── assets/
        ├── logs/
        └── project_config.json
        ```

### Step 2: Understand the Interface

AIMMS uses a tabbed interface with 8 main modules:

- **Shots** (Ctrl+1): Manage your shot list and details
- **Image Storyboard** (Ctrl+2): View and manage base image storyboard
- **Video Storyboard** (Ctrl+3): View and manage final video storyboard
- **Assets** (Ctrl+4): Manage project assets
- **Unused** (Ctrl+5): Clean up unused media files
- **Settings** (Ctrl+6): Configure project settings
- **Logs** (Ctrl+7): View application and project logs
- **Routing** (Ctrl+8): Routing health between database and media files

### Step 3: Add Your First Shot

1. **Navigate to Shots Page**:

    - Click the **Shots** tab or press `Ctrl+1`

2. **Add New Shot**:

    - Click **Add New Shot** button
    - Fill in the shot details:
        - **Order Number**: 1 *(sequence position can be changed to re-order shots across the storyboards)*
        - **Shot Name**: `INT_OFFICE_DAY_001` *(Unique naming is recommended but not enforced)*
        - **Section**: `Act 1 - Opening Scene` *(group shots by sections for later filtering as projects get larger)*
        - **Description**: `Hero enters office`
        - **Image Prompt**: `A man sitting at a desk in a modern office`
        - **Video Prompt**: `A man walks into an office and sits at his desk`
        - Add other metadata as required. *(All entries are optional except `shot_name` which must be provided. Though the shot name does not need to be unique, it is highly recommended to make it so.)*

[continue from here]

3. **Save the Shot**:

    - Click **Save** to add the shot to your project
    - The shot will appear in the shots table

### Step 4: Add Media to Your Shot

#### Adding a Base Image

1. **Navigate to Images Module**:

    - Click the **Images** tab or press `Ctrl+2`

2. **Add Image Take**:

    - Select your shot from the gallery
    - Click **Add Take**
    - Browse and select your image file
    - Choose take number (e.g., `base_01`)
    - Click **Add**

3. **View Your Image**:

    - The image will appear in the gallery
    - Double-click to view it full-size in the floating viewer
    - Click the star icon to mark it as your favorite

#### Adding a Video

1. **Navigate to Videos Module**:

    - Click the **Videos** tab or press `Ctrl+3`

2. **Add Video Take**:

    - Select your shot from the gallery
    - Click **Add Take**
    - Browse and select your video file
    - Choose take number (e.g., `video_01`)
    - Click **Add**

3. **View Your Video**:

    - The video will appear in the gallery
    - Click to play it in the floating video player
    - Click the star icon to mark it as your favorite

### Step 5: Explore Your Project

1. **View All Modules**:

    - Navigate through each tab to see your content
    - Notice how your shot appears in all relevant modules

2. **Use Keyboard Shortcuts**:

    - Practice using `Ctrl+1` through `Ctrl+8` to switch tabs
    - Try `Ctrl+N` for new project, `Ctrl+O` for open project

3. **Search and Filter**:

    - Use the search box in the Shots module to find your shot
    - Try filtering by section to organize your view

## Essential Keyboard Shortcuts

| Shortcut | Action | Module |
|----------|--------|---------|
| `Ctrl+1` | Switch to Shots | All |
| `Ctrl+2` | Switch to Images | All |
| `Ctrl+3` | Switch to Videos | All |
| `Ctrl+4` | Switch to Assets | All |
| `Ctrl+5` | Switch to Unused | All |
| `Ctrl+6` | Switch to Settings | All |
| `Ctrl+7` | Switch to Logs | All |
| `Ctrl+8` | Switch to Routing | All |
| `Ctrl+N` | New Project | All |
| `Ctrl+O` | Open Project | All |
| `Ctrl+E` | Export CSV | All |
| `Ctrl+I` | Import CSV | All |
| `F5` | Refresh View | All |
| `F11` | Toggle Fullscreen | All |

## Basic Workflow

1. **Plan**: Create shots with descriptions and prompts
2. **Generate**: Use your AI tools to create images/videos based on prompts
3. **Import**: Add generated media to AIMMS
4. **Review**: View and organize your media
5. **Iterate**: Replace takes as needed
6. **Export**: Export your storyboard for sharing

## Tips for Success

### Naming Conventions:

    - Use descriptive shot names: `INT_OFFICE_DAY_001`
    - Include location and key action
    - Keep names consistent across your project

### Organization:

    - Use sections to group related shots: `Act 1`, `Opening Scene`, `Climax`
    - Star your favorite takes for easy identification
    - Regularly clean up unused media files

### Workflow Efficiency:

    - Create all shots before adding media
    - Use keyboard shortcuts for faster navigation
    - Regularly export CSV files for backup

## Next Steps

### Explore Advanced Features:

    - **Import Existing Data**: Use CSV import to bring in existing shot lists
    - **Customize Settings**: Adjust themes and preferences to your liking
    - **Learn Advanced Modules**: Explore Assets, Logs, and Routing modules

### Practice with Examples:

    - Create a simple 3-shot scene
    - Practice adding different types of media
    - Experiment with the starred system
    - Try the search and filtering features

### Learn Best Practices:

    - Read the detailed user guides for each module
    - Watch video tutorials for visual learning
    - Join the community for tips and support

## Troubleshooting Common Issues

### Shot Not Appearing:

    - Check that you saved the shot successfully
    - Verify you're viewing "All Sections" in the filter
    - Try refreshing the view with `F5`

### Media Not Loading:

    - Ensure files are in supported formats (PNG, JPG, MP4, etc.)
    - Check file paths are accessible
    - Verify file sizes aren't too large

### Application Performance:

    - Close other applications to free up memory
    - Reduce thumbnail quality in settings if needed
    - Ensure sufficient disk space is available

## Getting Help

### Built-in Help:

    - **Documentation**: Press `F1` or go to Help → Documentation
    - **Keyboard Shortcuts**: Press `Ctrl+K` or go to Help → Keyboard Shortcuts
    - **Context Help**: Right-click any element for specific help

### Online Resources:

    - **User Guides**: Comprehensive step-by-step instructions
    - **Video Tutorials**: Visual guides for common tasks
    - **Community Forum**: Ask questions and share tips

### Support:

    - **Logs**: Check the Logs module for error information
    - **Export Data**: Use export features to share project data with support
    - **Contact**: Reach out to support for technical assistance

Congratulations! You've successfully created your first AIMMS project and learned the basics. Continue exploring the application and refer to the detailed user guides as you become more familiar with the features.