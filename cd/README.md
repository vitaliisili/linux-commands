# cd
*The `cd` command in linux known as change directory command. It is used to change current working directory.*

## Syntax
```bash
cd [OPTION] [DIRECTORY]
```

## Options

- `-L` : Follow symbolic links, even if the current shell is in symlinks, a mode in which symbolic links are not followed.
- `-P` : Do not follow symbolic links, even if the current shell is not in symlinks mode.
- `--` : End option processing. The rest of the arguments are treated as the name of the directory to change to.

## Examples

### 1. To change to the home directory
```bash
cd
```

### 2. To change to a specific directory
```bash
cd /path/to/directory
```

### 3. To change to the previous directory
```bash
cd -
```

### 4. To change to the parent directory
```bash
cd ..
```
