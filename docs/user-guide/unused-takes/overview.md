# Unused Takes Overview

## Introduction

The Unused Takes Manager module helps you identify and manage media files that are no longer associated with any shots in your project. This module is essential for maintaining a clean, organized project and optimizing storage space.

## Understanding Unused Takes

### What Are Unused Takes?

Unused takes are media files (images or videos) that exist in your project folders but are not referenced in the AIMMS database. These files can accumulate over time due to:

- **Deleted Shots**: When shots are deleted, their associated media files may remain
- **Replaced Takes**: Old takes are sometimes not properly cleaned up
- **Manual File Operations**: Files added or moved outside of AIMMS
- **Project Migration**: Files from previous versions or systems

### Why Manage Unused Takes?

**Storage Optimization**
- Free up disk space by removing unnecessary files
- Improve project performance by reducing file count
- Maintain efficient backup and sync operations

**Project Organization**
- Keep your project clean and organized
- Prevent confusion from orphaned files
- Maintain clear file-shot relationships

**Data Integrity**
- Identify potential data inconsistencies
- Ensure all media files are properly tracked
- Maintain project reliability

## Key Features

### Detection and Analysis

**Automatic Detection**
- Scans project folders for untracked media files
- Compares file system with database records
- Identifies orphaned images and videos

**Comprehensive Analysis**
- Categorizes unused files by type
- Shows file sizes and storage impact
- Provides detailed information about each unused file

### Safe Management

**Safety Checks**
- Verifies files are truly unused before deletion
- Prevents accidental removal of active files
- Maintains database integrity

**Recovery Options**
- Backup system for deleted files
- Recovery options for accidental deletions
- Audit trail of cleanup operations

### Bulk Operations

**Efficient Cleanup**
- Select multiple unused files for deletion
- Batch operations for large projects
- Progress tracking during cleanup

**Selective Management**
- Choose which files to keep or delete
- Filter by file type, size, or date
- Customizable cleanup criteria

## Using the Unused Takes Manager

### Accessing the Module

1. **Navigate to Unused Takes**
   - Click the **Unused** tab or press `Ctrl+5`
   - The unused takes manager will load

2. **Initial Scan**
   - Module automatically scans for unused files
   - Results appear in the main interface
   - Status indicators show scan progress

### Reviewing Unused Files

**File Information**
- **File Name**: Name of the unused file
- **File Type**: Image or video format
- **File Size**: Storage space used
- **Location**: Path within project structure
- **Last Modified**: When file was last changed

**Analysis Results**
- **Total Files**: Number of unused files found
- **Total Size**: Combined storage space of unused files
- **File Types**: Breakdown by format
- **Recommendations**: Suggested cleanup actions

### Managing Unused Files

**Selection Options**
- **Select All**: Choose all unused files
- **Select None**: Clear all selections
- **Invert Selection**: Toggle all selections
- **Filter Selection**: Choose files by criteria

**Cleanup Actions**
- **Delete Selected**: Remove chosen files permanently
- **Keep Selected**: Mark files to preserve
- **Export List**: Save list of unused files for review
- **Generate Report**: Create detailed cleanup report

## Best Practices

### Regular Maintenance

**Scheduled Reviews**
- Check for unused files regularly
- Set up routine cleanup schedules
- Monitor storage usage trends

**Conservative Approach**
- Review files before deletion
- Keep important files even if unused
- Document reasons for keeping files

### Safety Precautions

**Backup First**
- Always backup project before cleanup
- Verify backup integrity
- Test recovery procedures

**Gradual Cleanup**
- Remove files in batches
- Monitor project after each cleanup
- Verify no functionality is affected

### Documentation

**Cleanup Records**
- Document cleanup operations
- Note any files kept and why
- Track storage space recovered
- Maintain cleanup history

## Troubleshooting

### Common Issues

**Files Not Detected**
- **Problem**: Unused files not found by scanner
- **Solution**: Check file permissions and access
- **Prevention**: Ensure scanner has proper access

**False Positives**
- **Problem**: Active files marked as unused
- **Solution**: Verify file relationships in database
- **Prevention**: Use conservative detection settings

**Cleanup Errors**
- **Problem**: Deletion operations fail
- **Solution**: Check file permissions and locks
- **Prevention**: Close other applications accessing files

### Error Resolution

**Permission Issues**
- **Problem**: Cannot access or delete files
- **Solution**: Check file system permissions
- **Prevention**: Ensure proper user permissions

**Database Issues**
- **Problem**: Database inconsistencies affect detection
- **Solution**: Run database validation and repair
- **Prevention**: Regular database maintenance

**File System Errors**
- **Problem**: File system corruption or errors
- **Solution**: Run file system checks and repairs
- **Prevention**: Regular system maintenance

## Integration with Other Modules

### Cross-Module Coordination

**Shots Module**
- Coordinate with shot deletion operations
- Verify shot-media relationships
- Maintain data consistency

**Media Modules**
- Sync with image and video management
- Coordinate media file operations
- Maintain file organization

**Project Management**
- Integrate with project cleanup workflows
- Coordinate with backup operations
- Support project migration

### Workflow Integration

**Regular Maintenance**
- Include unused file cleanup in project maintenance
- Schedule regular reviews and cleanup
- Monitor project health and organization

**Project Lifecycle**
- Clean up unused files during project phases
- Prepare projects for archiving or migration
- Maintain project efficiency throughout lifecycle

The Unused Takes Manager is essential for maintaining a healthy, organized AIMMS project. Regular use of this module helps ensure optimal performance and storage efficiency.