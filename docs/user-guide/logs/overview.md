# Logs Viewer Overview

## Introduction

The Logs Viewer module provides comprehensive logging and monitoring for your AIMMS project. This module helps you track project activity, troubleshoot issues, and maintain a record of all operations performed in your project.

## Understanding the Logging System

### Log Types and Categories

AIMMS maintains several types of logs to track different aspects of project activity:

**Project Activity Logs:**
- Shot creation, editing, and deletion
- Image and video take management
- Asset additions and modifications
- Project settings changes
- User actions and operations

**System Logs:**
- Application startup and shutdown
- Database operations and errors
- File system operations
- Memory and performance events
- Theme and interface changes

**Error Logs:**
- Application errors and exceptions
- Database connection issues
- File access problems
- Import/export failures
- Validation errors

**Validation Logs:**
- Project validation results
- Data integrity checks
- Migration compatibility reports
- Backup and recovery operations

### Log Levels

Logs are categorized by severity levels:

| Level | Description | When Used |
|-------|-------------|-----------|
| **INFO** | Informational messages | Normal operations, successful actions |
| **WARNING** | Potential issues | Non-critical problems, deprecated features |
| **ERROR** | Error conditions | Failed operations, system problems |
| **SUCCESS** | Successful operations | Completed tasks, positive outcomes |

## Key Features

### Log Viewing and Navigation

**Main Log Display**
- Logs displayed in a scrollable list
- Real-time updates as new logs are generated
- Search and filter capabilities
- Export options for analysis

**Log Entry Format**
```
2025-12-21T14:30:45.123Z [INFO] Module: Description of the event
```

**Components:**
- **Timestamp**: UTC timestamp of the event
- **Level**: Log level (INFO, WARNING, ERROR, SUCCESS)
- **Module**: Which part of AIMMS generated the log
- **Message**: Description of what happened

### Log Categories

**Recent Logs**
- Last 20 entries from all sources
- Quick overview of recent activity
- Real-time updates as new logs are generated

**Project Activity**
- Shot management operations
- Media file operations
- Asset management
- User interactions

**System Events**
- Application lifecycle events
- Database operations
- File system changes
- Performance metrics

**Errors and Warnings**
- Error conditions and failures
- Warning messages
- Validation issues
- System problems

## Filtering and Searching

### Time-Based Filtering

Filter logs by time period:
- **Last Hour**: View logs from the past 60 minutes
- **Last 24 Hours**: View logs from the past day
- **Last 7 Days**: View logs from the past week
- **Custom Range**: Select specific start and end dates

### Content Filtering

**Text Search**
- Type keywords in the search box
- Filter logs containing specific text
- Case-insensitive matching
- Real-time filtering as you type

**Module Filtering**
- Filter by specific modules (Shots, Images, Videos, etc.)
- Focus on particular areas of interest
- Isolate issues to specific functionality

**Level Filtering**
- Show only specific log levels
- Filter out INFO messages to focus on errors
- View only warnings or errors

### Advanced Search

**Regular Expression Support**
- Use regex patterns for complex searches
- Match patterns in log messages
- Advanced filtering capabilities

**Multiple Criteria**
- Combine time, text, and level filters
- Create complex search queries
- Save frequently used filter combinations

## Log File Management

### Log File Locations

AIMMS stores logs in the project's `logs/` directory:

```
project_root/
├── logs/
│   ├── project_log.log          # Main project activity log
│   ├── validation.log          # Validation and migration logs
│   ├── system.log              # System and application logs
│   ├── error.log               # Error-specific logs
│   └── backup/
│       ├── project_log_20251221_143045.txt
│       └── validation_20251221_143045.txt
```

### Log Rotation

**Automatic Rotation**
- Files rotate when they exceed 5MB
- Old files are moved to backup folder
- Timestamped backup files for easy identification
- Maximum of 5 backup files kept

**Manual Rotation**
- Force log rotation when needed
- Clear current log files
- Create new log files immediately

### External Log Viewing

**Open in External Editor**
- Click **Open Log File** to view in system editor
- Use preferred text editor for detailed analysis
- Access full log file content

**Export Logs**
- Export specific log sections
- Save logs for support requests
- Create log reports for analysis

## Using Logs for Troubleshooting

### Identifying Issues

**Error Pattern Recognition**
- Look for ERROR level messages
- Identify recurring error patterns
- Note timestamps of problematic operations

**Warning Analysis**
- Review WARNING messages for potential issues
- Address warnings before they become errors
- Monitor deprecated feature usage

**Performance Monitoring**
- Watch for slow operation warnings
- Identify memory usage patterns
- Track database performance

### Common Log Patterns

**Database Issues:**
```
[ERROR] Database: Connection failed
[WARNING] Database: Slow query detected
[ERROR] Database: Table corruption detected
```

**File System Problems:**
```
[ERROR] File System: Permission denied
[WARNING] File System: Disk space low
[ERROR] File System: File not found
```

**Import/Export Failures:**
```
[ERROR] Import: CSV validation failed
[WARNING] Export: Some records skipped
[ERROR] Import: Database constraint violation
```

### Log Analysis Techniques

**Timeline Analysis**
- Correlate errors with user actions
- Identify sequences of related events
- Track issue progression over time

**Module Isolation**
- Focus on specific module logs
- Isolate issues to particular functionality
- Test fixes by monitoring relevant logs

**Trend Analysis**
- Look for increasing error rates
- Monitor performance degradation
- Identify usage patterns

## Log Configuration

### Log Settings

Configure logging behavior in Project Settings:

**Log Level:**
- **INFO**: All messages (recommended for troubleshooting)
- **WARNING**: Only warnings and errors
- **ERROR**: Only error messages
- **QUIET**: Minimal logging (for performance)

**Log Retention:**
- Maximum log file size before rotation
- Number of backup files to keep
- Automatic cleanup settings

**Log Format:**
- Timestamp format options
- Include/exclude module information
- Custom log message formatting

### Custom Logging

**User-Generated Logs**
- Add custom log entries through the interface
- Document manual operations
- Create audit trails for important changes

**Event Logging**
- Configure which events are logged
- Set logging frequency
- Customize log message content

## Integration with Other Modules

### Project Recovery

Logs support project recovery operations:
- **Recovery Analysis**: Review logs before recovery operations
- **Corruption Patterns**: Identify corruption patterns
- **Recovery Strategy**: Plan recovery strategy based on log history

### Validation Integration

Logs work with the validation system:
- **Validation Reports**: View detailed validation results
- **History Tracking**: Track validation history
- **Health Monitoring**: Monitor project health over time

### Performance Monitoring

Use logs for performance analysis:
- **Operation Timing**: Track operation durations
- **Bottleneck Identification**: Identify performance bottlenecks
- **Resource Usage**: Monitor system resource usage

## Best Practices

### Log Management

**Regular Review**
- Check logs weekly for issues
- Address warnings before they become errors
- Monitor system performance trends

**Log Cleanup**
- Regularly clean up old log files
- Maintain reasonable log file sizes
- Archive important logs for long-term storage

**Documentation**
- Document recurring issues and solutions
- Create troubleshooting guides based on logs
- Share log analysis techniques with team

### Troubleshooting Workflow

**Issue Identification**
1. Reproduce the issue
2. Check recent logs for error patterns
3. Identify the module causing problems
4. Analyze error context and timing

**Problem Resolution**
1. Use logs to understand the root cause
2. Implement fixes based on log analysis
3. Monitor logs to verify fix effectiveness
4. Document the solution for future reference

**Prevention**
1. Monitor warning patterns
2. Address performance degradation early
3. Implement preventive measures
4. Regular system maintenance

The Logs Viewer module is essential for maintaining a healthy, well-monitored AIMMS project. Regular use of this module helps ensure optimal performance and quick issue resolution.