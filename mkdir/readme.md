# mkdir

*`mkdir` command in Linux allows the user to create directories (also referred to as folders in some operating systems ). <br/>
This command can create multiple directories at once as well as set the permissions for the directories. <br/> 
It is important to note that the user executing this command must have enough permissions to create a directory <br/> 
in the parent directory, or he/she may receive a ‘permission denied’ error.*

## Syntax
```bash 
mkdir [options...] [directories ...]
```

## Options

- `-m` : This -m option is used to set the mode of the directory i.e. permissions such as read, write and execute for the created directory.
- `-p` : This option enables the user to create parent directories as per the requirement. If the directories exist already, no error will be displayed.
- `-v` : This option displays verbose information of each directory that is created.
- `-version` : This option will print the information of the version and exit.
- `--help` : This option will display the information of the mkdir command.
- `-Z` : This option is used to set default SELinux rules on a particular directory at the time of creation.

## Examples

### 1. Create a directory
```bash
mkdir project
```
This command will create a directory named project

### 2. Display help information about the mkdir command
```bash
mkdir --help
```

### 3. Display information about created directories
```bash
mkdir -v project
```

### 4. Set permissions
```bash
mkdir -m a=rwx project
```