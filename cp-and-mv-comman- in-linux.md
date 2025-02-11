#  cp and mv command in linux
In Linux, `cp`, `mv`, are essential commands for file and directory manipulation. Here's a brief explanation of each:

##  cp command 
### 1. `cp` (Copy)
The `cp` command is used to copy files or directories from one location to another.

#### Syntax:
```bash
cp [options] source destination
```

- **Basic example (copy a file):**
  ```bash
  cp file1.txt /path/to/destination/
  ```
  This copies `file1.txt` to the specified destination.

- **Copy a directory (with the `-r` option for recursive):**
  ```bash
  cp -r dir1/ /path/to/destination/
  ```

#### Useful options:
- `-r` or `--recursive`: Copy directories recursively.
- `-i` or `--interactive`: Prompt before overwriting files.
- `-u` or `--update`: Copy only when the source file is newer than the destination file or when the destination file is missing.

##  mv command 
### 2. `mv` (Move/Rename)
The `mv` command is used to move or rename files or directories.

#### Syntax:
```bash
mv [options] source destination
```

- **Move a file:**
  ```bash
  mv file1.txt /path/to/destination/
  ```

- **Rename a file:**
  ```bash
  mv oldname.txt newname.txt
  ```

#### Useful options:
- `-i`: Prompt before overwriting files.
- `-u`: Move only when the source file is newer than the destination file or when the destination file is missing.
- `-v`: Verbose mode, shows what is being done.
