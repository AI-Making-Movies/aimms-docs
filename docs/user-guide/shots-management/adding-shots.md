# Adding Shots

## Overview

Adding shots to your AIMMS project is the foundation of your storyboard. This guide covers different methods to add shots, best practices for shot organization, and tips for efficient shot management.

## Methods to Add Shots

### Method 1: Using the Add Button

1. **Navigate to Shots Module**
   - Click the **Shots** tab or press `Ctrl+1`
   - Ensure you're viewing the shots table

2. **Add New Shot**
   - Click the **Add New Shot** button in the top menu
   - A dialog will appear with all shot fields

3. **Fill in Shot Details**
   - **Order Number**: The sequence position (e.g., 1, 2, 3)
   - **Shot Name**: Descriptive name for the shot (e.g., "INT_OFFICE_DAY_001")
   - **Section**: Group the shot belongs to (e.g., "Act 1", "Opening Scene")
   - **Description**: What happens in this shot (e.g., "Hero enters office")

4. **Optional Fields**
   - **Image Prompt**: AI prompt for generating base image
   - **Video Prompt**: AI prompt for generating final video
   - **Color Scheme**: Color palette for the shot
   - **Time of Day**: When the shot takes place
   - **Location**: Where the shot takes place
   - **Country**: Country setting for the shot
   - **Year**: Time period for the shot

5. **Save the Shot**
   - Click **Save** to add the shot to your project
   - The shot will appear in the shots table

### Method 2: Adding Relative to Existing Shot

1. **Select Reference Shot**
   - Click on an existing shot in the table
   - This shot will be your reference point

2. **Add New Shot**
   - Click **Add New Shot**
   - Choose whether to add before or after the selected shot

3. **Automatic Order Numbering**
   - AIMMS will suggest an order number based on position
   - You can adjust the order number if needed
   - This helps maintain proper shot sequencing

4. **Fill in Details**
   - Complete the shot information as in Method 1
   - The shot will be inserted at the correct position

### Method 3: Bulk Addition via CSV Import

1. **Prepare CSV File**
   - Create a CSV file with shot information
   - Use the required format (see CSV Import guide)

2. **Import CSV**
   - Click **File** → **Import CSV**
   - Select your CSV file
   - AIMMS will validate and import the shots

3. **Review Import**
   - Check that all shots were imported correctly
   - Verify shot order and information

## Shot Information Fields

### Required Fields

**Order Number**
- **Purpose**: Determines shot sequence in your storyboard
- **Format**: Numeric value (1, 2, 3, etc.)
- **Best Practice**: Use sequential numbering with gaps for future additions (10, 20, 30)

**Shot Name**
- **Purpose**: Unique identifier for the shot
- **Format**: Descriptive text (e.g., "INT_OFFICE_DAY_001")
- **Best Practice**: Use consistent naming conventions

**Section**
- **Purpose**: Group related shots together
- **Format**: Text description (e.g., "Act 1", "Opening Scene")
- **Best Practice**: Use logical groupings for organization

**Description**
- **Purpose**: Brief explanation of what happens in the shot
- **Format**: Short text description
- **Best Practice**: Be descriptive but concise

### Optional Fields

**Image Prompt**
- **Purpose**: AI prompt for generating the base image
- **Format**: Detailed text description
- **Best Practice**: Include key visual elements and style

**Video Prompt**
- **Purpose**: AI prompt for generating the final video
- **Format**: Detailed text description
- **Best Practice**: Include movement, timing, and action details

**Metadata Fields**
- **Color Scheme**: Color palette and mood
- **Time of Day**: Lighting and time context
- **Location**: Physical setting details
- **Country**: Geographic context
- **Year**: Temporal context

## Best Practices for Shot Creation

### Naming Conventions

**Consistent Format**
- Use a consistent format across all shots
- Include location and key action
- Keep names descriptive but manageable

**Examples of Good Shot Names**
- `INT_OFFICE_DAY_001` (Interior Office Day Shot 1)
- `EXT_STREET_NIGHT_002` (Exterior Street Night Shot 2)
- `INT_CAR_DAY_003` (Interior Car Day Shot 3)
- `EXT_PARK_DAWN_004` (Exterior Park Dawn Shot 4)

**Naming Components**
- **Location Type**: INT (Interior) or EXT (Exterior)
- **Specific Location**: Office, Street, Car, Park
- **Time of Day**: DAY, NIGHT, DAWN, DUSK
- **Sequence Number**: 001, 002, 003, etc.

### Organization Strategies

**Section Planning**
- Plan sections before creating shots
- Use sections for acts, scenes, or locations
- Consider your story structure when organizing

**Shot Sequencing**
- Plan shot order carefully
- Leave gaps in numbering for future additions
- Consider logical flow and story progression

**Metadata Completeness**
- Fill in as much metadata as possible
- Use prompts that are specific and actionable
- Include context that will help with AI generation

### Workflow Efficiency

**Template Usage**
- Create templates for similar shot types
- Copy and modify existing shots when appropriate
- Use consistent metadata patterns

**Batch Operations**
- Add multiple related shots together
- Use CSV import for large shot lists
- Apply consistent formatting across shots

## Advanced Shot Management

### Shot Relationships

**Cross-Module Links**
- Shots automatically link to media in other modules
- Image and video takes are associated with shots
- Assets can be linked to specific shots

**Take Management**
- Each shot can have multiple takes
- Takes are organized by type (image, video, mask)
- Star system helps identify favorite takes

### Integration with Other Modules

**Image Storyboard**
- Shots provide context for image generation
- Image prompts are stored with shot information
- Easy navigation between shots and images

**Video Storyboard**
- Video prompts are linked to shots
- Video takes are organized by shot
- Workflow files are associated with shots

**Assets Management**
- Assets can be linked to specific shots
- Reference materials support shot creation
- Asset-shot relationships enhance organization

## Troubleshooting Shot Addition

### Common Issues

**Shot Not Appearing**
- Check that you clicked **Save** after filling in details
- Verify you're viewing "All Sections" in the filter
- Try refreshing the view with `F5`

**Duplicate Shot Names**
- AIMMS allows duplicate names but it's not recommended
- Use unique shot names for better organization
- Consider adding sequence numbers or descriptors

**Invalid Data**
- Ensure required fields are filled
- Check that order numbers are numeric
- Verify shot names aren't too long (max 50 characters)

### Data Validation

**Automatic Validation**
- AIMMS validates data as you enter it
- Required fields are highlighted if missing
- Invalid data shows error messages

**Manual Verification**
- Review shots after creation
- Check order numbers for consistency
- Verify metadata completeness

## Tips for Professional Shot Management

### Planning and Organization

**Storyboard First**
- Plan your storyboard before creating shots
- Consider shot flow and story progression
- Use sections to organize logically

**Metadata Strategy**
- Develop consistent metadata practices
- Use standardized color schemes and locations
- Create templates for common shot types

### Quality Control

**Review Process**
- Review shots after creation for accuracy
- Check for consistency in naming and metadata
- Use the search function to verify shot information

**Continuous Improvement**
- Update shot information as your project evolves
- Refine prompts based on AI generation results
- Adjust organization as your storyboard develops

Adding shots effectively sets the foundation for your entire AIMMS project. Take time to plan and organize your shots properly for the best results throughout your workflow.