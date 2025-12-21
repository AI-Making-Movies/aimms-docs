# Video Metadata

## Overview

Video metadata in AIMMS provides comprehensive information about your video files, including technical specifications, workflow data, and organizational details. This guide covers how to view, manage, and utilize video metadata effectively.

## Understanding Video Metadata

### What Is Video Metadata?

Video metadata is information about your video files that helps with organization, searchability, and workflow management. It includes both automatically extracted technical data and manually added organizational information.

### Types of Video Metadata

**Technical Metadata**
- **Duration**: Video length in HH:MM:SS format
- **Resolution**: Width x height in pixels
- **Frame Rate**: FPS (frames per second)
- **Codec**: Video compression format
- **File Size**: Storage space used by the video
- **Aspect Ratio**: Display proportions
- **Bitrate**: Data rate and quality indicators

**Workflow Metadata**
- **Workflow PNG**: Status of workflow file
- **Take Type**: Final video, mask video, etc.
- **Creation Date**: When the take was added
- **File Path**: Location in project structure
- **AI Prompts**: Prompts used to generate the video
- **Workflow Configuration**: Generation settings and parameters

**Organizational Metadata**
- **Shot Name**: Which shot this video belongs to
- **Take Number**: Version identifier
- **Star Status**: Whether video is starred/favorite
- **Quality Ratings**: Quality assessment and ratings
- **Tags**: Keywords for searchability
- **Notes**: Additional information and context

## Viewing Video Metadata

### Method 1: Hover Preview

1. **Navigate to Video Gallery**
   - Open the Video Storyboard module
   - Browse the thumbnail gallery

2. **Hover Over Thumbnails**
   - Hover your mouse over any video thumbnail
   - Quick metadata appears in a tooltip
   - See duration, resolution, and format

3. **Quick Information**
   - **Duration**: Video length
   - **Resolution**: Width x height
   - **File Size**: Storage space used
   - **Format**: Video type and quality

### Method 2: Click for Details

1. **Select Video**
   - Click any video thumbnail
   - The video details panel appears

2. **View Comprehensive Metadata**
   - **Technical Information**: Complete technical specifications
   - **Workflow Data**: AI prompts and workflow information
   - **Organizational Info**: Shot and take information
   - **Status Indicators**: Video status and quality markers

3. **Additional Actions**
   - **Play Full**: Open in floating player
   - **Replace**: Replace with new video
   - **Star/Unstar**: Mark as favorite
   - **Edit Details**: Modify metadata

### Method 3: Floating Player Metadata

1. **Open Floating Player**
   - Click any video to open the floating player
   - Video starts playing automatically

2. **Show Metadata**
   - Click the **📊** (metadata) button
   - Or press **I** key
   - Comprehensive metadata panel appears

3. **Detailed Information**
   - **Video Specifications**: Technical details
   - **Workflow Information**: Generation data
   - **File Properties**: Storage and access info
   - **Quality Assessment**: Quality ratings and notes

## Metadata Categories Explained

### Technical Information

**Duration**
- **Format**: HH:MM:SS (hours:minutes:seconds)
- **Purpose**: Video length for planning and organization
- **Usage**: Calculate total project runtime, plan edits

**Resolution**
- **Format**: Width x Height (e.g., 1920x1080)
- **Purpose**: Video quality and display size
- **Usage**: Ensure consistency, plan output format

**Frame Rate**
- **Format**: FPS (frames per second)
- **Purpose**: Video smoothness and motion quality
- **Usage**: Maintain consistency, match project requirements

**Codec**
- **Purpose**: Video compression format
- **Usage**: Compatibility, quality, file size
- **Common Types**: H.264, H.265, VP9, AV1

**File Size**
- **Format**: MB or GB
- **Purpose**: Storage space and performance
- **Usage**: Manage project size, optimize performance

**Aspect Ratio**
- **Format**: 16:9, 4:3, 1:1, etc.
- **Purpose**: Video proportions and display
- **Usage**: Maintain consistency, plan output

### Workflow Information

**Workflow PNG Status**
- **✅ Present**: Workflow PNG file exists and is valid
- **⚠️ Missing**: PNG file is missing (can be regenerated)
- **❌ Invalid**: PNG file exists but is corrupted

**AI Prompts**
- **Image Prompt**: Prompt used for base image generation
- **Video Prompt**: Prompt used for video generation
- **Workflow Settings**: Generation parameters and settings

**Take Type**
- **Final Video**: Completed shot video
- **Mask Video**: Mask or alpha channel video
- **Test Video**: Experimental or test generation
- **Reference**: Reference or placeholder video

### Organizational Information

**Shot Information**
- **Shot Name**: Descriptive identifier for the shot
- **Shot ID**: Numeric identifier in the database
- **Section**: Group the shot belongs to
- **Description**: Brief explanation of the shot

**Take Information**
- **Take Number**: Version identifier (video_01, video_02, etc.)
- **Take ID**: Unique UUID identifier
- **Creation Date**: When the take was added
- **Status**: Current status in workflow

**Quality and Ratings**
- **Star Status**: Whether video is starred/favorite
- **Quality Rating**: Quality assessment (1-5 stars or similar)
- **Notes**: Additional quality information
- **Tags**: Keywords for organization and search

## Managing Video Metadata

### Adding Custom Metadata

1. **Open Video Details**
   - Click any video thumbnail
   - The details panel appears

2. **Edit Metadata**
   - Click **Edit Details** button
   - Modify any editable fields
   - Add notes, ratings, or tags

3. **Save Changes**
   - Click **Save** to apply changes
   - Metadata is updated in the database
   - Changes appear immediately

### Metadata Fields You Can Edit

**Notes and Descriptions**
- **Purpose**: Add context and information
- **Usage**: Document decisions, note issues, add context
- **Best Practice**: Be descriptive and consistent

**Quality Ratings**
- **Purpose**: Assess video quality
- **Usage**: Track improvements, identify issues
- **Best Practice**: Use consistent rating criteria

**Tags and Keywords**
- **Purpose**: Improve searchability and organization
- **Usage**: Categorize videos, add search terms
- **Best Practice**: Use consistent tagging system

**Custom Fields**
- **Purpose**: Add project-specific information
- **Usage**: Track project-specific data
- **Best Practice**: Plan custom fields carefully

### Metadata Validation

**Automatic Validation**
- AIMMS validates metadata automatically
- Required fields are checked
- Format and content are verified

**Manual Verification**
- Review metadata for accuracy
- Check for consistency across takes
- Verify workflow information

**Error Handling**
- Invalid metadata shows error messages
- Required fields are highlighted
- Validation prevents saving invalid data

## Using Metadata Effectively

### Search and Organization

**Search by Metadata**
- Use search box to find videos by metadata
- Search technical specifications
- Find videos by tags or notes

**Filter by Metadata**
- Filter by resolution, duration, or other technical specs
- Organize by quality ratings
- Group by workflow status

**Sort by Metadata**
- Sort by creation date, file size, or duration
- Organize by quality or ratings
- Arrange by workflow status

### Workflow Integration

**Quality Control**
- Use metadata for quality assessment
- Track improvements over time
- Identify patterns in video quality

**Project Management**
- Use metadata for project organization
- Track progress and status
- Plan workflow based on metadata

**Collaboration**
- Share metadata with team members
- Use consistent metadata practices
- Document decisions and changes

### Export and Reporting

**Metadata Export**
- Export metadata with video files
- Include metadata in project reports
- Use metadata for project documentation

**Reporting and Analysis**
- Generate reports based on metadata
- Analyze project statistics
- Track workflow efficiency

## Best Practices for Video Metadata

### Consistency

**Standardized Formats**
- Use consistent date formats
- Standardize naming conventions
- Maintain consistent quality ratings

**Complete Information**
- Fill in all relevant metadata fields
- Don't leave important fields blank
- Update metadata as project evolves

**Regular Updates**
- Keep metadata current
- Update when videos are modified
- Review and clean up old metadata

### Quality Control

**Accuracy**
- Ensure metadata is accurate and correct
- Verify technical specifications
- Double-check workflow information

**Completeness**
- Include all relevant information
- Don't omit important details
- Use metadata to enhance organization

**Relevance**
- Focus on useful metadata
- Avoid unnecessary or redundant information
- Prioritize metadata that aids workflow

### Organization

**Logical Structure**
- Organize metadata logically
- Use consistent categorization
- Plan metadata structure carefully

**Searchability**
- Use descriptive and searchable terms
- Include relevant keywords
- Make metadata easy to find and use

**Integration**
- Integrate metadata with workflow
- Use metadata to enhance productivity
- Connect metadata to project goals

Effective video metadata management helps you organize, search, and manage your video assets more efficiently. Use these practices to maximize the value of your video metadata.