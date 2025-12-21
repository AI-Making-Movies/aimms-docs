# Asset Replacement

## Overview

Asset replacement in AIMMS allows you to update existing assets with new or improved versions while preserving all metadata and relationships. This guide covers the replacement process, best practices, and tips for maintaining project integrity.

## When to Replace Assets

### Quality Improvement

**Better Quality**
- You've created a higher quality version of an asset
- Improved resolution, clarity, or detail
- Enhanced visual or audio quality

**Updated Content**
- Changes to asset content or information
- Updated designs, references, or documentation
- Corrections to errors or inconsistencies

**Format Optimization**
- Better file format or compression
- Optimized file size without quality loss
- Improved compatibility or performance

### Error Correction

**Fixing Mistakes**
- Correcting errors in documents or references
- Fixing corrupted or damaged files
- Updating outdated or incorrect information

**Client Feedback**
- Incorporating requested changes
- Addressing quality concerns
- Meeting specific requirements or standards

### Project Evolution

**Style Updates**
- Updating visual style to match project evolution
- Consistency improvements across assets
- Brand or aesthetic updates

**Workflow Changes**
- Changes in project requirements
- Updated reference materials
- Process improvements

## Replacement Process

### Method 1: Right-Click Context Menu

1. **Select Asset to Replace**
   - Right-click the asset you want to replace
   - A context menu will appear

2. **Choose Replace Option**
   - Select **Replace Asset** from the context menu
   - A file browser dialog will open

3. **Choose New Asset**
   - Browse to your new asset file location
   - Select the replacement asset file
   - Ensure it's in a supported format

4. **Confirm Replacement**
   - AIMMS will show a confirmation dialog
   - Review what will be replaced
   - Confirm the replacement

5. **Verify Changes**
   - Check that the new asset appears correctly
   - Verify that metadata is preserved
   - Ensure the asset functions as expected

### Method 2: Using Asset Details

1. **Open Asset Details**
   - Click the asset to view details
   - The asset details panel will appear

2. **Access Replace Option**
   - Click the **Replace Asset** button in the details panel
   - A file browser dialog will open

3. **Select New Asset**
   - Choose your replacement asset file
   - Ensure it meets project requirements

4. **Complete Replacement**
   - Confirm the replacement
   - Verify the new asset appears correctly

### Method 3: Drag and Drop Replacement

1. **Prepare Replacement**
   - Have your new asset file ready
   - Ensure it's the correct replacement

2. **Drag to Target**
   - Drag the new asset file onto the existing asset thumbnail
   - AIMMS will prompt for replacement confirmation

3. **Confirm Action**
   - Confirm that you want to replace the asset
   - Verify the replacement was successful

## What Happens During Replacement

### File Management

**Backup Creation**
- AIMMS automatically backs up the old asset
- Backup is stored in a safe location
- Original asset can be recovered if needed

**File Replacement**
- New asset replaces the old file in the file system
- File path and naming remain consistent
- Asset metadata is preserved

**Relationship Preservation**
- Links to shots and other assets are maintained
- Cross-module references remain intact
- Project structure remains consistent

### Database Updates

**Record Updates**
- Database records are updated with new file information
- File paths are updated to point to new asset
- Metadata relationships are maintained

**History Tracking**
- Replacement is logged in the database
- Original asset information is preserved
- Change history is maintained

## Best Practices for Asset Replacement

### Preparation

**File Verification**
- Ensure replacement asset is in supported format
- Verify asset quality and content
- Check file size and compatibility
- Confirm the replacement meets project standards

**Backup Strategy**
- Always backup important assets before replacement
- Use export features to save current versions
- Document reasons for replacement

**Quality Assessment**
- Compare new asset to original
- Ensure improvements are significant
- Verify the replacement meets all requirements

### Replacement Strategy

**Selective Replacement**
- Replace only when improvements are significant
- Avoid unnecessary replacements that clutter history
- Focus on quality and necessity

**Consistent Naming**
- Let AIMMS handle file naming automatically
- Maintain consistent asset organization
- Avoid manual file system changes

**Metadata Preservation**
- Ensure all metadata is preserved during replacement
- Update any relevant information if needed
- Check that asset relationships are maintained

### Quality Control

**Before Replacement**
- Review the new asset thoroughly
- Compare with the original
- Ensure it meets all requirements
- Verify compatibility with project workflow

**After Replacement**
- Verify the new asset displays correctly
- Check that all metadata is preserved
- Test that the asset works in context
- Confirm asset relationships are intact

**Documentation**
- Document the reason for replacement
- Note any changes in quality or content
- Maintain replacement history
- Track asset evolution

## Asset Versioning

### Manual Versioning

**Version Numbers**
- Create multiple assets with version numbers
- Examples: "character_design_v01.pdf", "character_design_v02.pdf"
- Track changes and improvements over time

**Naming Conventions**
- Use consistent versioning format
- Include version information in asset names
- Maintain clear version history

### Metadata-Based Versioning

**Description Updates**
- Use description field to document changes
- Note improvements and updates
- Maintain version history in metadata

**Tag Management**
- Add version tags to assets
- Use tags to track asset evolution
- Maintain searchable version history

### Backup and Recovery

**Version Backup**
- Backup important asset versions
- Maintain version history
- Use export features for version management

**Recovery Options**
- Restore from backup if replacement fails
- Recover previous versions when needed
- Maintain asset continuity

## Troubleshooting Replacement Issues

### Common Problems

**File Access Errors**
- **Problem**: Cannot access replacement file
- **Solution**: Check file permissions and path
- **Prevention**: Ensure files are accessible and not locked

**Format Compatibility**
- **Problem**: Replacement file format not supported
- **Solution**: Convert to supported format
- **Prevention**: Verify format compatibility before replacement

**Size Limitations**
- **Problem**: Replacement file too large
- **Solution**: Optimize file size or use different format
- **Prevention**: Check file size limits before replacement

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

**Multiple Assets**
- Replace multiple assets efficiently
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
- Replace assets at appropriate workflow stages
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
- Test replaced assets in context
- Verify compatibility with other elements
- Ensure no workflow disruptions

Replacing assets effectively helps maintain high quality and consistency throughout your AIMMS project. Follow these guidelines to ensure successful replacements while preserving project integrity.