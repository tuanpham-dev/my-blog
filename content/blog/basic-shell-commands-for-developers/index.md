---
title: Essential Shell Commands for Developers
date: "2020-06-24 12:54:00"
description: "Unix-based environments are getting more popular among developers. Even Windows is now supporting Linux with WSL. If you are new to Linux or want to switch to Linux Terminal. Here are essential commands you need to know. They apply to the macOS command line too."
---

Unix-based environments are getting more popular among developers.
Even Windows is now supporting Linux with WSL. If you are new to Linux or want to switch to Linux Terminal.
Here are essential commands you need to know. They apply to the macOS command line too.

## ls (list)

This command lists files and directories in current directory or in given directories.

```bash
# List files in current directory
ls

# List all files (including hidden files)
ls -a

# List files with details
ls -l

# List files in $(pwd)/src and /etc
ls src /etc
```

## cd (change directory)

We use this command to change to home directory or to given directoy (relative or absolute).

```bash
# Change directory to home
cd ~
# or even
cd

# Change directory to $(pwd)/src
cd src

# Change to parent directory
cd ..
```

## mkdir (make directory)

This command is used to create directories.

```bash
# Create src directory
mkdir src

# Create src/components directory if src haven't created
mkdir -p src/components

# Create components, pages and templates directories
mkdir components pages templates
```

## touch

We usually use this command to create empty files

```bash
# Create index.html
touch index.html

# Create index.ts and index.css
touch index.ts index.css
```

## cat

This prints content of a file.

```bash
cat index.ts
```

## head/tail

If file is too large and we only want to see part of that file, head and tail are your friends.

```bash
# Print first 10 lines of index.ts
head index.ts

# Watch and print 100 last lines of /var/log/auth.log
tail -f /var/log/auth.log -n 100
```

## cp (copy)

This copies files or directories to another directory

```bash
cp *.png assets/images
```

## mv (move)

This moves file or directories to another directory. It also can be used to rename file.

```bash
# Rename posts.ts to blog-posts.ts
mv posts.ts blog-posts.ts
```

## rm (remove)

This command removes files or directories

```bash
# Remove App.ts and App.css
rm App.ts App.css

# Remove node_modules directory
rm -rf node_modules
```

## chmod (change mode)

This command changes mode of files to control who can read, write or execute files.

```bash
# Make build.sh executable
chmod +x build.sh
./build.sh
```

## sudo (super user do)

We use this command to run commands as a superuser to perform tasks that need permission to do.

```bash
# Install python
sudo apt install python
```

## Conclusion

The above commands are what you use frequently when you work in Unix-based systems. Hope this article make you more familliar with shell commands.
