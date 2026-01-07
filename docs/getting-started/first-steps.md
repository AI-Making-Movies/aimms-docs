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
    - Enter a project name (e.g., "project_MyShortFilm")
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
        │   ├── {shot_id}/          
        │   ├── characters/
        │   ├── locations/
        │   └── other/
        ├── logs/
        └── project_config.json
        ```

### Step 2: Understand the Interface

AIMMS uses a tabbed interface with 8 main modules:

- **Shots** (Ctrl+1): Manage your shot list and details
- **Image Storyboard** (Ctrl+2): View and manage base image storyboard
- **Video Storyboard** (Ctrl+3): View and manage final video storyboard
- **Assets** (Ctrl+4): Manage project assets (characters, locations, other)
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

3. **Save the Shot**:

    - Click **Save** to add the shot to your project
    - The shot will appear in the shots table

### Step 4: Add Media (Takes) to Your Shot

Media is added to shots by creating empty placeholder "Takes" then replacing them with valid media. There are two places this can be done manually: 

1. From the Shots Page with "Add Takes" button (creates empty placeholder takes in both Image and Video storyboards for that shot).

2. From within the shot popup modals of the Image or Video Storyboard pages (creates empty placeholder takes only in the storyboard you action it from).

#### Adding Base Image "Takes"

1. **Navigate to Images Storyboard Page**:

    - Click the **Images** tab or press `Ctrl+2`

2. **Add Image Take(s)**:

    - Select your shot from the gallery
    - Click "View Media" button.
    - Click **Add Take** button from the popup modal for the shot.
    - Choose the number of takes you wish to add (empty placeholders will be created)
    - Select **Replace** button in the popup modal for an empty take
    - Browse and select your valid image file *(workflow metadata png)*
    - Click **Add** 

3. **View Your Image**:

    - The image will appear in the gallery
    - Double-click to view it full-size in the floating viewer
    - Click the star icon to mark it as your favorite

**Note**: Imported media will not retain their file names on import, but will be renamed and added to the `\media\{shot_id}\` folder using `base_image_xx.png` for images.

#### Adding a Video

1. **Navigate to Videos Storyboard Page**:

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

**Note**: Imported media will not retain their file names on import, but will be renamed and added to the `\media\{shot_id}\` folder. For the video storyboard, two empty placeholder files are created and required per take during replacement; `final_video_xx.mp4` and `video_workflow_xx.png` which is the accompanying png file that must be supplied with the video at upload *(it assumes a workflow metadata png file will be stored with the video, this will also be used as preview image)*.

### Step 5: Explore Your Project

1. **View All Modules**:

    - Navigate through each tab to see your content
    - Notice how your shot appears in all relevant modules

2. **Use Keyboard Shortcuts**:

    - Practice using `Ctrl+1` through `Ctrl+8` to switch tabs
    - Try `Ctrl+N` for new project, `Ctrl+O` for open project

3. **Search and Filter**:

    - Use the search box in the Shots Page module to find your shot
    - Try filtering by section (bottom menu bar) to organize your view. Section filtering is retained as you navigate between pages. 
    - To show all shots change the filter back to "All Sections".

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

1. **Plan**: Create shots with descriptions and prompts.
2. **Generate**: Use your AI tools to create images/videos based on prompts
3. **Import**: Add generated media to AIMMS
4. **Review**: View and organize your media
5. **Iterate**: Replace takes as needed
6. **Export**: Export your storyboard for sharing

## Tips for Success

### Naming Conventions:

- Use descriptive shot names: `INT_OFFICE_DAY_001` or `HWM_01A_01A_first_scene`
- Include location and key action if you are familiar with that method
- Keep shot name management consistent and unique across your project, but be aware it is not enforced.
- If managing shots is new to you trial this approach: `HWM_01A_01A_first_scene` which breaksdown as: `{Project name}_{Scene number}_{Shot number of scene}_{short_descriptor}`


### Organization:

- Use sections to group related shots: `Act 1`, `Opening Scene`, `Climax`. 
- Star your favorite takes for easy identification (Image and Video Storyboard pages)
- Regularly clean up unused media files (Unused page)

### Workflow Efficiency:

- Create all shots before adding media (ideally create a csv of all shots with their metadata, then import)
- Use keyboard shortcuts for faster navigation
- Regularly export CSV files for backup
- At the end of each session save (.aimms routing info), backup the database.
- At the end of big media import changes archive the entire project to a zip file and copy it off site.

NOTE: We can not be held responsible for loss of data. Backups and features to rescue corrupt databases, stored connection integrity for re-creation of failed data has been provided in several ways. We highly recommend you save, backup, and archive regularly for peace of mind.

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
- If that fails change between the pages
- As a last resort restart the application.

**NOTE**: If a take or shot is still not showing up, then run the "Analyze Zeroed-Out Takes" button in Unused page. It might be there was a failure to connect the media to the database. If your shot shows there, delete it, restart the application and then try again. If the problem continues, check permissions on folders or locked files.

### Media Not Loading:

- Ensure files are in supported formats (PNG, JPG, MP4, etc.)
- Check file paths are accessible
- Verify file sizes aren't too large

**NOTE**: AIMMS has been tested with a 600 shot project containing 21,000 takes with a total size of 23GB in media files and it worked fine. The only delay (1 to 2 seconds) was cache related in managing the navigation between pages (50 videos per page when caching). But this was with 3 to 5 second long clips and only a few larger ones. If your individual clips are huge (which can happen for edited sequences) then you will need to account for that in use of the Storyboard management software.

### Application Performance:

AIMMS has been made with low processing overhead in mind. This is to allow for ComfyUI to run on the same machine with it open if necessary. However, AIMMS does not need to use a GPU and has been tested running on cheap 4GB ram laptop without issue. It uses ffmpeg and ffprobe for video previewing (bundled with Windows version of AIMMS application, but those will need to be provided with Linux or OSX).

It should not need much to run, but if you have problems, ensure sufficient disk space is available and that system ram is not full during use.

Projects are best stored on SSD drives for speed of media loading. This could be on network or external drives. If you are storing projects on SATA or slow USB external drives this might impact speed of performance. While the AIMMS application does not need to run on SSD drive, it will perform better if it does.

## Getting Help

### Built-in Help:

- **Documentation**: Press `F1` or go to Help → Documentation
- **Keyboard Shortcuts**: Press `Ctrl+K` or go to Help → Keyboard Shortcuts

### Online Resources:

*(The below features are planned for implementation after launch)*

- **User Guides**: Comprehensive step-by-step instructions
- **Video Tutorials**: Visual guides for common tasks 
- **Community Forum**: Ask questions and share tips

### Support:

- **Logs**: Check the Logs page module for error information
- **Export Data**: Use export features to help track health of project data if you need to seek support

Congratulations! You've successfully created your first AIMMS project and learned the basics. Continue exploring the application and refer to the detailed user guides as you become more familiar with the features.