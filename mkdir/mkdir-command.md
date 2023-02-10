# mkdir

*mkdir command in Linux allows the user to create directories (also referred to as folders in some operating systems ). <br/>
This command can create multiple directories at once as well as set the permissions for the directories. <br/> 
It is important to note that the user executing this command must have enough permissions to create a directory <br/> in the parent directory, or he/she may receive a ‘permission denied’ error.*

### Syntax
#### *mkdir [options...] [directories ...]*

## Options

- `-m` : This -m option is used to set the mode of the directory i.e. permissions such as read, write and execute for the created directory.
- `-p` : This option enables the user to create parent directories as per the requirement. If the directories exist already, no error will be displayed.
- `-v` : This option displays verbose information of each directory that is created.
- `-version` : This option will print the information of the version and exit.
- `--help` : This option will display the information of the mkdir command.
- `-Z` : This option is used to set defaul SELinux rules on a particular directory at the time of creation.