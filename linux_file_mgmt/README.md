# Linux File Management

This directory contains Linux file management exercises demonstrating basic file operations and commands.

## Overview

This module covers fundamental Linux file management operations including:
- Creating directories with `mkdir`
- Navigating directories with `cd`
- Creating files and using redirects with `cat` and `<<EOF`
- Viewing file contents
- File permissions and ownership
- File manipulation and organization

## Example Commands

The following demonstrates basic file management operations:

```bash
# Create a directory
mkdir linux_file_mgmt

# Navigate into the directory
cd linux_file_mgmt/

# Create a file with multi-line content using heredoc redirect
cat <<EOF>students.txt
Aaryan
Sarthak
Steve Rogers
Robert Downey Junior
EOF

# View file contents
cat students.txt
```

## Files in This Directory

- **students.txt** - Example text file created using file redirection and heredoc syntax

## Key Concepts Demonstrated

- **mkdir**: Create new directories
- **cd**: Change working directory
- **cat**: Display file contents and create files
- **<<EOF**: Heredoc syntax for multi-line input redirection
- **>**: Output redirection to create/overwrite files
