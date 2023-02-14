# mv

*The `mv` command is used to move or rename files and directories in Linux.*

## Syntax
```bash
mv [OPTION]... SOURCE DEST
```

## Options

- `-b`: Make a backup of each file that would otherwise be overwritten or deleted.
- `-f`: Force move, overwrite existing destination files.
- `-i`: Interactive, prompt before overwriting existing destination files.
- `-n`: Do not overwrite existing files.
- `-u`: Move only when the SOURCE file is newer than the destination file or when the destination file is missing.
- `-v`: Verbose, print the name of each file before moving it.

## Examples

### 1. To move a file named file.txt to a directory named docs
```bash
mv file.txt docs/
```

### 2. To rename a file named oldfile.txt to newfile.txt
```bash
mv oldfile.txt newfile.txt
```

### 3. To move a file named file.txt to a directory named docs and overwrite the existing file:
```bash
mv -f file.txt docs/
```
