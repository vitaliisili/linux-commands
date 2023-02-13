# touch

The `touch` command is a useful tool for creating empty files that any Linux user should know. <br/> 

Running the `touch` command inside the terminal session without any additional options, a new file or multiple files will be created under the name(s) and extension(s) of the argument provided along with the command. If the file already exists `touch` will change the file last access and modification times to the current time.

It's a very good way to populate a new code project with empty files while also being visible in logs as a file-creation moment.

## Syntax
```bash
$ touch [ OPTIONS ] filename(s)
```

## Additional Options

`-a` : option to change only the file’s *access* time<br/>
`-m` : option to change only the file’s *modify* time<br/>
`-d` : create a file with a specific time other than the current time<br/>
`--help` : displays the commands help page and exit<br/>
`--version` :  outputs version information and exit<br/>

## Examples

### 1. Create an empty new file with the name "test.txt"

```bash
$ touch test.txt
```

### 2. Create multiple files

```bash
$ touch test.txt test1.doc test2.pdf
```
### 3. Update the timestamps of an existing file to the current time

```bash
$ touch existing_file.*
```

### 4. Create a file with a specific time (date enclosed in single quotes)

```bash
$ touch -d '13 February 2023 20:20' file1
```


###