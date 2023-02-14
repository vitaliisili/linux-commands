# man

The `man` command provides a user manual of any command or utility that you can run inside terminal, including the name, description, and options.

It consists of nine sections:

- Executable programs or shell commands
- System calls
- Library calls
- Games
- Special files
- File formats and conventions
- System administration commands
- Kernel routines
- Miscellaneous

## Syntax

To display the complete manual, enter:
```bash
man [command_name]
```

## Options

- `-a`: Display all available manual pages for the specified command.
- `-C` `FILE`: Use the specified configuration file instead of the default one.
- `-f`: Equivalent to whatis.
- `-k` `KEYWORD`: Search the manual page names and descriptions for the specified `KEYWORD`.
- `-w`: Equivalent to whereis.
- `-P` `PAGER`: Use the specified pager program instead of the default one.
- `-t`: Format the man page as PostScript.

## Examples

For example, you want to access the manual for the `ls` command:
```bash
man ls
```
Enter this command if you want to specify the displayed section:
```bash
man [option] [section_number] [command_name]
```
For instance, you want to see section 2 of the `ls` command manual:
```bash
man 2 ls
```