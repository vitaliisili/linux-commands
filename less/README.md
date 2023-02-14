# less

*The `less` command in Ubuntu is a text file viewer, used to view the contents of a file in a terminal window. <br/> 
It allows you to scroll through the file and is often used as a replacement for the more basic `cat` command.*

## Syntax
```bash
less [OPTION]... [FILE]...
```

## Options

- `-E` or `--quit-on-intr`: Exit immediately if an interrupt signal is received.
- `-F` or `--quit-if-one-screen`: Exit immediately if the file can be displayed in one screenful.
- `-I` or `--ignore-case`: Search case-insensitively.
- `-N` or `--line-numbers`: Display line numbers.
- `-R` or `--RAW-control-chars`: Interpret backspaces, tabs and other control characters in raw mode.
- `-S` or `--chop-long-lines`: Chop long lines rather than wrapping them.
- `-X` or `--no-init`: Do not send the terminal initialization string.
- `+<LINE>`: Start at line number <LINE>.
- `+/<PATTERN>`: Start at the first line containing the pattern <PATTERN>.
- `-<NUMBER>`: Start <NUMBER> lines from the end of the file.

## Navigation

Once you have the file open in `less`, you can use the following commands to navigate the file:

- `Up Arrow` and `Down Arrow`: Move up and down one line at a time
- `Page Up` and `Page Down`: Move up and down one page at a time
- `Home` and `End`: Move to the beginning and end of the file, respectively
- `/` followed by a search term: Search for the specified term in the file
- `n`: Repeat the last search
- `q`: Quit `less` and return to the command line

## Examples

### 1. To view a file
```bash
less file.txt
```

### 2. To view a file and start from the line number 100
```bash
less +100 file.txt
```

### 3. To view a file and start from the first line containing the pattern "ERROR"
```bash
less +/ERROR file.txt
```
