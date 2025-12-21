# Managing Assets

## Overview

Managing assets in AIMMS involves organizing, updating, and maintaining your project's supporting materials. This guide covers how to view, organize, update, and maintain your asset collection effectively.

## Viewing and Organizing Assets

### Gallery View

**Thumbnail Display**
- Assets displayed as thumbnails with key information
- Visual preview for image-based assets
- Quick overview of all project assets

**Information Display**
- **Asset Name**: Descriptive name for the asset
- **Category**: Type of asset (references, audio, documents, etc.)
- **File Type**: Icon indicating file format
- **Size**: File size information
- **Star Status**: Whether asset is starred/favorite

### List View

**Tabular Format**
- Detailed information in columns
- Sortable columns for organization
- Comprehensive asset overview

**Column Information**
- **Name**: Asset name
- **Type**: File format
- **Size**: File size
- **Date Added**: When asset was imported
- **Category**: Asset classification
- **Description**: Asset description

### Filtering and Search

**By Category**
- Use category filters to show specific asset types
- Common categories: References, Audio, 3D, Documents
- Custom categories for project-specific organization

**By File Type**
- Filter by specific file formats
- Show only images, audio, or documents
- Focus on specific asset types

**Search Functionality**
- Use search box to find assets by name or description
- Search across all asset metadata
- Real-time filtering as you type

## Asset Metadata Management

### Adding Asset Metadata

1. **Select Asset**
   - Click any asset to view details
   - The asset details panel appears

2. **Edit Details**
   - Click **Edit Details** button
   - Fill in asset information:
     - **Name**: Descriptive asset name
     - **Category**: Asset type classification
     - **Description**: What the asset is used for
     - **Tags**: Keywords for easy searching
     - **Source**: Where the asset came from
     - **License**: Usage rights and permissions

3. **Save Changes**
   - Click **Save** to update metadata
   - Changes are saved to the database
   - Asset information is updated immediately

### Metadata Fields Explained

**Name**
- **Purpose**: Clear, descriptive identifier
- **Format**: Include key identifying information
- **Example**: "Forest Background Reference Images"

**Category**
- **Purpose**: Asset type classification
- **Options**: References, Audio, 3D Model, Texture, Document, etc.
- **Usage**: Organization and filtering

**Description**
- **Purpose**: What the asset contains and how it's used
- **Format**: Detailed explanation
- **Example**: "Reference images for forest scene background and lighting"

**Tags**
- **Purpose**: Keywords for searchability
- **Format**: Multiple tags separated by commas
- **Example**: "forest, trees, background, reference, lighting"

**Source**
- **Purpose**: Where the asset came from
- **Format**: Source information
- **Example**: "Unsplash", "Self-created", "Client provided", "Stock library"

**License**
- **Purpose**: Usage rights and restrictions
- **Format**: License type and permissions
- **Example**: "Creative Commons", "Commercial", "Personal", "Internal use only"

## The Starred Asset System

### What Are Starred Assets?

Starred assets are your most important or frequently used assets. This system helps you quickly access critical resources.

### How to Star an Asset

1. **Click Star Icon**
   - Click the star icon on any asset thumbnail
   - The star turns yellow/gold to indicate it's starred
   - Multiple assets can be starred (unlike shots)

2. **Benefits of Starring**
   - **Quick Access**: Starred assets are easily accessible
   - **Priority Organization**: Focus on most important assets
   - **Workflow Efficiency**: Fast access to frequently used resources
   - **Project Focus**: Clear visual hierarchy of asset importance

### Managing Stars

**Multiple Stars**
- Unlike shots, multiple assets can be starred
- Star as many assets as needed for your workflow
- Use stars to mark priority resources

**Remove Stars**
- Click star again to unstar an asset
- No confirmation required
- Asset remains in the collection

**Filter by Stars**
- Use filter to show only starred assets
- Focus on most important resources
- Quick access to frequently used assets

## Asset Replacement and Updates

### Replacing Assets

1. **Select Asset to Replace**
   - Right-click the asset you want to replace
   - Select **Replace Asset** from context menu

2. **Choose New File**
   - Browse to your new asset file
   - Select the replacement file
   - Click **Replace** to confirm

3. **Verify Replacement**
   - AIMMS will:
     - Backup old asset (if enabled)
     - Replace with new file
     - Preserve metadata
     - Update references

4. **Check Results**
   - Verify the new asset appears correctly
   - Confirm metadata is preserved
   - Test that the asset works as expected

### Updating Asset Metadata

1. **Open Asset Details**
   - Click asset to view details
   - The details panel appears

2. **Edit Information**
   - Click **Edit Details**
   - Make changes to any metadata field
   - Update information as needed

3. **Save Changes**
   - Click **Save** to apply updates
   - Changes are saved immediately
   - Asset information is updated

### Asset Versioning

**Manual Versioning**
- Create multiple assets with version numbers
- Examples: "character_design_v01.pdf", "character_design_v02.pdf"
- Track changes and improvements over time

**Metadata Tracking**
- Use description field for version notes
- Document changes and updates
- Maintain version history in metadata

**Backup System**
- Old versions can be recovered from backups
- Manual backup of important assets
- Version control through naming conventions

## Asset Organization Strategies

### By Project Phase

**Pre-production**
- Reference images and mood boards
- Concept art and storyboards
- Scripts and planning documents
- Location and casting references

**Production**
- Assets actively in use
- Current reference materials
- Working documents and notes
- Communication and coordination files

**Post-production**
- Final assets and deliverables
- Completed reference materials
- Final documentation and reports
- Archive and backup materials

### By Asset Type

**Visual Assets**
- Images, videos, 3D models
- Color palettes and style guides
- Character and location designs
- Storyboard and concept art

**Audio Assets**
- Sound effects and music
- Voiceovers and dialogue
- Ambient sounds and atmospheres
- Audio style references

**Documentation**
- Scripts and screenplays
- Technical documentation
- Research and reference materials
- Communication and notes

### By Usage Frequency

**Frequently Used**
- Star these assets for quick access
- Keep in easily accessible locations
- Use consistent naming for quick identification
- Maintain current and accurate information

**Occasionally Used**
- Standard organization and naming
- Include in regular backups
- Keep metadata up to date
- Organize by category and type

**Archive**
- Old versions and unused assets
- Historical reference materials
- Backup copies and archives
- Legacy project materials

## Asset Quality Control

### File Integrity

**Regular Checks**
- Periodically verify all assets are accessible
- Test audio and video assets
- Check image quality and resolution
- Verify document readability

**Corruption Prevention**
- Use appropriate file formats
- Maintain proper file permissions
- Regular backup and recovery testing
- Monitor file system health

### Metadata Quality

**Completeness**
- Ensure all assets have complete metadata
- Fill in missing information
- Maintain consistent naming conventions
- Use meaningful descriptions and tags

**Accuracy**
- Verify all metadata is accurate
- Update information as needed
- Check source and license information
- Maintain current and relevant data

### License Compliance

**Tracking Usage Rights**
- Document license information for all assets
- Track expiration dates and restrictions
- Maintain license documentation
- Regular review of license terms

**Compliance Monitoring**
- Regular review of asset usage
- Verify compliance with license terms
- Update license information as needed
- Remove assets with expired or invalid licenses

## Troubleshooting Asset Management

### Common Issues

**Assets Not Appearing**
- Check file format is supported
- Verify file isn't corrupted
- Ensure file size is within limits
- Try refreshing the gallery (F5)

**Missing Metadata**
- Check file permissions
- Verify database isn't locked
- Try restarting AIMMS
- Check for software updates

**File Access Issues**
- Install appropriate software for file types
- Check file associations
- Verify files aren't corrupted
- Try opening files outside AIMMS

**Organization Problems**
- Use consistent naming conventions
- Add comprehensive metadata
- Create meaningful categories
- Use tags for additional organization

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

Effective asset management helps you maintain organized, accessible, and well-documented project resources. Use these practices to ensure your assets support your AIMMS workflow efficiently.