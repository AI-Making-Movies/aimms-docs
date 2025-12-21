# Managing Video Takes

## Overview

Managing video takes in AIMMS allows you to organize multiple versions of videos for each shot, track improvements, and maintain quality control. This guide covers adding, replacing, deleting, and organizing video takes effectively.

## Understanding Video Takes

### What Are Video Takes?

Video takes represent different versions or iterations of the final video for a shot. Each shot can have multiple takes, allowing you to:

- **Track Progress**: See the evolution of your video creation
- **Compare Versions**: Evaluate different approaches or quality levels
- **Maintain Options**: Keep multiple versions for flexibility
- **Quality Control**: Select the best version for your project

### Take Numbering System

**Automatic Numbering**
- AIMMS automatically assigns take numbers (video_01, video_02, video_03, etc.)
- Sequential numbering helps track the order of creation
- Consistent naming prevents conflicts and confusion

**Take Identification**
- Each take has a unique identifier (UUID-based)
- Take numbers are displayed in the gallery
- Metadata includes creation date and other details

### Workflow PNG Files

**Companion Images**
- Each video take has an associated workflow PNG file
- Stores AI prompts and workflow information
- Links video to its generation process
- Essential for workflow tracking and recovery

**PNG File Management**
- Automatically created when videos are added
- Updated when videos are replaced
- Can be regenerated if missing or corrupted
- Critical for maintaining workflow integrity

## Adding New Video Takes

### Method 1: Using Add Take Button

1. **Select Shot**
   - Navigate to the Video Storyboard module
   - Find the shot you want to add a video to

2. **Add New Take**
   - Click the **Add Take** button
   - A file browser dialog will appear

3. **Choose Video File**
   - Browse to your video file location
   - Select the video file
   - Supported formats: MP4, WebM, MKV, GIF

4. **Configure Take**
   - AIMMS will suggest a take number
   - Review the take settings
   - Click **Add** to create the new take

5. **Verify Addition**
   - The new take appears in the gallery
   - Check that the video displays correctly
   - Verify take number and metadata
   - Confirm workflow PNG file was created

### Method 2: Drag and Drop

1. **Prepare Files**
   - Have your video files ready
   - Ensure they're in supported formats

2. **Drag to Gallery**
   - Drag video files directly onto the video gallery
   - AIMMS will automatically import them
   - Files are organized by shot automatically

3. **Add Metadata**
   - After import, add any necessary metadata
   - Review take numbering and organization
   - Star favorites if applicable

### Method 3: Bulk Import

1. **Prepare Multiple Files**
   - Organize multiple video files
   - Ensure they're for the correct shots

2. **Bulk Addition**
   - Use Add Take for multiple files
   - Or drag multiple files at once
   - AIMMS handles batch processing

3. **Review Results**
   - Check that all files were imported correctly
   - Verify take numbering and organization
   - Update metadata as needed

## Replacing Video Takes

### When to Replace Takes

**Quality Improvement**
- You've created a better version of a video
- The new video has higher resolution or better quality
- Improved compression or file size

**Content Updates**
- Changes to video content or composition
- Updated visual effects or animations
- Corrections to errors or inconsistencies

**Technical Improvements**
- Better codec or compression settings
- Improved frame rate or resolution
- Enhanced color grading or effects

### Replacement Process

1. **Select Video to Replace**
   - Right-click the video take you want to replace
   - Or select the video and choose replace option

2. **Choose New Video**
   - Browse to your new video file
   - Select the replacement video
   - Ensure it's in a supported format

3. **Confirm Replacement**
   - AIMMS will show a confirmation dialog
   - Review what will be replaced
   - Confirm the replacement

4. **Verify Changes**
   - Check that the new video appears correctly
   - Verify that metadata is preserved
   - Ensure take numbering remains consistent
   - Confirm workflow PNG file was updated

### What Happens During Replacement

**File Management**
- Old video file is backed up automatically
- New video replaces the old one in the file system
- Workflow PNG file is updated with new information

**Database Updates**
- Database records are updated with new file information
- Take relationships are maintained
- Star status and other metadata is preserved

**Workflow Integration**
- Workflow PNG file is regenerated if needed
- Video metadata is extracted and updated
- Take history is maintained

## Deleting Video Takes

### When to Delete Takes

**Quality Control**
- Remove low-quality or unusable videos
- Clean up test or experimental takes
- Maintain only the best versions

**Project Organization**
- Remove duplicates or similar videos
- Clean up outdated versions
- Optimize project size and performance

**Workflow Management**
- Remove takes that are no longer relevant
- Clean up after major revisions
- Maintain focused video collections

### Deletion Process

1. **Select Take to Delete**
   - Right-click the video take you want to delete
   - Or select the video and choose delete option

2. **Confirm Deletion**
   - A confirmation dialog will appear
   - Read the warning carefully
   - Confirm that you want to delete the take

3. **Verify Deletion**
   - The take disappears from the gallery
   - Check that the correct take was removed
   - Ensure the shot still has other takes if needed

### Safety Features

**Confirmation Required**
- Always requires confirmation before deletion
- Clear warning about permanent removal
- Option to cancel the deletion

**Selective Deletion**
- Only removes the selected take
- Does not affect the shot or other takes
- Maintains project integrity

**Backup Options**
- Consider backing up important takes
- Use export features to save important videos
- Document reasons for deletion

## Take Organization

### Starred Video System

**Marking Favorites**
- Click the star icon on any video thumbnail
- Only one video per shot can be starred at a time
- Starred videos are highlighted for easy identification

**Benefits of Starring**
- **Quick Identification**: Easily find your best takes
- **Export Priority**: Starred videos used for exports
- **Workflow Focus**: Focus improvement on non-starred videos
- **Quality Control**: Clear visual hierarchy of video quality

**Managing Stars**
- **Change Stars**: Click a different video's star to move the favorite
- **Remove Stars**: Click the star again to unstar (none will be starred)
- **View Only Stars**: Use filter to show only starred videos

### Take Comparison

**Side-by-Side Comparison**
- Use the floating video player to compare takes
- View multiple takes simultaneously
- Evaluate differences in quality, content, or effects

**Quality Assessment**
- Compare technical quality (resolution, frame rate)
- Evaluate artistic quality (composition, effects)
- Assess suitability for project requirements

**Decision Making**
- Use comparison to decide which take to star
- Identify areas for improvement in non-starred takes
- Make informed decisions about video selection

### Take Metadata Management

**Adding Metadata**
- Click any video to view details
   - Add descriptions, notes, or ratings
   - Update creation dates or other information
   - Document the purpose or context of each take

**Metadata Categories**
- **Technical Information**: Resolution, file size, format, duration
- **Quality Assessment**: Ratings, notes, improvement areas
- **Workflow Status**: Current status in your workflow
- **Relationships**: Links to related takes or assets

## Workflow PNG File Management

### Understanding Workflow PNG Files

**Purpose and Content**
- Stores AI prompts used to generate the video
- Contains workflow configuration information
- Provides additional metadata storage
- Links video to its generation workflow

**File Status Indicators**
- **✅ Present**: Workflow PNG file exists and is valid
- **⚠️ Missing**: PNG file is missing (can be regenerated)
- **❌ Invalid**: PNG file exists but is corrupted

### PNG File Operations

**Automatic Management**
- AIMMS creates PNG files automatically
- Files are updated when videos are replaced
- Validation checks for missing or corrupted files

**Manual Operations**
- **Regenerate PNG**: Create PNG file from video metadata
- **Validate PNG**: Check PNG file integrity
- **Repair PNG**: Fix corrupted PNG files

**Recovery Options**
- Regenerate missing PNG files
- Restore PNG files from backup
- Manual PNG file creation if needed

## Best Practices for Take Management

### Organization Strategies

**Consistent Naming**
- Let AIMMS handle take numbering automatically
- Use descriptive shot names for organization
- Maintain consistent file formats

**Quality Control**
- Regularly review and update takes
- Star your best versions clearly
- Remove low-quality takes to maintain focus

**Workflow Integration**
- Use takes to track progress and improvements
- Maintain clear progression of quality
- Document changes and improvements

### Efficiency Tips

**Batch Operations**
- Add multiple takes at once when possible
- Use drag and drop for quick additions
- Organize takes by quality or version

**Search and Filter**
- Use search to find specific takes quickly
- Filter by section or other criteria
- Use starred system for quick access

**Backup and Recovery**
- Regularly export important takes
- Use backup features for critical videos
- Document take history and changes

## Troubleshooting Take Management

### Common Issues

**Take Not Appearing**
- Check file format is supported
- Verify file wasn't corrupted during import
- Ensure file size isn't too large
- Try refreshing the gallery (F5)

**Replacement Problems**
- Check that replacement file is accessible
- Verify file format compatibility
- Ensure sufficient disk space
- Check file permissions

**PNG File Issues**
- Use regenerate option for missing PNG files
- Check file permissions for PNG creation
- Verify video file integrity
- Contact support if PNG issues persist

### Error Resolution

**File System Errors**
- Check file permissions and access
- Verify sufficient disk space
- Ensure files aren't locked by other applications
- Check for file system corruption

**Database Issues**
- Run database validation tools
- Check for database corruption
- Verify database permissions
- Contact support if database issues persist

Effective take management helps you maintain organized, high-quality video collections and track improvements throughout your project workflow.