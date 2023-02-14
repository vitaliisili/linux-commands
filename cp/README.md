# cp

*The `cp` (Copy) command is used to copy files and directories in a Linux terminal.*

## Syntax
```bash
cp [OPTION]... SOURCE DEST
```

## Options

- `-a` or `--archive`: Equivalent to -dR --preserve=all.
- `-b` or `--backup`: Make a backup of each file that would otherwise be overwritten or lost.
- `-f` or `--force`: If the destination file cannot be opened, remove it and create a new file, without prompting for confirmation, regardless of its permissions.
- `-i` or `--interactive`: Prompt for confirmation before overwriting an existing file.
- `-l` or `--link`: Create a hard link instead of copying the file.
- `-n` or `--no-clobber`: Do not overwrite an existing file.
- `-P` or `--no-dereference`: Do not follow symbolic links.
- `-p` or `--preserve`: Preserve the specified attributes (default: mode, ownership, timestamps).
- `-R` or `--recursive`: Copy directories recursively.
- `-s` or `--symbolic-link`: Create a symbolic link instead of copying the file.
- `-S` or `--suffix`: Append the specified SUFFIX to each backup file made with -b.

## Examples

### 1. To copy a file
```bash
cp file.txt /path/to/destination/
```

### 2. To copy multiple files
```bash
cp file1.txt file2.txt /path/to/destination/
```

### 3. To copy a directory recursively
```bash
cp -R directory/ /path/to/destination/
```

### 4. To copy a file and prompt for confirmation before overwriting
```bash
cp -i file.txt /path/to/destination/
```
