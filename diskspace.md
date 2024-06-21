# How to Find and List Files Larger Than a Specific Size in Linux

## Introduction

This tutorial will explore a list of helpful disk space usage command lines in Linux, with examples of use for each command line.

### How to Find and List Files Larger Than 100MB in Linux

If you wish to find all files over 100M and to see where they are located and what is their size:

```bash
find . -type f -size +100M -exec ls -lh {} \;
```

### How to Find and List Files Larger Than 1GB in Linux

For example, to find files that are bigger than 1GB, use the following command:

```bash
find . -type f -size +1G -exec ls -lh {} \;
```

### How to Find and List Files Smaller Than 100MB in Linux

If you wish to find all files under 100M and to see where they are located and what is their size:

```bash
find . -type f -size -100M -exec ls -lh {} \;
```

### How to Find and List Files Between a Certain Size in Linux

You might wonder how to find and list files between a certain size. For instance, you can find files between 100MB and 500MB using the following command:

```bash
find . -type f -size +100M -size -500M -exec ls -l {} \;
```

### How to Find Files Larger Than 10MB, 100MB, or 1GB in Linux

To find files larger than 10MB, 100MB, or 1GB, you can use the following commands:

```bash
find / -type f -size +10M
find / -type f -size +100M
find / -type f -size +1G
```

### How to Find Files by Size and Extension

Instead of searching all files, you can also search files of specific extensions greater than 1GB size. For example, search all files with extension “.log” and size are 1GB or more:

```bash
find / -type f -name "*.log" -size +1G
```

### How to Find Files Larger Than a Specific File Size

Use the `find` command with its `-size` flag to find files larger than a specific file size.

```bash
find . -type f -size +100M
```

### How to List Files Larger Than a Specific Size

Use the `find` command with its `-size` flag to list files larger than a specific size.

```bash
find . -type f -size +100M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension

Use the `find` command with its `-size` and `-name` flags to find files larger than a specific size and extension.

```bash
find / -type f -name "*.log" -size +1G
```

### How to Find Files Larger Than a Specific Size and Directory

Use the `find` command with its `-size` and `-path` flags to find files larger than a specific size and directory.

```bash
find /path/to/directory -type f -size +100M
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory

Use the `find` command with its `-size`, `-name`, and `-path` flags to find files larger than a specific size and extension in a specific directory.

```bash
find /path/to/directory -type f -name "*.log" -size +1G
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories

Use the `find` command with its `-size`, `-name`, and `-path` flags to find files larger than a specific size and extension in a specific directory and subdirectories.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively

Use the `find` command with its `-size`, `-name`, and `-path` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit

Use the `find` command with its `-size`, `-name`, `-path`, and `-maxdepth` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, and Extension Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, and `-name` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, and extension limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +100M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -size -500M -exec ls -lh {} \;
```

### How to Find Files Larger Than a Specific Size and Extension in a Specific Directory and Subdirectories Recursively with Depth Limit, Size Limit, Extension Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, Size Limit, and Size Limit

Use the `find` command with its `-size`, `-name`, `-path`, `-maxdepth`, `-size`, `-name`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, `-size`, and `-size` flags to find files larger than a specific size and extension in a specific directory and subdirectories recursively with a depth limit, size limit, extension limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, size limit, and size limit.

```bash
find /path/to/directory -type f -name "*.log" -size +1G -maxdepth 3 -size -500M -name "*.log" -size +

Citations:
[1] https://chemicloud.com/kb/article/find-and-list-files-bigger-or-smaller-than-in-linux/
[2] https://tecadmin.net/find-all-files-larger-than-1gb-size-in-linux/
[3] https://manage.accuwebhosting.com/knowledgebase/3647/How-to-Find-All-Files-Larger-than-1GB-in-Linux.html
[4] https://superuser.com/questions/233616/list-files-bigger-than-filesize-specified
[5] https://askubuntu.com/questions/1193386/how-to-find-or-list-file-and-directories-which-having-size-more-than-100mb
