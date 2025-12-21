# Deleting Shots

## Overview

Deleting shots in AIMMS is a safe process that includes multiple safety features and recovery options. This guide covers how to delete shots, understand the safety mechanisms, and recover deleted shots when needed.

## Safety Features

AIMMS includes multiple safety features for shot deletion:

### Confirmation Dialog
- **Always Asks**: AIMMS always asks before deleting any shot
- **Clear Warning**: Shows clear warning about the deletion
- **Recovery Information**: Informs about recovery options

### Recovery Options
- **Deleted Shots Table**: Deleted shots are moved to a special table
- **Media Preservation**: Associated media files are preserved temporarily
- **Database Integrity**: Maintains database consistency
- **Backup System**: Multiple backup mechanisms available

### Media File Handling
- **Temporary Preservation**: Media files are kept for recovery
- **Safe Cleanup**: Files are only removed after confirmation
- **Relationship Tracking**: Maintains file-shot relationships

## Deleting Individual Shots

### Method 1: Using the Delete Button

1. **Select the Shot**
   - Click on the shot you want to delete in the shots table
   - The shot will be highlighted

2. **Delete the Shot**
   - Click the **Delete Selected Shots** button
   - Or press the **Delete** key on your keyboard

3. **Confirm Deletion**
   - A confirmation dialog will appear
   - Read the warning message carefully
   - Click **Yes** to confirm or **No** to cancel

4. **Verify Deletion**
   - The shot will disappear from the main shots table
   - It will be moved to the deleted_shots table

### Method 2: Using Context Menu

1. **Right-Click the Shot**
   - Right-click on the shot you want to delete
   - A context menu will appear

2. **Select Delete Option**
   - Choose **Delete Shot** from the context menu
   - Follow the same confirmation process

### Method 3: Batch Deletion

1. **Select Multiple Shots**
   - Hold **Ctrl** (or **Cmd** on Mac) while clicking shots
   - Or click and drag to select a range
   - Selected shots will be highlighted

2. **Delete Selection**
   - Click **Delete Selected Shots**
   - Confirm the deletion of multiple shots

3. **Verify Results**
   - All selected shots will be deleted
   - Each shot goes through the same safety process

## What Happens During Deletion

### Database Operations

**Shot Removal**
- Shot is removed from the main shots table
- All shot metadata is preserved in deleted_shots table
- Database relationships are maintained

**Media File Handling**
- Associated media files are NOT immediately deleted
- Files are preserved for potential recovery
- File paths are stored for restoration

**Take Management**
- Shot takes are preserved with their metadata
- Take relationships are maintained
- Starred status and other take information is saved

### Recovery Information Stored

**Deleted Shot Data**
- Complete shot information is preserved
- All metadata and prompts are saved
- Original order and organization data is maintained

**Media File References**
- File paths and relationships are stored
- Take information is preserved
- Workflow file references are maintained

## Recovering Deleted Shots

### Accessing Recovery Tools

1. **Open Project Recovery**
   - Click **File** → **Project Recovery**
   - Or navigate to the recovery section in the menu

2. **View Deleted Shots**
   - The recovery interface shows recently deleted shots
   - Filter by date or search for specific shots
   - View shot details and associated media

### Recovery Process

1. **Select Shots to Recover**
   - Check the boxes next to shots you want to restore
   - Review shot information before recovery
   - Select multiple shots if needed

2. **Initiate Recovery**
   - Click the **Restore** button
   - Confirm the recovery operation
   - AIMMS will restore shots to their original state

3. **Verify Recovery**
   - Restored shots appear back in the main shots table
   - Media files are reassociated
   - All metadata and relationships are restored

### Recovery Limitations

**Time Limits**
- Recovery is typically available for recent deletions
- Older deletions may not be recoverable
- Check recovery tool for available timeframes

**Media File Availability**
- Recovery depends on media files still being present
- If media files were manually deleted, recovery may be partial
- Always verify media file availability before recovery

## Best Practices for Shot Deletion

### Before Deleting

**Review Shot Information**
- Double-check that you're deleting the correct shot
- Review associated media and takes
- Consider if the shot might be needed later

**Document Reasons**
- Note why you're deleting the shot
- Document any important information
- Consider creating a backup before deletion

**Check Dependencies**
- Verify the shot isn't referenced elsewhere
- Check for associated assets or workflows
- Consider impact on project organization

### During Deletion

**Use Confirmation Dialogs**
- Always read warning messages carefully
- Confirm you understand the implications
- Don't rush through deletion confirmations

**Selective Deletion**
- Delete only what you're certain about
- Consider hiding shots instead of deleting
- Use sections to organize rather than delete

### After Deletion

**Verify Results**
- Confirm the shot was deleted successfully
- Check that related shots are still intact
- Verify project organization is maintained

**Monitor Recovery Options**
- Keep recovery tools accessible
- Understand the recovery timeframe
- Know how to restore shots if needed

## Troubleshooting Deletion Issues

### Common Problems

**Shot Won't Delete**
- Check if the shot is locked or in use
- Verify database permissions
- Ensure no other processes are accessing the shot

**Recovery Failed**
- Check if recovery timeframe has expired
- Verify media files are still present
- Try restoring individual shots instead of batches

**Unexpected Behavior**
- Check for database corruption
- Verify AIMMS has proper file permissions
- Restart AIMMS and try again

### Error Resolution

**Database Errors**
- Run database validation tools
- Check for database locks
- Contact support if database issues persist

**File System Errors**
- Verify file system permissions
- Check available disk space
- Ensure media files aren't locked by other processes

## Advanced Deletion Features

### Permanent Deletion

**When to Use**
- After confirming you don't need the shot
- When recovering storage space is necessary
- For cleaning up test or duplicate shots

**Process**
- Use permanent deletion tools in recovery section
- Confirm understanding of irreversible action
- Verify all associated data will be removed

### Bulk Cleanup

**Project Cleanup**
- Identify shots that are no longer needed
- Use batch deletion for efficiency
- Always backup before bulk operations

**Storage Management**
- Delete shots to free up storage space
- Clean up unused media files
- Optimize project size and performance

## Integration with Project Management

### Project Organization

**Section Management**
- Use sections to organize rather than delete
- Move shots between sections as needed
- Maintain logical project structure

**Workflow Integration**
- Coordinate deletions with team members
- Document changes for project history
- Maintain version control if applicable

### Data Integrity

**Backup Procedures**
- Always backup before major deletion operations
- Use CSV export for additional backup
- Verify backup integrity before deletion

**Audit Trail**
- Keep records of major deletions
- Document reasons for deletions
- Maintain project history for reference

Deleting shots safely requires understanding AIMMS's safety features and recovery options. Always take time to review before deletion and maintain proper backups for important project data.