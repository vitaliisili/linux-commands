# find

*The find command in UNIX is a command line utility for walking a file hierarchy. It can be used to find files and <br/> 
directories and perform subsequent operations on them. It supports searching by file, folder, name, creation date,<br/>
modification date, owner and permissions. By using the ‘-exec’ other UNIX commands can be executed on files or folders found. *

## Syntax
```bash
find [where to start searching from] [expression determines what to find] [-options] [what to find]
```

## Options

- `-exec CMD` : The file being searched which meets the above criteria and returns 0 for as its exit status for successful command execution.
- `-ok CMD` :  It works same as -exec except the user is prompted first.
- `-inum N` : Search for files with inode number ‘N’.
- `-links N` : Search for files with ‘N’ links.
- `-name demo` : Search for files that are specified by ‘demo’.
- `-newer file `: Search for files that were modified/created after ‘file’.
- `-perm octal` : Search for the file if permission is ‘octal’.
- `-print` : Display the path name of the files found by using the rest of the criteria.
- `-empty `: Search for empty files and directories.
- `-size +N/-N `: Search for files of ‘N’ blocks; ‘N’ followed by ‘c’ can be used to measure size in characters; ‘+N’ means size > ‘N’ blocks and ‘-N’ means size < ‘N’ blocks.
- `-user name` : Search for files owned by user name or ID ‘name’.
- `\(expr \)`: True if ‘expr’ is true; used for grouping criteria combined with OR or AND.
- `! expr` : True if ‘expr’ is false.

## Examples

### 1. Search a file with specific name.
```bash
find ./GFG -name sample.txt 
```
It will search for sample.txt in GFG directory.

### 2. Search a file with pattern.
```bash
find ./GFG -name *.txt 
```
It will give all files which have ‘.txt’ at the end. 

### 3. Search for empty files and directories.
```bash
find ./GFG -empty
```
This command find all empty folders and files in the entered directory or sub-directories.

### 4. Search for file with entered permissions.
```bash
find ./GFG -perm 664
```
This command find all the files in the GFG directory or sub-directory with the given permissions.
