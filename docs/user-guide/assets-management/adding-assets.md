# Adding Assets

## Overview

Adding assets to your AIMMS project allows you to organize and manage all the supporting materials for your storyboard. This guide covers different methods to add assets, supported file types, and best practices for asset organization.

## Methods to Add Assets

### Method 1: Direct File Addition

1. **Navigate to Assets Module**
   - Click the **Assets** tab or press `Ctrl+4`
   - The asset gallery will display

2. **Add New Asset**
   - Click the **Add Asset** button
   - A file browser dialog will appear

3. **Select Asset File**
   - Browse to your asset file location
   - Select the file
   - Click **Open** to proceed

4. **Configure Asset Details**
   - **Asset Name**: Enter a descriptive name
   - **Category**: Choose appropriate category (references, audio, documents, etc.)
   - **Description**: Add details about what the asset is used for
   - **Tags**: Add keywords for easy searching
   - **Source**: Document where the asset came from
   - **License**: Specify usage rights and permissions

5. **Import Asset**
   - Click **Add** to import the asset
   - AIMMS will copy the file to the project assets folder
   - Asset appears in the gallery

### Method 2: Drag and Drop

1. **Prepare Files**
   - Have your asset files ready
   - Ensure they're in supported formats

2. **Drag to Gallery**
   - Open your file explorer
   - Drag asset files directly onto the assets gallery
   - AIMMS will automatically import them

3. **Add Metadata**
   - After import, click the asset to view details
   - Click **Edit Details** to add metadata
   - Fill in asset information and save

### Method 3: Bulk Import

1. **Access Bulk Import**
   - Click **Import Assets** button
   - Or use File → Import Assets

2. **Select Multiple Files**
   - Browse to your asset files location
   - Select multiple files or entire folders
   - Click **Import** to proceed

3. **Configure Import Settings**
   - Choose default category for imported assets
   - Set default metadata values
   - Configure import options

4. **Complete Import**
   - AIMMS will import all selected files
   - Assets appear in the gallery
   - Add individual metadata as needed

## Supported Asset Types

### Images

**Supported Formats:**
- PNG (recommended for quality)
- JPG/JPEG (smaller file size)
- WebP (modern format, good compression)
- BMP, TIFF (specialized formats)

**File Size Limits:**
- Maximum: 100MB per file
- Recommended: Under 50MB for optimal performance

**Best Uses:**
- Reference images and mood boards
- Location photos and concept art
- Character designs and storyboards
- Color palettes and style guides

### Audio

**Supported Formats:**
- MP3 (widely compatible)
- WAV (high quality, large files)
- FLAC (lossless compression)
- OGG, AAC (modern formats)

**File Size Limits:**
- Maximum: 500MB per file
- Recommended: Under 100MB for optimal performance

**Best Uses:**
- Sound effects and ambient audio
- Music references and mood tracks
- Voiceovers and dialogue samples
- Audio style references

### Documents

**Supported Formats:**
- PDF (universal document format)
- DOC, DOCX (Microsoft Word)
- TXT (plain text)
- RTF (rich text format)

**File Size Limits:**
- Maximum: 50MB per file
- Recommended: Under 10MB for optimal performance

**Best Uses:**
- Scripts and screenplays
- Storyboards and shot lists
- Technical documentation
- Research and reference materials

### 3D and Technical

**Supported Formats:**
- OBJ (3D model format)
- FBX (Autodesk format)
- STL (3D printing format)
- GLTF (modern 3D format)

**File Size Limits:**
- Maximum: 1GB per file
- Recommended: Under 500MB for optimal performance

**Best Uses:**
- 3D model references
- Technical specifications
- Animation references
- Lighting and texture references

## Asset Organization

### Category Management

**Default Categories:**
- **References**: Mood boards, location photos, character designs
- **Audio**: Sound effects, music, voiceovers
- **Documents**: Scripts, storyboards, technical docs
- **3D Models**: 3D models, textures, technical files

**Custom Categories:**
- Create custom categories for your project
- Use project-specific category names
- Organize by workflow stage or asset type

### Naming Conventions

**Descriptive Names:**
- Use clear, descriptive names
- Include key identifying information
- Examples:
  - "forest_background_v01.jpg"
  - "character_design_main.pdf"
  - "sound_effect_door_open.wav"

**Version Numbers:**
- Include version numbers when applicable
- Use consistent versioning format
- Examples: "v01", "v02", "final", "draft"

**Consistency:**
- Use consistent naming across all assets
- Avoid special characters and spaces
- Use underscores or hyphens for separation

## Asset Metadata

### Required Information

**Asset Name**
- **Purpose**: Unique identifier for the asset
- **Format**: Clear, descriptive name
- **Example**: "Forest Background Reference"

**Category**
- **Purpose**: Asset type classification
- **Options**: References, Audio, Documents, 3D Models, etc.
- **Usage**: Organization and filtering

### Optional Information

**Description**
- **Purpose**: What the asset contains and how it's used
- **Format**: Detailed explanation
- **Example**: "Reference images for forest scene background"

**Tags**
- **Purpose**: Keywords for searchability
- **Format**: Comma-separated keywords
- **Example**: "forest, trees, background, reference"

**Source**
- **Purpose**: Where the asset came from
- **Format**: Source information
- **Example**: "Unsplash", "Self-created", "Client provided"

**License**
- **Purpose**: Usage rights and permissions
- **Format**: License type and restrictions
- **Example**: "Creative Commons", "Commercial", "Internal use"

## Best Practices for Adding Assets

### File Preparation

**File Organization**
- Organize files before importing
- Use consistent folder structures
- Rename files with descriptive names

**File Quality**
- Use appropriate file formats
- Balance quality with file size
- Optimize files for web use when possible

**File Naming**
- Use consistent naming conventions
- Include version numbers when needed
- Avoid special characters and spaces

### Metadata Quality

**Complete Information**
- Fill in all relevant metadata fields
- Provide detailed descriptions
- Use meaningful tags and keywords

**Consistency**
- Use consistent terminology
- Follow established naming conventions
- Maintain category standards

**Accuracy**
- Ensure all information is accurate
- Verify source and license information
- Keep metadata up to date

### Organization Strategies

**Logical Grouping**
- Group related assets together
- Use consistent categories
- Create meaningful folder structures

**Searchability**
- Use descriptive names and tags
- Include relevant keywords
- Make assets easy to find

**Accessibility**
- Ensure files are accessible and readable
- Use appropriate file formats
- Maintain file integrity

## Troubleshooting Asset Addition

### Common Issues

**File Not Supported**
- **Problem**: File format not recognized
- **Solution**: Convert to supported format
- **Prevention**: Check format compatibility before import

**File Too Large**
- **Problem**: File exceeds size limits
- **Solution**: Compress or resize the file
- **Prevention**: Check size limits for each format

**Import Failed**
- **Problem**: Asset doesn't appear after import
- **Solution**: Check file permissions and path
- **Prevention**: Ensure files are accessible

### Error Resolution

**File System Errors**
- **Problem**: Cannot access or copy file
- **Solution**: Check file permissions and disk space
- **Prevention**: Ensure proper file system access

**Database Errors**
- **Problem**: Asset information not saved
- **Solution**: Run database validation and repair
- **Prevention**: Ensure database integrity

**Corruption Issues**
- **Problem**: Imported file is corrupted
- **Solution**: Re-import from original source
- **Prevention**: Verify file integrity before import

## Integration with Other Modules

### Linking to Shots

**Asset References**
- Link assets to specific shots
- Use in shot descriptions and prompts
- Cross-module navigation for related content

**Workflow Integration**
- Use assets in image/video generation
- Reference assets in shot planning
- Maintain consistent asset-shot relationships

### Project Organization

**Consistent Naming**
- Use consistent naming across modules
- Maintain organized file structure
- Document asset usage and relationships

**Metadata Standards**
- Apply consistent metadata practices
- Use standardized categories and tags
- Maintain quality documentation

Adding assets effectively helps you maintain organized, accessible, and well-documented project resources. Use these guidelines to ensure your assets are properly integrated into your AIMMS workflow.