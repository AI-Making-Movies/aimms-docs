# Export CSV

## Overview

The Export CSV feature in AIMMS allows you to export your project data to CSV files for backup, sharing, or analysis purposes. This guide covers the export process, file formats, and best practices for using exported data.

## What Gets Exported

### Complete Project Data

When you export CSV data, AIMMS creates timestamped files containing:

**Shots Data:**
- All shot information and metadata
- Shot order, names, descriptions
- Image and video prompts
- Color schemes, locations, time settings
- Custom metadata fields

**Takes Data:**
- Media take information for images and videos
- Take numbers and file paths
- Take status and metadata
- Starred take information

**Assets Data:**
- Project asset information
- Asset names, categories, descriptions
- Asset metadata and relationships
- Asset file paths and status

**Meta Data:**
- Project metadata and configuration
- Database schema information
- Project settings and preferences
- Export timestamp and version information

**Deleted Shots:**
- Recently deleted shot information (if available)
- Deletion timestamps and reasons
- Recovery information for deleted shots

## Export Process

### Method 1: Menu Export

1. **Access Export Function**
   - Click **File** in the main menu
   - Select **Export CSV** from the dropdown
   - Or use the keyboard shortcut `Ctrl+E`

2. **Export Execution**
   - AIMMS validates project data
   - Creates timestamped CSV files
   - Saves files to `project_root/data/csv/`

3. **Export Completion**
   - Export summary shows which files were created
   - Files are ready for use or sharing
   - Project remains open and functional

### Method 2: Automatic Export

1. **Scheduled Export**
   - Configure automatic export in settings
   - Set export frequency and timing
   - Enable automatic backup creation

2. **Event-Triggered Export**
   - Export on specific events (project save, close)
   - Export on data changes
   - Export on user actions

## Export File Format

### CSV Structure

**File Naming Convention:**
```
shots_YYYYMMDD_HHMM.csv
takes_YYYYMMDD_HHMM.csv
assets_YYYYMMDD_HHMM.csv
meta_YYYYMMDD_HHMM.csv
```

**Column Structure:**
- **Headers**: First row contains column names
- **Data Rows**: Subsequent rows contain data
- **Encoding**: UTF-8 encoding for international characters
- **Delimiter**: Comma-separated values

### Data Format Details

**Shots CSV Format:**
```csv
shot_id,order_number,shot_name,section,description,image_prompt,colour_scheme_image,time_of_day,location,country,year,video_prompt,created_date,modified_date
1,1,INT_OFFICE_DAY_001,Act 1,Hero enters office,A man sitting at a desk,Warm tones,Day,Office,USA,2024,A man walks into an office,2025-12-21T10:30:00Z,2025-12-21T14:45:00Z
```

**Takes CSV Format:**
```csv
take_id,shot_id,take_type,take_number,file_path,file_size,created_date,starred,status
1,1,image,base_01,media/1/base_01.png,2560000,2025-12-21T10:35:00Z,1,active
2,1,video,video_01,media/1/video_01.mp4,51200000,2025-12-21T10:40:00Z,1,active
```

**Assets CSV Format:**
```csv
asset_id,asset_name,category,description,file_path,file_size,created_date,source,license
1,Forest Background,references,Reference images for forest scene,assets/references/forest.jpg,1024000,2025-12-21T09:30:00Z,Unsplash,Creative Commons
```

## Use Cases for Export

### Backup and Recovery

**Regular Backups:**
- Create regular CSV exports for backup
- Store exports in safe locations
- Use for project recovery if needed

**Version Control:**
- Export before major changes
- Track project evolution over time
- Compare different project versions

**Disaster Recovery:**
- Use exports to restore corrupted projects
- Recover data from backup files
- Rebuild projects from CSV data

### Data Sharing and Collaboration

**Team Collaboration:**
- Share project data with team members
- Export specific sections or shots
- Coordinate work across team members

**Client Communication:**
- Export shot lists for client review
- Share project progress reports
- Provide data for external review

**Integration with Other Tools:**
- Import CSV data into other applications
- Use with spreadsheet software
- Integrate with project management tools

### Analysis and Reporting

**Project Analysis:**
- Analyze project statistics and trends
- Track progress and productivity
- Generate project reports

**Data Analysis:**
- Use with data analysis tools
- Create custom reports and charts
- Analyze workflow efficiency

## Best Practices

### Export Frequency

**Regular Schedule:**
- Export after significant changes
- Create daily or weekly exports
- Maintain consistent export schedule

**Event-Based Export:**
- Export before major edits
- Export after completing project phases
- Export before sharing with others

### File Management

**Organized Storage:**
- Store exports in organized folders
- Use consistent naming conventions
- Maintain export history

**Backup Strategy:**
- Store exports in multiple locations
- Use cloud storage for additional backup
- Verify export file integrity

### Data Security

**File Protection:**
- Protect export files with appropriate permissions
- Encrypt sensitive project data
- Control access to export files

**Version Control:**
- Track changes between exports
- Document export purposes and contents
- Maintain export documentation

## Troubleshooting Export Issues

### Common Problems

**Export Fails:**
- Check file permissions in export directory
- Verify sufficient disk space
- Ensure project is not locked or in use

**Incomplete Export:**
- Check for corrupted project data
- Verify all modules are accessible
- Run project validation before export

**File Access Issues:**
- Check file system permissions
- Verify export directory is writable
- Ensure no other processes are using files

### Error Resolution

**Permission Errors:**
- Check user permissions for export directory
- Run AIMMS with appropriate privileges
- Verify file system access

**Disk Space Issues:**
- Check available disk space
- Clean up old export files
- Use alternative export location

**Corruption Issues:**
- Run project validation
- Check for database corruption
- Contact support if issues persist

## Advanced Export Features

### Selective Export

**Filter by Criteria:**
- Export specific sections or shots
- Filter by date ranges
- Export only starred or active items

**Custom Export:**
- Choose specific data fields to export
- Create custom export formats
- Export to different file formats

### Automated Export

**Scheduled Tasks:**
- Set up automated export schedules
- Configure export triggers
- Monitor export success and failures

**Export Scripts:**
- Create custom export scripts
- Automate complex export workflows
- Integrate with external systems

The Export CSV feature is essential for project backup, collaboration, and analysis. Regular use of this feature helps ensure data safety and facilitates efficient project management.