Here is how you can list all files larger than 100MB on Linux:

## Using the `find` command

The `find` command is the most versatile way to search for files based on their size. Here's the command:

```
find / -type f -size +100M -exec ls -lh {} \;
```

Let's break down the command:

- `find /` - Starts the search from the root directory `/`. You can replace this with a specific directory if you only want to search a certain location.
- `-type f` - Specifies that we only want to search for regular files, not directories.
- `-size +100M` - Looks for files larger than 100MB. The `+` sign means "greater than".
- `-exec ls -lh {} \;` - Executes the `ls -lh` command on each file found, displaying the file size in a human-readable format.

This will list all files larger than 100MB along with their sizes and locations.

## Using the `du` command

Another way to find large files is to use the `du` (disk usage) command. Here's an example:

```
du -h --max-depth=1 | sort -hr | head -n 10
```

This command:

- `du -h` - Displays the file/directory sizes in human-readable format (e.g. 100M instead of 104857600).
- `--max-depth=1` - Limits the search to the current directory, not subdirectories.
- `sort -hr` - Sorts the results in descending order by file size.
- `head -n 10` - Displays the top 10 largest files/directories.

This will show you the 10 largest files/directories in the current directory, which can help you identify the biggest space hogs.

## Combining `find` and `du`

You can also combine the `find` and `du` commands to get more detailed information about large files:

```
find / -type f -size +100M -exec du -h {} \; | sort -hr
```

This command:

- `find / -type f -size +100M` - Finds all files larger than 100MB.
- `-exec du -h {} \;` - Runs the `du` command to get the size of each file found.
- `sort -hr` - Sorts the results in descending order by file size.

This will give you a sorted list of all files larger than 100MB along with their sizes.

Remember to adjust the file size threshold (100M in the examples) based on your specific needs. You can use other size units like `k` for kilobytes, `G` for gigabytes, etc.

Citations:
[1] https://unix.stackexchange.com/questions/733884/find-folders-who-have-at-least-two-files-over-100-mb
[2] https://chemicloud.com/kb/article/find-and-list-files-bigger-or-smaller-than-in-linux/
[3] https://askubuntu.com/questions/1193386/how-to-find-or-list-file-and-directories-which-having-size-more-than-100mb
[4] https://superuser.com/questions/233616/list-files-bigger-than-filesize-specified
[5] https://tecadmin.net/find-all-files-larger-than-1gb-size-in-linux/
[6] https://www.tomshardware.com/how-to/find-large-files-linux
[7] https://stackoverflow.com/questions/35447027/linux-command-how-to-find-files-by-size-larger-than-x
[8] https://manage.accuwebhosting.com/knowledgebase/3647/How-to-Find-All-Files-Larger-than-1GB-in-Linux.html
