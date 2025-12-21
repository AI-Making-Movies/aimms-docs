# Importing Shots

## Overview

Importing shots allows you to bring existing shot lists into AIMMS from external sources like spreadsheets or other storyboard tools. This guide covers the CSV import process, file format requirements, and best practices for successful imports.

## When to Use Import

### Common Use Cases

**Moving from Other Tools**
- Transitioning from spreadsheets (Excel, Google Sheets)
- Migrating from other storyboard applications
- Consolidating shot lists from multiple sources

**Collaboration**
- Receiving shot lists from team members
- Integrating client-provided shot information
- Sharing shot data between projects

**Project Setup**
- Bulk shot creation for large projects
- Setting up template projects
- Creating initial project structure

**Backup and Recovery**
- Restoring shots from CSV backups
- Recovering data from corrupted projects
- Merging shot lists from different sources

## CSV Import Format

### Required Columns

Your CSV file must include these columns (order doesn't matter):

```csv
order_number,shot_name,section,description,image_prompt,colour_scheme_image,time_of_day,location,country,year,video_prompt
```

### Column Descriptions

| Column | Description | Example |
|--------|-------------|---------|
| **order_number** | Sequence position of the shot | 1, 2, 3, 10 |
| **shot_name** | Descriptive name for the shot | INT_OFFICE_DAY_001 |
| **section** | Group the shot belongs to | Act 1, Opening Scene |
| **description** | Brief description of the shot | Hero enters office |
| **image_prompt** | AI prompt for generating base image | A man sitting at a desk |
| **colour_scheme_image** | Color palette for the shot | Warm tones |
| **time_of_day** | When the shot takes place | Day, Night, Dawn |
| **location** | Where the shot takes place | Office, Street, Home |
| **country** | Country setting for the shot | USA, France, Japan |
| **year** | Time period for the shot | 2024, 1980s, Future |
| **video_prompt** | AI prompt for generating final video | A man walks into an office |

### CSV File Requirements

**File Format**
- **Encoding**: UTF-8 encoding
- **Delimiter**: Comma-separated values
- **Text Qualifier**: Use double quotes for text containing commas
- **Line Endings**: Standard line endings (LF or CRLF)

**Data Format**
- **Headers**: First row must contain column headers
- **No Empty Rows**: Remove empty rows from the file
- **Consistent Format**: Use consistent formatting throughout
- **Valid Data**: Ensure all required fields have valid data

### Example CSV File

```csv
order_number,shot_name,section,description,image_prompt,colour_scheme_image,time_of_day,location,country,year,video_prompt
1,INT_OFFICE_DAY_001,Act 1,Hero enters office,A man sitting at a desk,Warm tones,Day,Office,USA,2024,A man walks into an office
2,EXT_STREET_NIGHT_002,Act 1,Villain on street,A dark figure in shadows,Cold tones,Night,Street,USA,2024,A figure walks down a dark street
3,INT_CAR_DAY_003,Act 2,Car chase scene,Two cars racing through city,Bright colors,Day,City,USA,2024,Cars speeding through city streets
```

## Import Process

### Step 1: Prepare Your CSV File

1. **Create or Export CSV**
   - Export from your spreadsheet application
   - Ensure proper column headers
   - Verify data accuracy and completeness

2. **Validate Format**
   - Check that all required columns are present
   - Verify data format matches requirements
   - Remove any empty rows or invalid data

3. **Save File**
   - Save as CSV format with UTF-8 encoding
   - Use a descriptive filename
   - Store in an accessible location

### Step 2: Import the CSV File

1. **Access Import Function**
   - Click **File** → **Import CSV**
   - Or use the import button in the shots module

2. **Select File**
   - Browse to your CSV file location
   - Select the file
   - Click **Open** to begin import

3. **Validation Process**
   - AIMMS will validate the file format
   - Check for required columns and data
   - Identify any potential issues

### Step 3: Review Import Summary

1. **Validation Results**
   - Review validation summary
   - Check for any errors or warnings
   - Address any issues identified

2. **Import Summary**
   - See how many shots will be imported
   - Review any data that couldn't be imported
   - Confirm import settings

3. **Proceed with Import**
   - Click **Import** to proceed
   - Wait for import to complete
   - Verify shots appear in your project

## Import Validation

### Automatic Checks

**File Format Validation**
- **Required Columns**: Ensures all necessary columns are present
- **Header Row**: Verifies first row contains headers
- **Data Format**: Checks data types and formats
- **Encoding**: Validates UTF-8 encoding

**Data Quality Checks**
- **Shot Names**: Verifies shot names aren't too long (max 50 characters)
- **Empty Fields**: Identifies missing required information
- **Duplicate Names**: Warns about potential duplicate shot names
- **Order Numbers**: Validates numeric format for sequence numbers

### Error Handling

**Validation Failures**
- **Clear Messages**: Specific error messages for each issue
- **Line Numbers**: Identifies problematic rows
- **Column Information**: Shows which columns have issues
- **Fix Suggestions**: Provides guidance on how to fix problems

**Partial Import**
- **Continue Option**: Import valid shots even if some fail
- **Error Log**: Detailed log of failed entries
- **Manual Review**: Option to review and fix before re-import

## Best Practices

### File Preparation

**Data Consistency**
- Use consistent naming conventions
- Standardize date and time formats
- Maintain consistent terminology
- Avoid special characters in shot names

**Data Completeness**
- Fill in all required fields
- Provide complete descriptions
- Include relevant metadata
- Use specific, actionable prompts

**File Organization**
- Use clear, descriptive column headers
- Organize data logically
- Remove unnecessary columns
- Keep file size reasonable

### Import Strategy

**Test Import**
- Start with a small test import
- Verify data appears correctly
- Check for any unexpected behavior
- Confirm import settings are correct

**Batch Processing**
- Import in manageable batches for large files
- Monitor import progress
- Check results after each batch
- Address issues before continuing

**Backup and Recovery**
- Export current data before import
- Keep original CSV files as backup
- Document import process and results
- Have recovery plan if import fails

## Troubleshooting Import Issues

### Common Problems

**File Format Errors**
- **Problem**: CSV file won't import
- **Solution**: Check file encoding and format
- **Prevention**: Use proper CSV export settings

**Data Validation Failures**
- **Problem**: Shots fail validation
- **Solution**: Review error messages and fix data
- **Prevention**: Validate data before import

**Missing Data**
- **Problem**: Required fields are empty
- **Solution**: Fill in missing information
- **Prevention**: Review data completeness before export

### Advanced Issues

**Large File Handling**
- **Problem**: Very large CSV files cause issues
- **Solution**: Split into smaller files or batches
- **Prevention**: Plan import strategy for large datasets

**Encoding Problems**
- **Problem**: Special characters don't import correctly
- **Solution**: Ensure UTF-8 encoding
- **Prevention**: Test with files containing special characters

**Data Conflicts**
- **Problem**: Import conflicts with existing data
- **Solution**: Review existing shots and plan accordingly
- **Prevention**: Check for duplicates before import

## Post-Import Tasks

### Verification

**Data Review**
- Check that all shots imported correctly
- Verify shot information is accurate
- Confirm shot order and organization
- Review any error messages or warnings

**Media Integration**
- Link imported shots to existing media if applicable
- Update shot information based on media availability
- Organize shots by section and sequence

**Project Organization**
- Review project structure after import
- Adjust sections and organization as needed
- Update project settings if required

### Cleanup

**File Management**
- Remove temporary CSV files
- Document import process and results
- Update project documentation
- Backup project after successful import

**Data Quality**
- Review and clean up any inconsistent data
- Standardize naming and formatting
- Update metadata as needed
- Verify data integrity

Importing shots efficiently requires careful preparation and validation. Follow these guidelines to ensure successful data migration into your AIMMS project.