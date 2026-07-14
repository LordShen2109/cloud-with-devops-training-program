# Linux Search Operations

This directory contains materials related to Linux search and file finding operations as part of the Cloud with DevOps Training Program.

## Overview

The `linux_search_ops` module focuses on teaching effective search and file discovery techniques in Linux environments. This is a critical skill for DevOps engineers who need to quickly locate files, analyze logs, and manage configurations across systems.

## Directory Contents

- **image2.jpeg** - Informational or instructional image related to Linux search operations

## Key Topics Covered

### Search Commands
- `find` - Search for files by name, type, size, and other attributes
- `grep` - Search text patterns within files
- `locate` - Quick file location using a database
- `which` - Find executable files in the PATH

### Common Use Cases

1. **Finding Files**
   - Search by filename patterns
   - Search by file type and size
   - Search by modification time
   - Search by permissions

2. **Searching File Contents**
   - Pattern matching with grep
   - Case-insensitive searches
   - Search in multiple files
   - Display context around matches

3. **Combining Search Operations**
   - Using pipes with search commands
   - Chaining find and grep
   - Filtering and formatting results

## Learning Outcomes

After completing this module, you should be able to:

- ✓ Use `find` command with various options and predicates
- ✓ Perform efficient text searches using `grep` and related tools
- ✓ Combine multiple search techniques for complex queries
- ✓ Optimize search performance in large file systems
- ✓ Write search patterns and regular expressions

## Practical Examples

### Find all `.log` files modified in the last 7 days
```bash
find /var/log -name "*.log" -mtime -7
```

### Search for a specific error in all config files
```bash
grep -r "ERROR" /etc/ --include="*.conf"
```

### Find large files and sort by size
```bash
find . -type f -size +100M -exec ls -lh {} \; | sort -k5 -h
```

## Prerequisites

- Basic Linux command line knowledge
- Familiarity with file systems and directory structure
- Understanding of basic file permissions

## Additional Resources

- Linux `find` man page: `man find`
- Linux `grep` man page: `man grep`
- Regular Expressions (Regex) guide
- Linux documentation and community forums

## Related Modules

- **linux_file_mgmt** - File management operations and administration
- Other training modules in this program

---

**Last Updated:** 2026

**Difficulty Level:** Beginner to Intermediate

**Estimated Time:** 2-3 hours
