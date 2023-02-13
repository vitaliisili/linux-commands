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