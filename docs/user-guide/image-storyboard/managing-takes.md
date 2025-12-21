# Managing Image Takes

## Overview

Managing image takes in AIMMS allows you to organize multiple versions of images for each shot, track improvements, and maintain quality control. This guide covers adding, replacing, deleting, and organizing image takes effectively.

## Understanding Image Takes

### What Are Image Takes?

Image takes represent different versions or iterations of the base image for a shot. Each shot can have multiple takes, allowing you to:

- **Track Progress**: See the evolution of your image creation
- **Compare Versions**: Evaluate different approaches or quality levels
- **Maintain Options**: Keep multiple versions for flexibility
- **Quality Control**: Select the best version for your project

### Take Numbering System

**Automatic Numbering**
- AIMMS automatically assigns take numbers (base_01, base_02, base_03, etc.)
- Sequential numbering helps track the order of creation
- Consistent naming prevents conflicts and confusion

**Take Identification**
- Each take has a unique identifier (UUID-based)
- Take numbers are displayed in the gallery
- Metadata includes creation date and other details

## Adding New Image Takes

### Method 1: Using Add Take Button

1. **Select Shot**
   - Navigate to the Image Storyboard module
   - Find the shot you want to add an image to

2. **Add New Take**
   - Click the **Add Take** button
   - A file browser dialog will appear

3. **Choose Image File**
   - Browse to your image file location
   - Select the image file
   - Supported formats: PNG, JPG, JPEG, WebP

4. **Configure Take**
   - AIMMS will suggest a take number
   - Review the take settings
   - Click **Add** to create the new take

5. **Verify Addition**
   - The new take appears in the gallery
   - Check that the image displays correctly
   - Verify take number and metadata

### Method 2: Drag and Drop

1. **Prepare Files**
   - Have your image files ready
   - Ensure they're in supported formats

2. **Drag to Gallery**
   - Drag image files directly onto the image gallery
   - AIMMS will automatically import them
   - Files are organized by shot automatically

3. **Add Metadata**
   - After import, add any necessary metadata
   - Review take numbering and organization
   - Star favorites if applicable

### Method 3: Bulk Import

1. **Prepare Multiple Files**
   - Organize multiple image files
   - Ensure they're for the correct shots

2. **Bulk Addition**
   - Use Add Take for multiple files
   - Or drag multiple files at once
   - AIMMS handles batch processing

3. **Review Results**
   - Check that all files were imported correctly
   - Verify take numbering and organization
   - Update metadata as needed

## Replacing Image Takes

### When to Replace Takes

**Quality Improvement**
- You've created a better version of an image
- The new image has higher resolution or better quality
- You want to update the visual style or content

**Error Correction**
- Fixing mistakes in the original image
- Correcting color, composition, or content issues
- Updating based on feedback or requirements

**Version Updates**
- Updating images based on project changes
- Incorporating new information or requirements
- Refreshing older images with current techniques

### Replacement Process

1. **Select Image to Replace**
   - Right-click the image take you want to replace
   - Or select the image and choose replace option

2. **Choose New Image**
   - Browse to your new image file
   - Select the replacement image
   - Ensure it's in a supported format

3. **Confirm Replacement**
   - AIMMS will show a confirmation dialog
   - Review what will be replaced
   - Confirm the replacement

4. **Verify Changes**
   - Check that the new image appears correctly
   - Verify that metadata is preserved
   - Ensure take numbering remains consistent

### What Happens During Replacement

**File Management**
- Old image file is backed up automatically
- New image replaces the old one in the file system
- Take metadata is preserved

**Database Updates**
- Database records are updated with new file information
- Take relationships are maintained
- Star status and other metadata is preserved

**Backup System**
- Old image is saved in backup location
- Can be recovered if replacement was accidental
- Maintains project history

## Deleting Image Takes

### When to Delete Takes

**Quality Control**
- Remove low-quality or unusable images
- Clean up test or experimental takes
- Maintain only the best versions

**Project Organization**
- Remove duplicates or similar images
- Clean up outdated versions
- Optimize project size and performance

**Workflow Management**
- Remove takes that are no longer relevant
- Clean up after major revisions
- Maintain focused image collections

### Deletion Process

1. **Select Take to Delete**
   - Right-click the image take you want to delete
   - Or select the image and choose delete option

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
- Consider backing up before deletion
- Use export features to save important takes
- Document reasons for deletion

## Take Organization

### Starred Image System

**Marking Favorites**
- Click the star icon on any image thumbnail
- Only one image per shot can be starred at a time
- Starred images are highlighted for easy identification

**Benefits of Starring**
- **Quick Identification**: Easily find your best takes
- **Export Priority**: Starred images used for exports
- **Workflow Focus**: Focus improvement on non-starred images
- **Quality Control**: Clear visual hierarchy of image quality

**Managing Stars**
- **Change Stars**: Click a different image's star to move the favorite
- **Remove Stars**: Click the star again to unstar (none will be starred)
- **View Only Stars**: Use filter to show only starred images

### Take Comparison

**Side-by-Side Comparison**
- Use the floating image viewer to compare takes
- View multiple takes simultaneously
- Evaluate differences in quality, composition, or content

**Quality Assessment**
- Compare technical quality (resolution, clarity)
- Evaluate artistic quality (composition, style)
- Assess suitability for project requirements

**Decision Making**
- Use comparison to decide which take to star
- Identify areas for improvement in non-starred takes
- Make informed decisions about image selection

### Take Metadata Management

**Adding Metadata**
- Click any image to view details
   - Add descriptions, notes, or ratings
   - Update creation dates or other information
   - Document the purpose or context of each take

**Metadata Categories**
- **Technical Information**: Resolution, file size, format
- **Quality Assessment**: Ratings, notes, improvement areas
- **Workflow Status**: Current status in your workflow
- **Relationships**: Links to related takes or assets

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
- Use backup features for critical images
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

**Deletion Issues**
- Verify you have proper permissions
- Check if take is locked or in use
- Ensure database isn't corrupted
- Try restarting AIMMS

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

Effective take management helps you maintain organized, high-quality image collections and track improvements throughout your project workflow.