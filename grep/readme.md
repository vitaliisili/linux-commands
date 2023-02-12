# grep

*The `grep` command is used for searching and filtering text in Linux. It stands for <br/> 
"global regular expression print" and is used to search for a specific pattern in a <br/> file or input from the command line.*

## Syntax
```bash
grep [OPTIONS] PATTERN [FILE...]
```

Where `PATTERN` is the string or regular expression you want to search for, <br/> 
and `FILE` is the file or files you want to search in. The `OPTIONS` are optional <br/> 
flags that modify the behavior of the grep command.

## Options

- `-i`: Ignore case.
- `-v`: Invert the match, showing lines that do not match the pattern.
- `-r` or `--recursive`: Recursively search all files in a directory and its subdirectories.
- `-n` or `--line-number`: Show the line numbers of the matching lines.
- `-c` or `--count`: Only show the count of the number of matching lines, not the lines themselves.
- `-w` or `--word-regexp`: Only match complete words, not substrings.
- `-E` or `--extended-regexp`: Interpret the pattern as an extended regular expression.
- `-F` or `--fixed-strings`: Interpret the pattern as a list of fixed strings, separated by newlines.
- `-x` or `--line-regexp`: Only match lines that match the entire pattern.
- `-l` or `--files-with-matches`: Only show the names of files that contain matching lines, not the lines themselves.
- `-L` or `--files-without-match`: Only show the names of files that do not contain matching lines.

## Examples

### 1. Search for a specific word in a file
```bash
grep "word" file.txt
```

### 2. Search for a pattern in multiple files
```bash
grep "pattern" file1.txt file2.txt file3.txt
```

### 3. Search for a pattern in all files in a directory
```bash
grep "pattern" /path/to/directory/*
```

### 4. Search for a pattern in all files in a directory and its subdirectories
```bash
grep -r "pattern" /path/to/directory
```

### 5. Search for a pattern in a file, ignoring case
```bash
grep -i "pattern" file.txt
```

### 6. Search for a pattern using an extended regular expression
```bash
grep -E "pattern" file.txt
```