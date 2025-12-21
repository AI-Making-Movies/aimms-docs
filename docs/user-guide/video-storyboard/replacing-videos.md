# Replacing Videos

## Overview

Replacing videos in AIMMS allows you to update existing video takes with new or improved versions while preserving all metadata and relationships. This guide covers the replacement process, workflow PNG file management, and best practices for maintaining project integrity.

## When to Replace Videos

### Quality Improvement

**Better Resolution**
- You've created a higher resolution version
- Improved clarity or detail in the video
- Enhanced visual quality or sharpness

**Content Updates**
- Changes to video content or composition
- Updated visual effects or animations
- Corrections to errors or inconsistencies

**Technical Improvements**
- Better codec or compression settings
- Improved frame rate or resolution
- Enhanced color grading or effects

### Error Correction

**Fixing Mistakes**
- Correcting composition errors
- Fixing color or exposure issues
- Removing unwanted elements or artifacts

**Client Feedback**
- Incorporating requested changes
- Addressing quality concerns
- Meeting specific requirements or standards

### Project Evolution

**Style Updates**
- Updating visual style to match project evolution
- Consistency improvements across shots
- Brand or aesthetic updates

**Workflow Changes**
- Changes in AI generation parameters
- Updated prompts or techniques
- Process improvements

## Replacement Process

### Method 1: Right-Click Context Menu

1. **Select Video to Replace**
   - Right-click the video take you want to replace
   - A context menu will appear

2. **Choose Replace Option**
   - Select **Replace Video** from the context menu
   - A file browser dialog will open

3. **Choose New Video**
   - Browse to your new video file location
   - Select the replacement video file
   - Ensure it's in a supported format (MP4, WebM, MKV, GIF)

4. **Confirm Replacement**
   - AIMMS will show a confirmation dialog
   - Review what will be replaced
   - Confirm the replacement

5. **Verify Changes**
   - Check that the new video appears correctly
   - Verify that metadata is preserved
   - Ensure take numbering remains consistent
   - Confirm workflow PNG file was updated

### Method 2: Using Video Details

1. **Open Video Details**
   - Click the video thumbnail to view details
   - The video details panel will appear

2. **Access Replace Option**
   - Click the **Replace Video** button in the details panel
   - A file browser dialog will open

3. **Select New Video**
   - Choose your replacement video file
   - Ensure it meets project requirements

4. **Complete Replacement**
   - Confirm the replacement
   - Verify the new video appears correctly

### Method 3: Drag and Drop Replacement

1. **Prepare Replacement**
   - Have your new video file ready
   - Ensure it's the correct replacement

2. **Drag to Target**
   - Drag the new video file onto the existing video thumbnail
   - AIMMS will prompt for replacement confirmation

3. **Confirm Action**
   - Confirm that you want to replace the video
   - Verify the replacement was successful

## Workflow PNG File Management

### What Are Workflow PNG Files?

Workflow PNG files are companion images that store workflow and prompt information for videos. They're automatically created and managed by AIMMS.

### Why Workflow PNG Files Matter

**Prompt Storage**
- Contains the AI prompt used to generate the video
- Stores workflow configuration
- Additional metadata storage
- Links video to generation workflow

### PNG File Handling During Replacement

**Automatic Updates**
- AIMMS automatically updates the workflow PNG file
- New video prompts are extracted and stored
- Workflow configuration is preserved
- Metadata is synchronized with the new video

**Validation and Repair**
- System checks for PNG file integrity
- Missing or corrupted PNG files are detected
- Automatic regeneration if needed
- Manual repair options available

**PNG File Status**
- **✅ Present**: Workflow PNG file exists and is valid
- **⚠️ Missing**: PNG file is missing (can be regenerated)
- **❌ Invalid**: PNG file exists but is corrupted

## What Happens During Replacement

### File Management

**Backup Creation**
- AIMMS automatically backs up the old video
- Backup is stored in a safe location
- Original video can be recovered if needed

**File Replacement**
- New video replaces the old file in the file system
- File path and naming remain consistent
- Take numbering is preserved

**PNG File Updates**
- Workflow PNG file is updated with new information
- Video metadata is extracted and stored
- Workflow relationships are maintained

### Database Updates

**Record Updates**
- Database records are updated with new file information
- File paths are updated to point to new video
- Metadata relationships are maintained

**Relationship Preservation**
- Links to shots remain intact
- Connections to other media are preserved
- Project structure remains consistent

**History Tracking**
- Replacement is logged in the database
- Original video information is preserved
- Change history is maintained

## Best Practices for Video Replacement

### Preparation

**File Verification**
- Ensure replacement video is in supported format
- Verify video quality and resolution
- Check file size and compatibility
- Confirm workflow PNG file can be created

**Backup Strategy**
- Always backup important videos before replacement
- Use export features to save current versions
- Document reasons for replacement

**Quality Assessment**
- Compare new video to original
- Ensure improvements are significant
- Verify the replacement meets project standards

### Replacement Strategy

**Selective Replacement**
- Replace only when improvements are significant
- Avoid unnecessary replacements that clutter history
- Focus on quality and necessity

**Consistent Naming**
- Let AIMMS handle file naming automatically
- Maintain consistent take numbering
- Avoid manual file system changes

**PNG File Management**
- Ensure workflow PNG files are properly updated
- Check PNG file status after replacement
- Regenerate PNG files if needed

### Quality Control

**Before Replacement**
- Review the new video thoroughly
- Compare with the original
- Ensure it meets all requirements
- Verify workflow PNG file can be created

**After Replacement**
- Verify the new video displays correctly
- Check that all metadata is preserved
- Test that the video plays properly
- Confirm workflow PNG file was updated

**Documentation**
- Document the reason for replacement
- Note any changes in quality or content
- Maintain replacement history
- Track PNG file status

## Troubleshooting Replacement Issues

### Common Problems

**File Access Errors**
- **Problem**: Cannot access replacement file
- **Solution**: Check file permissions and path
- **Prevention**: Ensure files are accessible and not locked

**Format Compatibility**
- **Problem**: Replacement file format not supported
- **Solution**: Convert to supported format (MP4, WebM, MKV)
- **Prevention**: Verify format compatibility before replacement

**Size Limitations**
- **Problem**: Replacement file too large
- **Solution**: Optimize file size or use different format
- **Prevention**: Check file size limits before replacement

**PNG File Issues**
- **Problem**: Workflow PNG file missing or corrupted
- **Solution**: Use regenerate option or manual repair
- **Prevention**: Ensure proper file system permissions

### Error Resolution

**Database Errors**
- **Problem**: Database update fails during replacement
- **Solution**: Run database validation and repair
- **Prevention**: Ensure database integrity before replacement

**File System Errors**
- **Problem**: Cannot write replacement file
- **Solution**: Check disk space and permissions
- **Prevention**: Verify file system access before replacement

**Corruption Issues**
- **Problem**: Replacement causes file corruption
- **Solution**: Restore from backup and retry
- **Prevention**: Verify file integrity before replacement

## Advanced Replacement Features

### Batch Replacement

**Multiple Videos**
- Replace multiple videos efficiently
- Use consistent replacement criteria
- Maintain project consistency

**Template Replacement**
- Use templates for consistent replacements
- Apply standardized improvements
- Maintain visual consistency

### Version Management

**Version Tracking**
- Track improvements across replacements
- Maintain version history
- Document changes and improvements

**Rollback Options**
- Ability to revert to previous versions
- Recovery from problematic replacements
- Maintain project stability

## Integration with Workflow

### Workflow Considerations

**Timing**
- Replace videos at appropriate workflow stages
- Coordinate with team members
- Avoid disrupting ongoing work

**Communication**
- Document replacements for team awareness
- Communicate changes to stakeholders
- Maintain project transparency

### Quality Assurance

**Review Process**
- Implement review process for replacements
- Ensure replacements meet quality standards
- Maintain consistent quality across project

**Testing**
- Test replaced videos in context
- Verify compatibility with other elements
- Ensure no workflow disruptions

Replacing videos effectively helps maintain high quality and consistency throughout your AIMMS project. Follow these guidelines to ensure successful replacements while preserving project integrity and workflow PNG file management.