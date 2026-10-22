# User and Filesystem Basics

This module introduces basic Linux commands for identifying the current user, displaying text, understanding the filesystem, and navigating directories.

## 1. Background and Concepts

Before using the commands in this module, let's briefly cover a few concepts that will help you understand what they do.

### Users

Linux is a multi-user operating system. It can have multiple user accounts, each with its own identity and permissions.

When you execute a command in your terminal, it runs under a particular user account. The commands in this module will help you identify that user and understand your current environment.

### Files and Directories

A **file** stores information, such as text, configuration, or program data.

A **directory** is used to organise files and other directories. Directories can contain multiple levels of nested directories, forming a hierarchy.

### The Linux Filesystem

Linux organises files and directories under a single hierarchy that begins at the root directory, represented by `/`.

Unlike Windows, where drives are commonly represented by letters such as `C:` and `D:`, Linux exposes its filesystem through a unified directory tree. Other storage devices and filesystems can be mounted at locations within this hierarchy.

Some important locations include:

| Path | Purpose |
|---|---|
| `/` | The root of the filesystem hierarchy. |
| `/home` | Typically contains users' home directories. |
| `/etc` | Contains system-wide configuration files. |
| `/tmp` | Used for temporary files. |
| `/usr` | Contains many installed programs, libraries, and shared resources. |

You don't need to memorise these locations yet. Just recognise that different directories serve different purposes.

### Paths and the Working Directory

A **path** identifies the location of a file or directory.

There are two common types:

- **Absolute path:** Starts from the root directory, such as `/home/user/Documents`.
- **Relative path:** Describes a location relative to the current working directory, such as `Documents` or `../Downloads`.

Your **current working directory** is the directory your shell is currently operating from. Commands such as `ls` and `cd` commonly use it as their starting point.

Some useful path symbols are:

| Symbol | Meaning |
|---|---|
| `/` | Root directory when used as a path; also separates path components. |
| `~` | The current user's home directory in the shell. |
| `.` | The current directory. |
| `..` | The parent directory. |

With these concepts in mind, let's explore the commands.

## 2. Commands and Examples

### `whoami`

Displays the username of the user running the command.

```bash
whoami
```

### `echo`

Prints text or variable values to standard output.

```bash
echo "Hello, Linux!"
```

### `pwd`

Displays the absolute path of the current working directory.

```bash
pwd
```

### `ls`

Lists files and directories in a location. If no location is specified, it lists the contents of the current working directory.

```bash
ls
ls -l
ls -a
ls -al
```

The options `-l`, `-a`, and `-al` modify how `ls` displays directory contents. These are commonly referred to as **flags** or **options**.

- `-l`: Displays a detailed listing, including permissions, ownership, size, and modification time.
- `-a`: Includes hidden entries, whose names begin with a dot (`.`).
- `-al`: Combines both options, displaying hidden entries in a detailed listing.

Options can often be combined when they use the short-option format. For example, `ls -al` is equivalent to `ls -a -l`.

### `cd`

Changes the current working directory.

```bash
cd /tmp
cd ..
cd ~
cd -
```

- `cd /tmp`: Moves to `/tmp`.
- `cd ..`: Moves to the parent directory.
- `cd ~`: Moves to the current user's home directory.
- `cd -`: Returns to the previous working directory.

## 3. What Are Flags in Commands?

Commands can accept additional options and arguments that change their behaviour or specify what they should operate on.

### Flags and Options

A **flag** or **option** modifies how a command behaves. Short options commonly begin with a single hyphen (`-`), while long options often begin with two hyphens (`--`).

For example:

```bash
ls -a
ls --all
```

Both commands tell `ls` to include hidden entries in its output.

Some options can be combined:

```bash
ls -al
```

This combines the `-a` and `-l` options.

### Arguments

An **argument** provides information to a command, such as the file or directory it should operate on.

For example:

```bash
ls /home
```

Here, `/home` is an argument specifying which directory to list.

You can combine options and arguments:

```bash
ls -la /home
```

This displays a detailed listing, including hidden entries, for `/home`.

**Remember:** option syntax varies between commands. Not every command uses the same flags, and some options require their own arguments. Use `command --help` when supported, or consult the command's manual with `man command`.

## 4. Practice

Open a terminal and execute the following commands one at a time. Observe the output after each command.

```bash
whoami
echo "I am learning Linux"
pwd
ls
ls -la
cd /
pwd
ls
cd ~
pwd
cd -
pwd
```

Pay attention to how the output of `pwd` changes when you navigate between directories.

These examples work in Bash and Fish. More advanced shell syntax may differ between them.
