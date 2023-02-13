# The `chmod` Command

The `chmod` command in Ubuntu is used to change the permissions on files and directories. It allows you to specify who can read, write, and execute the file, and is commonly used to make a file executable.

## Usage

To use the `chmod` command, simply type `chmod` followed by the permission settings and the name of the file or directory you want to modify:


## Permission Settings

Permission settings in `chmod` are specified as a three-digit number, where each digit represents the permissions for the owner, group, and other users, respectively. The following table shows the most commonly used permission settings:

| Number | Permissions |
| ------ | ----------- |
| 7      | rwx         |
| 6      | rw-         |
| 5      | r-x         |
| 4      | r--         |
| 3      | -wx         |
| 2      | -w-         |
| 1      | --x         |
| 0      | ---         |

For example, a permission setting of `755` would allow the owner to read, write, and execute the file, while the group and other users would only have the ability to read and execute the file.

## Recursive Option

To modify the permissions of all files and directories within a directory, you can use the `-R` or `--recursive` option:
