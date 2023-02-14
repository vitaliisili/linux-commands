# cat

*The `cat` command is a utility command in Linux. One of its most common usages is to print the content of a file onto <br/>
the standard output stream. Other than that, the cat command also allows us to write some texts into a file.*

## Syntax
```bash
cat [OPTION]... [FILE]...
```

## Options
- `-A`  or `--show-all` : Equivalent to -vET.
- `-b`  or `--number-nonblank` : Number the non-empty output lines, starting at 1.
- `-e` : Equivalent to `-vE`.
- `-E`  or `--show-ends`: Display a $ character at the end of each line.
- `-n`  or `--number`: Number all output lines, starting at 1.
- `-s`  or `--squeeze-blank`: Suppress repeated empty output lines.
- `-t` : Equivalent to `-vT`.
- `-T`  or `--show-tabs`: Display TAB characters as ^I.
- `-u` : Ignored.
- `-v`  or `--show-nonprinting`: Display non-printable characters (see the LC_CTYPE category in the locale(7) manual page) in a visible form.

## Examples

### 1. To display the contents of a file
```bash
cat file.txt
```

### 2. To display the contents of multiple files
```bash
cat file1.txt file2.txt
```

### 3. To concatenate and display the contents of multiple files
```bash
cat file1.txt file2.txt > output.txt
```

### 4. To display the contents of a file with line numbers
```bash
cat -n file.txt
```