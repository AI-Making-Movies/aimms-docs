# Video Storyboard Overview

## Introduction

The Video Storyboard module is where you view and manage all the final videos for your shots. This gallery-style interface displays video thumbnails with playback capabilities, making it easy to review, organize, and manage your video assets.

## Understanding the Video Gallery

The video storyboard displays all final videos for your shots in a grid layout. Each thumbnail represents a "take" - a version of the final video for that shot.

### Gallery Layout

- **Grid View**: Videos displayed in rows and columns
- **Shot Organization**: Videos grouped by shot (you can filter by section)
- **Thumbnail Quality**: Optimized video thumbnails for fast loading
- **Metadata Display**: Key information shown on hover or in details

### Video Take Information

Each video take shows:
- **Shot Name**: Which shot this video belongs to
- **Take Number**: Version number (e.g., video_01, video_02)
- **Video Format**: Format and quality indicators
- **Duration**: Video length
- **Star Status**: Whether this take is starred/favorite
- **Workflow Status**: Whether workflow PNG file exists

## Key Features

### Video Playback and Management

**Thumbnail Gallery**
- Browse all videos in a visual grid layout
- Quick overview of all final videos in your project
- Efficient navigation through large video collections

**Video Playback**
- Click any video thumbnail to play it in the floating player
- Full video playback with controls
- Support for multiple video formats

**Video Organization**
- Videos automatically organized by shot
- Section filtering to focus on specific parts of your project
- Search functionality to find specific videos quickly

### Take Management

**Multiple Takes per Shot**
- Each shot can have multiple video takes
- Different versions or iterations of the same shot
- Easy comparison between different takes

**Take Numbering System**
- Automatic take numbering (video_01, video_02, etc.)
- Clear identification of video versions
- Logical organization of multiple takes

**Take Operations**
- Add new video takes
- Replace existing takes with new videos
- Delete takes that are no longer needed
- View take history and metadata

### Starred Video System

**Favorite Management**
- Mark your favorite video take for each shot
- Only one video per shot can be starred at a time
- Starred videos are highlighted for easy identification

**Workflow Benefits**
- Quickly identify your best takes
- Use starred videos for exports and presentations
- Focus improvement efforts on non-starred videos
- Clear visual hierarchy of video quality

## Video Operations

### Adding New Videos

**Direct Addition**
- Click **Add Take** for any shot
- Browse and select your video file
- Choose take number and settings
- Video is automatically organized in the correct shot folder

**Supported Formats**
- **MP4**: Recommended for maximum compatibility
- **WebM**: Modern format with good compression
- **MKV**: Container format, flexible
- **GIF**: Animated images, limited quality
- **Maximum Size**: 500MB per file

### Video Replacement

**Replace Existing Videos**
- Right-click any video and select **Replace Video**
- Choose your new video file
- AIMMS validates the new video file
- Old video is backed up automatically

**Quality Improvement**
- Replace lower quality videos with better versions
- Maintain consistent naming and organization
- Track improvements through take numbering

### Video Deletion

**Safe Deletion**
- Right-click video and select **Delete Take**
- Confirmation dialog prevents accidental deletion
- Only removes the take, not the entire shot
- Original shot remains intact

## Video Metadata and Information

### Video Details

**Technical Information**
- **Duration**: Video length (HH:MM:SS)
- **Resolution**: Width x height in pixels
- **Frame Rate**: FPS (frames per second)
- **Codec**: Video compression format
- **File Size**: Storage space used by the video
- **Aspect Ratio**: Display proportions

**Workflow Information**
- **Workflow PNG**: Status of workflow file
- **Take Type**: Final video, mask video, etc.
- **Creation Date**: When the take was added
- **File Path**: Location in project structure

### Metadata Display

**Hover Information**
- Hover over thumbnails for quick metadata
- See key information without opening details
- Fast overview of video properties

**Detailed View**
- Click video to view comprehensive metadata
- Full technical specifications
- Shot information and relationships

## Workflow PNG System

### What Are Workflow PNG Files?

Workflow PNG files are companion images that store workflow and prompt information for videos. They're automatically created and managed by AIMMS.

### Why Workflow PNG Files Matter

**Prompt Storage**
- Contains the AI prompt used to generate the video
- Stores workflow configuration
- Additional metadata storage
- Links video to generation workflow

### Workflow PNG Management

**Automatic Creation**
- AIMMS creates PNG files when videos are added
- Automatically updated when videos are replaced
- Validation checks for missing or corrupted PNG files
- Can regenerate PNG files from video metadata

**Status Indicators**
- **✅ Present**: Workflow PNG file exists and is valid
- **⚠️ Missing**: PNG file is missing (can be regenerated)
- **❌ Invalid**: PNG file exists but is corrupted

## Floating Video Player

### Player Features

**Playback Controls**
- **Play/Pause**: Spacebar or play button
- **Seek**: Click on progress bar or use arrow keys
- **Volume**: Mouse wheel or volume slider
- **Fullscreen**: F11 or fullscreen button

**Navigation**
- **Frame Navigation**: Arrow keys for frame-by-frame
- **Previous/Next**: Navigate between takes for the same shot
- **Shot Navigation**: Jump to different shots

**Information Display**
- **Metadata**: Display video technical information
- **Workflow Data**: Show workflow and prompt information
- **Status Indicators**: Show video status and quality

### Player Controls

| Control | Function | Keyboard Shortcut |
|---------|----------|-------------------|
| ▶️ | Play/Pause | Spacebar |
| ⏹️ | Stop | Esc |
| ⏭️ | Next frame | Right Arrow |
| ⏮️ | Previous frame | Left Arrow |
| 🔊 | Volume control | Mouse wheel |
| 🖼️ | Toggle fullscreen | F11 |
| 📊 | Show/hide metadata | I |
| ✕ | Close player | Esc |

## Integration with Other Modules

### Cross-Module Navigation

**Shots Module Integration**
- Direct links from shots to their videos
- Quick navigation between shot details and videos
- Consistent organization across modules

**Image Storyboard Connection**
- Videos often correspond to base images
- Use starred images as reference for video generation
- Cross-module navigation for related media

**Assets Management**
- Videos can be linked to project assets
- Reference videos support shot creation
- Consistent file organization across modules

### Workflow Integration

**Shot Workflow**
- Videos are part of the shot completion workflow
- Final videos represent completed shots
- Metadata flows between modules

**Quality Control**
- Starred videos indicate preferred versions
- Easy comparison between takes
- Clear progression of video quality

## Performance and Optimization

### Loading and Display

**Thumbnail Generation**
- AIMMS creates optimized video thumbnails automatically
- Fast gallery loading for large video collections
- Efficient memory usage

**Video Playback**
- Optimized video playback for various formats
- Smooth playback with hardware acceleration
- Memory management for large video files

**Caching System**
- Recently viewed videos load faster
- Intelligent cache management
- Performance optimization for frequently accessed videos

### File Management

**Automatic Organization**
- Videos automatically placed in correct shot folders
- Take numbering system prevents conflicts
- UUID-based take identification

**Backup and Recovery**
- Automatic backup of video relationships
- Recovery options for deleted takes
- Database integrity for video management

## Best Practices

### Video Organization

**Consistent Naming**
- Let AIMMS handle take numbering automatically
- Use descriptive shot names for organization
- Maintain consistent file formats

**Quality Management**
- Use MP4 format for maximum compatibility
- Keep file sizes reasonable for performance
- Regularly review and update video takes

**Workflow Efficiency**
- Star your favorite takes for easy identification
- Use search and filtering for large projects
- Maintain organized shot structure

### Professional Workflow

**Version Control**
- Use take numbering to track video versions
- Replace takes rather than creating duplicates
- Maintain clear progression of quality improvements

**Quality Standards**
- Set quality standards for your project
- Use starred system to maintain quality control
- Regular review of video takes

The Video Storyboard module provides a comprehensive solution for managing your project's video assets. Mastering this module ensures efficient organization and quality control of your final video outputs.