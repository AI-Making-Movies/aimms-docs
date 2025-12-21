# Editing Shots

## Overview

Editing shots in AIMMS allows you to modify shot information, update metadata, and refine your storyboard. This guide covers different methods to edit shots, batch editing capabilities, and best practices for maintaining data consistency.

## Single Shot Editing

### Method 1: Double-Click Editing

1. **Select the Shot**
   - Click on the shot row in the shots table
   - The shot will be highlighted

2. **Open Edit Dialog**
   - Double-click the selected shot
   - The shot details dialog will open

3. **Make Changes**
   - Modify any shot information:
     - Order number
     - Shot name
     - Section
     - Description
     - All prompt fields
     - Metadata fields

4. **Save Changes**
   - Click **Save** to apply your changes
   - The updated information will appear in the table

### Method 2: Context Menu Editing

1. **Right-Click the Shot**
   - Right-click on any shot in the table
   - A context menu will appear

2. **Select Edit Option**
   - Choose **View/Edit Details** from the menu
   - The shot details dialog will open

3. **Edit Information**
   - Make your desired changes
   - All fields are editable

4. **Apply Changes**
   - Click **Save** to confirm changes
   - Cancel to discard changes

### Method 3: Direct Table Editing

1. **Click to Edit**
   - Click directly on a cell in the shots table
   - The cell will become editable

2. **Modify Content**
   - Edit the cell content directly
   - Use Enter to confirm changes
   - Use Escape to cancel changes

3. **Automatic Save**
   - Changes are saved automatically
   - The table updates immediately

## What You Can Edit

### Core Shot Information

**Order Number**
- **Purpose**: Change the shot sequence
- **Impact**: Affects shot ordering throughout AIMMS
- **Best Practice**: Be careful when changing order numbers

**Shot Name**
- **Purpose**: Rename the shot
- **Impact**: Media files are updated automatically
- **Best Practice**: Use consistent naming conventions

**Section**
- **Purpose**: Move shot to different section
- **Impact**: Affects section filtering and organization
- **Best Practice**: Use logical section groupings

**Description**
- **Purpose**: Update shot description
- **Impact**: Changes displayed information
- **Best Practice**: Keep descriptions clear and concise

### Prompt and Metadata Fields

**Image Prompt**
- **Purpose**: Update AI prompt for base image generation
- **Impact**: Affects future image generation
- **Best Practice**: Make prompts more specific and detailed

**Video Prompt**
- **Purpose**: Update AI prompt for video generation
- **Impact**: Affects future video generation
- **Best Practice**: Include movement and timing details

**Metadata Fields**
- **Color Scheme**: Update color palette information
- **Time of Day**: Change lighting context
- **Location**: Update physical setting
- **Country**: Change geographic context
- **Year**: Update temporal context

## Batch Editing

### Selecting Multiple Shots

1. **Multi-Selection**
   - Hold **Ctrl** (or **Cmd** on Mac) while clicking shots
   - Or click and drag to select a range of shots
   - Selected shots will be highlighted

2. **Verify Selection**
   - Check that all intended shots are selected
   - Use the selection count if available

### Batch Edit Process

1. **Right-Click Selection**
   - Right-click on any selected shot
   - Choose **Edit Selected Shots** from context menu

2. **Make Changes**
   - Changes will apply to all selected shots
   - Only common fields can be edited in batch mode
   - Be careful with fields that should be unique

3. **Apply Changes**
   - Click **Save** to apply changes to all selected shots
   - Changes are applied simultaneously

### Batch Editing Best Practices

**Common Fields Only**
- Edit fields that should be the same across shots
- Examples: Section, Color Scheme, Time of Day
- Avoid editing unique fields like Shot Name in batch mode

**Preview Changes**
- Review what will be changed before applying
- Consider the impact on each selected shot
- Use undo if changes aren't as expected

**Selective Editing**
- Use filters to select shots for batch editing
- Edit similar shots together (same section, location, etc.)
- Verify changes after batch operations

## Advanced Editing Features

### Shot Information Panel

**Details View**
- Click any shot to view detailed information
- See all shot metadata in one place
- Access related media and assets

**Quick Actions**
- Direct links to related modules
- Quick access to shot-specific functions
- Context-sensitive actions

### Search and Replace

**Find and Replace**
- Use search to locate specific text
- Replace across multiple shots if needed
- Be careful with broad replacements

**Filter-Based Editing**
- Filter shots by criteria
- Edit all filtered shots at once
- Useful for updating similar shots

## Data Validation and Safety

### Validation Features

**Real-Time Validation**
- AIMMS validates data as you edit
- Required fields are highlighted
- Invalid data shows error messages

**Duplicate Detection**
- Warns about duplicate shot names
- Prevents invalid order numbers
- Checks for data consistency

### Safety Features

**Confirmation Dialogs**
- Confirm before making significant changes
- Warn about potential data conflicts
- Provide undo options when available

**Backup and Recovery**
- Changes are tracked in the database
- Can revert to previous versions if needed
- Export data before major edits

## Troubleshooting Editing Issues

### Common Problems

**Changes Not Saving**
- Ensure you clicked **Save** after editing
- Check for validation errors
- Verify database isn't locked

**Unexpected Behavior**
- Check if multiple shots are selected
- Verify you're editing the correct field
- Look for system messages or warnings

**Data Loss Prevention**
- Always export data before major edits
- Use the backup system regularly
- Be careful with batch operations

### Error Resolution

**Validation Errors**
- Read error messages carefully
- Check field requirements and formats
- Fix issues before saving

**System Errors**
- Restart AIMMS if editing stops working
- Check system resources and permissions
- Contact support if issues persist

## Best Practices for Shot Editing

### Data Consistency

**Naming Conventions**
- Maintain consistent shot naming
- Use standardized formats
- Avoid special characters and spaces

**Metadata Standards**
- Use consistent terminology
- Follow established color schemes
- Maintain location and time standards

### Workflow Efficiency

**Batch Operations**
- Use batch editing for similar shots
- Filter shots before editing
- Plan edits to minimize individual operations

**Organization**
- Keep related shots grouped by section
- Use consistent metadata across similar shots
- Regularly review and clean up shot information

### Quality Control

**Review Process**
- Review changes after editing
- Check for consistency across shots
- Verify all required fields are complete

**Continuous Improvement**
- Update shot information as project evolves
- Refine prompts based on results
- Improve organization over time

## Integration with Other Modules

### Cross-Module Updates

**Media Module Updates**
- Shot name changes update media file references
- Section changes affect filtering in media modules
- Description changes update displayed information

**Asset Module Integration**
- Shot edits can affect asset associations
- Metadata changes may impact asset organization
- Prompt updates affect asset usage

### Workflow Synchronization

**Real-Time Updates**
- Changes appear immediately in other modules
- No need to manually refresh other views
- Consistent data across all AIMMS modules

Editing shots effectively helps maintain an organized and accurate storyboard. Use these techniques to keep your project data current and consistent throughout your workflow.