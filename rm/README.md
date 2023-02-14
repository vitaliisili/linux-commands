# rm

*The `rm` command is used to remove files and directories in Linux.*

## Syntax
```bash
rm [OPTION]... FILE...
```

## Options

- `-f`: Force remove, ignore nonexistent files and never prompt for confirmation.
- `-i`: Interactive mode, prompt for confirmation before removing files.
- `-r` or `-R`: Recursive, remove directories and their contents recursively.
- `--`: Treat all arguments after this option as file names, even if they start with a dash (-).

## Examples

### 1. Remove a single file
```bash
rm file.txt
```

### 2. Remove multiple files:
```bash
rm file1.txt file2.txt file3.txt
```

### 3. Remove a directory and its contents
```bash
rm -r directory/
```