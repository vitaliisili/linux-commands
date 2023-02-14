# chmod

*The `chmod` command in Ubuntu is used to change the permissions on files and directories. It allows you to specify who can read, write, and execute the file, and is commonly used to make a file executable.*

## Usage

To use the `chmod` command, simply type `chmod` followed by the permission settings and the name of the file or directory you want to modify

## Syntax

```bash
chmod u+rwx,g+rw,o+r file.txt
```

## Options

- Adds executable permission to a file for all users:

```bash
`chmod +x file
```

- Removes executable permission from a file for all users:

```bash
`chmod -x file
```

- Adds executable permission to a file for the owner:

```bash
`chmod u+x file
```

- Adds executable permission to a file for the group:
```bash
`chmod g+x file
```

- Adds executable permission to a file for all other users:
```bash
`chmod o+x file
```

- Adds executable permission to a file for all users:
```bash
`chmod a+x file
```

- Sets the file permissions to read, write, and execute for the owner, read and write for the group, and read only for others:

```bash
`chmod u=rwx,g=rw,o=r file
```

- Recursively sets the file permissions of a directory and its contents to read and write for the owner and group, and read for others:

```bash
`chmod -R u+rwX,g+rwX,o+rX directory
```

## Examples

- Make a file executable for all users:

```bash
`chmod +x script.sh
```

- Make a directory and its contents readable and writable by the owner and group, and readable by others:

```bash
`chmod -R u+rw,g+rw,o+r mydirectory
```

- Give a specific user read and write access to a file:

```bash
`chmod u+rw file.txt
```

- Remove execute permission for all users from a file:

```bash
`chmod a-x script.sh
```

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

To modify the permissions of all files and directories within a directory, you can use:

```bash
`-R` or `--recursive` option
```
