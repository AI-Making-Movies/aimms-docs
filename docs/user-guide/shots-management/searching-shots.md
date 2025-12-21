# Searching Shots

## Overview

The search functionality in AIMMS allows you to quickly find specific shots using various search methods and filters. This guide covers different search techniques, filtering options, and tips for efficient shot discovery.

## Quick Search

### Basic Search

1. **Access Search Box**
   - Locate the search box at the top of the shots table
   - The search box is available in all modules

2. **Enter Search Terms**
   - Type keywords to search across all columns
   - Results update in real-time as you type
   - Use partial words or phrases

3. **Navigate Results**
   - Use **Enter** to cycle through search results
   - Click on any result to select the shot
   - Search highlights matching text

### Search Examples

**By Shot Name**
- Type: `OFFICE`
- Finds: `INT_OFFICE_DAY_001`, `EXT_OFFICE_NIGHT_005`

**By Description**
- Type: `hero`
- Finds: Shots with "hero" in the description

**By Section**
- Type: `act 1`
- Finds: All shots in Act 1 section

**By Location**
- Type: `street`
- Finds: Shots with "street" in location field

## Column-Specific Search

### Using Column Picker

1. **Open Column Picker**
   - Click the **Column Picker** button near the search box
   - A dialog will appear showing available columns

2. **Select Search Columns**
   - Check columns you want to include in search
   - Uncheck columns to exclude from search
   - Common combinations:
     - Shot Name + Description
     - Section + Location
     - All columns for comprehensive search

3. **Apply Search**
   - Click **Apply** to set the column selection
   - Your search will now only include selected columns
   - Results update immediately

### Column-Specific Search Benefits

**Focused Search**
- Search only relevant columns
- Reduce false positives
- Faster search results

**Targeted Results**
- Find shots based on specific criteria
- Combine multiple column searches
- More precise search outcomes

## Section Filtering

### Filter by Section

1. **Access Section Filter**
   - Look for the section dropdown in the status bar
   - Or find section filter controls in the shots module

2. **Select Section**
   - Choose a specific section from the dropdown
   - Options typically include:
     - **All Sections**: Show all shots
     - **Act 1**, **Act 2**, **Act 3**: Story acts
     - **Opening Scene**, **Climax**, **Ending**: Scene types
     - Custom sections you've created

3. **View Filtered Results**
   - Only shots from the selected section appear
   - Filter applies immediately
   - Use "All Sections" to remove filter

### Section Filter Benefits

**Focused Work**
- Work on specific parts of your project
- Reduce visual clutter
- Improve workflow efficiency

**Project Organization**
- Organize shots by narrative structure
- Group related shots together
- Maintain logical project flow

## Advanced Search Techniques

### Boolean Search Operators

**AND Search**
- Type: `office AND day`
- Finds: Shots containing both "office" and "day"

**OR Search**
- Type: `office OR street`
- Finds: Shots containing either "office" or "street"

**NOT Search**
- Type: `office NOT night`
- Finds: Shots with "office" but not "night"

### Wildcard and Pattern Search

**Partial Matches**
- Type: `INT_*`
- Finds: All interior shots (if using consistent naming)

**Character Patterns**
- Use asterisk (*) for multiple characters
- Use question mark (?) for single character
- Example: `EXT_??_DAY_*` finds exterior day shots

### Case Sensitivity

**Case-Insensitive Search**
- AIMMS search is typically case-insensitive
- `office` finds `Office`, `OFFICE`, `office`
- No need to match exact case

## Search Shortcuts and Tips

### Keyboard Shortcuts

**Quick Search**
- **Ctrl+F**: Focus on search box
- **Enter**: Cycle through results
- **Esc**: Clear search and exit

**Navigation**
- **Arrow Keys**: Navigate through search results
- **Home/End**: Jump to first/last result
- **Page Up/Down**: Scroll through results quickly

### Search Efficiency Tips

**Use Specific Terms**
- More specific terms = fewer, more relevant results
- Include unique identifiers when possible
- Avoid very common words

**Combine Search Methods**
- Use search + section filter together
- Apply column picker for focused results
- Use multiple search techniques in combination

**Save Search Combinations**
- Remember effective search combinations
- Document search patterns for your project
- Create search templates for common tasks

## Search Results Management

### Result Highlighting

**Visual Indicators**
- Matching text is highlighted in results
- Selected shots are highlighted in the table
- Search terms are emphasized in details view

**Result Count**
- See total number of matching shots
- Track progress through results
- Monitor search effectiveness

### Working with Results

**Select Multiple Results**
- Use **Ctrl+Click** to select multiple search results
- Apply batch operations to selected shots
- Export or manipulate multiple shots at once

**Save Search Results**
- Export search results to CSV if needed
- Create filtered views for ongoing work
- Document search criteria for future reference

## Troubleshooting Search Issues

### Common Problems

**No Results Found**
- Check spelling of search terms
- Try broader search terms
- Verify search columns include relevant fields
- Check if section filter is too restrictive

**Too Many Results**
- Use more specific search terms
- Apply section filtering
- Use column picker to focus search
- Combine multiple search criteria

**Unexpected Results**
- Review search term interpretation
- Check for partial matches you didn't expect
- Verify column selection in column picker
- Consider case sensitivity issues

### Performance Optimization

**Large Project Handling**
- Use filters to reduce search scope
- Apply section filtering before searching
- Use specific search terms to minimize results
- Consider breaking large projects into smaller ones

**Search Speed**
- Close other applications to free system resources
- Reduce project size if possible
- Use focused search methods
- Regularly maintain project files

## Integration with Other Features

### Search and Batch Operations

**Combine with Selection**
- Search for shots meeting specific criteria
- Select all search results
- Apply batch operations (edit, delete, export)

**Search-Based Workflows**
- Use search to identify shots for specific tasks
- Create work queues based on search results
- Organize workflow around search patterns

### Search and Project Organization

**Organization Through Search**
- Use search to identify organizational issues
- Find shots that need reorganization
- Identify patterns for better project structure

**Search History and Patterns**
- Remember effective search patterns
- Document search strategies for your project
- Create search templates for team members

Mastering search functionality helps you work more efficiently with large shot lists and find exactly what you need quickly. Practice these techniques to become proficient at navigating your AIMMS project.