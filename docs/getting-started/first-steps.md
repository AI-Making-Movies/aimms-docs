# First Steps with AIMMS

## Welcome to AIMMS!

This guide will help you get started with AIMMS and create your first project in just a few minutes.

Check the [**Video Tutorials**](https://www.youtube.com/playlist?list=PLVCJTJhkunkRutnutiP9dgd6crw8MWEHN) for up to date information on use.

## Your First Project

For first time setup of licensing see [installation](../getting-started/installation.md)

### Step 1: Create a New Project

1. **Launch AIMMS**:
    
    - *Windows*: Double-click the `AIMMS.exe` application
    - *Linux*: launch `./main-aimms_qt.bin`
    - Wait for the application to load completely
    - A console window will provide debug information *(this will be possible to hide in future versions)*

2. **Create New Project**:

    - *(First time use will offer a dialogue popup to browse or create a a new project)*
    - Click **File** → **New Project** (or press `Ctrl+N`)
    - Enter a project name (e.g., "project_MyShortFilm")
    - Choose a location to save your project *(do not save projects to the application folder)*
    - Click **Create**

3. **Project Structure Created**:

   - AIMMS automatically creates this structure:

        ```
        Your_Project/
        ├── data/
        │   ├── shots.db
        │   ├── shot_name_mapping.json
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

AIMMS uses a tabbed interface with 8 main page modules:

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
        - **Shot Name**: `INT_OFFICE_DAY_001` *(Unique naming is recommended but not enforced)*. (One approach is to use `HWM_01A_01A_first_scene` which breaksdown as: *`{Project name}_{Scene number}_{Shot number of scene}_{short_descriptor}`*)
        - **Section**: `1. Opening Scene` *(group shots by sections for later filtering as projects get larger)*
        - **Description**: `Hero enters office`
        - **Image Prompt**: `A man walking into a modern office`
        - **Video Prompt**: `A man walks into an office and sits at his desk`
        - Add other metadata as required. *(All entries are optional except `shot_name` which must be provided though duplicates are accepted. Default entries will be created if not imported from CSV. The shot name does not need to be unique, but it is recommended to make it so.)*

3. **Save the Shot**:

    - Click **Save** to add the shot to your project
    - The shot will appear in the shots table and will create empty media placeholders in both "Image" and "Video" storyboard pages.

### Step 4: Add Media (Takes) to Your Shot

Media is added to shots by creating empty placeholder "Takes" then replacing them with valid media. There are three places this can be done manually *(placeholders are created automatically when importing from CSV)*: 

1. From the Shots Page with "Add Takes" button *(will create empty placeholder takes in both Image and Video storyboards for that shot)*.

2. From within the shot popup modals of the "Image" or "Video" Storyboard pages *(creates empty placeholder takes only in the storyboard you action it from)*.

#### Adding "Takes" In Just The Image Storyboard

1. **Navigate to Images Storyboard Page**:

    - Click the **Images** tab or press `Ctrl+2`

2. **Add Image Take(s)**:

    - Select your shot from the gallery
    - Click "View Media" button.
    - Click **Add Take** button from the popup modal *(found on the last take of that shot)*.
    - Choose the number of takes you wish to add *(empty placeholders will be created only in the "Images" storyboard)*
    - Select **Replace** button in the popup modal for an empty take
    - Browse and select your valid image file *(workflow metadata png is recommended)*
    - Click **Add** 

3. **View Your Image**:

    - The image will appear in the gallery
    - Double-click to view it full-size in the floating viewer
    - Click the star icon to mark it as your favorite *(selectable in the popup modal for the shot)*
    - If the image contains workflow metadata, that can be viewed or downloaded from the button on the preview card.

**Note**: Imported media will not retain their file names on import, but will be renamed and added to the `\media\{shot_id}\` folder using `base_image_xx.png` for images. A json file `/project_Your_Project/data/shot_name_mapping.json` maintains a record of the relationship between `shot_name` and the `\media\{shot_id}\` folder for migration out if required.

#### Adding "Takes" In Just The Video Storyboard

1. **Navigate to Videos Storyboard Page**:

    - Click the **Videos** tab or press `Ctrl+3`

2. **Add Video Take**:

    - Select your shot from the gallery
    - Click "View Media" button.
    - Click **Add Take** button from the popup modal *(found on the last take of that shot)*.
    - Choose the number of takes you wish to add *(empty placeholders will be created only in the "Video" storyboard)*
    - Select **Replace** button in the popup modal for an empty take
    - Browse and select your video file and then browse and select your thumbnail image for the video *(workflow metadata png file is recommended)*
    - Click **Add**

3. **View Your Video**:

    - The video will appear in the gallery
    - Click to play it in the floating video player
    - Click the star icon to mark your favorite take *(selected from within the popup modal)*
    - If the associated video image contains workflow metadata, that can be viewed or downloaded from the button on the shot preview card.

**Note**: Imported media will not retain their file names on import, but will be renamed and added to the `\media\{shot_id}\` folder. For the video storyboard, two files are required per take during replacement: `final_video_xx.mp4` and `video_workflow_xx.png`. It is recommended to use the accompanying workflow metadata png file for the video, but any image can serve as preview image thumbnail. An image must be provided with the video at upload.

A json file `/project_Your_Project/data/shot_name_mapping.json` maintains a record of the relationship between `shot_name` and the `\media\{shot_id}\` folder for migration out if required.

### Step 5: Explore Your Project

1. **View All Modules**:

    - Navigate through each tab to see your content
    - Notice how your shot appears in all relevant modules

2. **Use Keyboard Shortcuts**:

    - Practice using `Ctrl+1` through `Ctrl+8` to switch tabs
    - A list of keyboard shortcuts are provided from the "Project" menu dropdown

3. **Search and Filter**:

    - Use the search box in the Shots page to find your shot. This works in combination with the "Column Picker" to help refine your search.
    - Type in the letters and the database list of shots will be reduced to those choices *(based on selected columns in the "Column Picker")*
    - Alternatively, try filtering by section *(bottom menu bar)* to reduce your view. Section filtering is retained as you navigate between the "Shot", "Image", and "Video" pages. 
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

1. **Plan**: Create shots with descriptions and prompts within AIMMS, or import from CSV.
2. **Generate**: Use your AI tools to create images/videos based on prompts
3. **Import**: Add generated media to AIMMS
4. **Review**: View and organize your media
5. **Iterate**: Add, Delete, or Replace takes as needed
6. **Organise**: Re-order, manage, or change your shot plan
7. **Export**: Export your storyboard for backup or sharing

## Tips for Success

### Shot Naming Conventions:

- Use descriptive shot names: `INT_OFFICE_DAY_001` or `HWM_01A_01A_first_scene`
- If managing shots is new to you trial this approach: `HWM_01A_01A_first_scene` which breaksdown as: *`{Project name}_{Scene number}_{Shot number of scene}_{short_descriptor}`*
- It's recommended to keep your shot name management consistent and unique across your project, but it is not enforced in the column entry. This allows for maximum flexibility across different methodologies


### Organization:

- Use sections to group related shots: `Act 1`, `1. Opening Scene`, `Climax`. *(You may find numbering these helps for sorting later. You can change them at any time and change multiple rows to unified section names by selecting groups of rows for multi-editing)*.
- Star your favorite takes for easy identification *(found in the shot popup modal of the Image and Video Storyboard pages)*
- Regularly clean up unused media placeholder files *(Unused page module)* that accumulate when adding multiple takes and shots.

A json file `/project_Your_Project/data/shot_name_mapping.json` maintains a record of the relationship between `shot_name` and the `\media\{shot_id}\` folder for migration out if required. A copy of this file is automatically backed up to the `\backup` folder and cycled on a 30-day retention policy.

### Workflow Efficiency (Tips & Tricks):

- Prefix the name of your project with something instantly recognisable as an AIMMS project. For example, `project_Some-Project`. A prefix will make it easy to search later across drives.

- Create a csv of multiple shots with metadata, then import via the Shots page. *(You can import a csv at any time. Importing a csv will accept duplicated names or empty column entries (only a `shot_name` must be present, along with relevant column headings)*. A `shot_id` is automatically created by the system for each shot to manage its unique identity in the database.

- For an example csv, create a dummy entry in a new AIMMS project using "Add Shot" button to automatically populate the columns, then export the csv out *(from the "File" menu drop down)*. Exported csv files can be found in the `project_YourProject\data\csv` folder.

- You can change the order of shots from within the Shots page by double-clicking on a shot and changing the `order_number`. This will change its placement order in the Shot, Images, and Videos pages.

- To export only your starred media out for editing in external software, e.g., Davinci Resolve to make a final cut or edited sequences from multiple video clips, use *"Export Starred Takes"* from the *"File"* dropdown menu. A simple python script can then be used to copy the media and rename it using `shot_name` column, for quick import to the video editing software of your choice. *(EDL and XML export methods were trialled, but found to be inconsistent between different video editing systems)*.

- Use keyboard shortcuts for faster navigation.

- Regularly save *(.aimms routing info)*, and backup the database *(found in the "File" dropdown menu)*.

- After large media changes, archive the entire project to a zip file for storage *(found in the "File" dropdown menu)*.

- Regularly backup acrhived projects to offline storage for safe-keeping.

- If you lose control of a large media project, look at the [AIMMS migration software](https://github.com/mdkberry/migrating-to-aimms) as a way to restructure a project. With it you can import a csv of metadata, use the last saved `.aimms` file or `shot_name_mapping.json` to re-construct a project, or migrate disorganised media files into a valid AIMMS project format.

- The backup options provided under the "File" menu will help in restoring projects if required.

***IMPORTANT NOTE:*** *Databases failures are rare, but we can not be held responsible for loss of data when using this software. Every precaution has been taken to provide ways to re-establish integrity of a corrupted project. Multiple backup features are provided from the "File" dropdown menu to help in the case of failed project integrity. We highly recommend you save, backup, and archive regularly for peace of mind.*

## Next Steps

### Explore Advanced Features:

- **Import Existing Data**: Use CSV import to bring in existing shot lists
- **Customize Settings**: Adjust themes and preferences to your liking
- **Learn Advanced Modules**: Explore Assets, Unused, Logs, and Routing pages.

### Practice with Examples:

- Create a simple 3-shot scene
- Practice adding different types of media
- Experiment with the starred system
- Try the search and filtering features
- Try the popup viewing modals in Image, Videos, and Assets pages.

### Learn Best Practices:

- Watch [the video tutorials](https://www.youtube.com/playlist?list=PLVCJTJhkunkRutnutiP9dgd6crw8MWEHN) for the most up to date information and methods in practice
- Join the [Patreon (free tier)](https://www.patreon.com/c/AIMakingMovies) for latest information and news

## Troubleshooting Common Issues

### Shot Not Appearing:

- Check that you saved the shot successfully
- Verify you're viewing "All Sections" in the filter
- Try refreshing the view with `F5`
- If that fails change between the pages
- As a last resort restart the application.

**NOTE**: If a take or shot is still not showing up, then run the "Analyze Zeroed-Out Takes" button in Unused page. It might be there was a failure to connect the media to the database. If your shot is listed as orphaned or has an error, delete it, restart the application and then try again. If the problem continues, check permissions on folders or locked files. For bugs or strange results post to the [github issues](https://github.com/AI-Making-Movies/aimms-docs/issues) page

### Media Not Loading:

- Ensure files are in supported formats (PNG, JPG, MP4, etc.)
- Check file paths are accessible
- Verify file sizes aren't so large that they impact load times

**NOTE**: AIMMS has been tested with a 600 shot project containing 21,000 takes with a total size of 23GB in media files. A short delay can occur when managing the navigation between pages for larger projects *(50 entries per page require caching)*. If individual video clips are large in file size *(which can happen for edited sequences)* then you will need to account for that in use of the software load times.

### Application Performance:

AIMMS has been made with low processing overhead in mind and has a robust caching system. However, AIMMS does not need to use a GPU and has been tested running on  low ram devices. It uses `ffmpeg` and `ffprobe` for video previewing *(bundled with Windows version of AIMMS application, but will need to be provided with other platforms)*.

If you have problems, ensure sufficient disk space is available and that system ram is not full during use. AIMMS will generally use between 500mb and 1GB in application ram with a large project. 

For low ram devices and older machines you may need to close other software for best performace. For example, multiple browser tabs left open can consume large amounts of ram.

AIMMS projects are best stored on SSD drives for speed of media loading. This could be on local, network, or external drives. If you are storing projects on SATA or slow USB external drives, this will impact speed of performance. While the AIMMS application itself does not need to run on SSD drive, it will likely perform better if it does.

## Getting Help

### Built-in Help:

- **Documentation**: Press `F1` or go to Help → Documentation (Online resource)

### Online Resources:

- [**Official Website**](https://markdkberry.com/software/): Visit for latest downloads and news
- [**Documentation**](https://ai-making-movies.github.io/aimms-docs/): Comprehensive user guides
- [**Video Tutorials**](https://www.youtube.com/@markdkberry): Step-by-step video guides
- **Community Forum**: At this time [Patreon (Free Tier)](https://www.patreon.com/c/AIMakingMovies) provides the best option for discussion on use.

### Support:

- **Logs**: Check the Logs page module for error information
- **Export Data**: Use export features to help track health of project data
- [**Github Issues**](https://github.com/AI-Making-Movies/aimms-docs/issues): For reporting bugs and issues

Congratulations! You've successfully created your first AIMMS project and learned the basics. Continue exploring the application and refer to the detailed user guides as you become more familiar with the features.