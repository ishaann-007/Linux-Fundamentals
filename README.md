# Linux Fundamentals

A beginner-friendly repository for learning and practising basic Linux commands through hands-on exercises.

## Background

### Environment

The commands and examples in this repository are primarily tested in the following environment:

- **Operating System:** CachyOS (Arch Linux-based distribution)
- **Shell:** Fish

Commands may behave differently depending on the Linux distribution, shell, or installed utilities.

**If you're using a different environment and notice differences, please open a Pull Request.**

### What is this about?

I'm learning Linux commands and wanted a practical way to revise what I've learned. Since other beginners might find this useful too, I'm building this repository as a place to practise basic Linux commands through simple exercises.

Feel free to clone the repository and use the practice material to improve your understanding of the Linux command line.

### Why am I doing this?

I studied Linux Fundamentals through TryHackMe, but realised that I had forgotten many of the commands I learned. I decided to create this GitHub repository to practise those commands again and explore others as I continue using Linux daily.

The project will cover the given commands in detail along with relevant flags which you'll probably use if you daily drive linux - additional commands would be covered in a seperate repository (or this one i donno) sometime in the future.

## Commands Covered

The commands are organised in a progressive order, starting with basic system identification and moving towards filesystem operations, text processing, and data transfers.

### 1. User and Terminal Basics

| Command | Purpose |
|---|---|
| `whoami` | Displays the username of the current user. |
| `echo` | Prints text or variable values to standard output. |

### 2. Understanding and Navigating the Filesystem

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory. |
| `ls` | Lists files and directories. |
| `cd` | Changes the current working directory. |
| `find` | Searches for files and directories based on specified criteria. |

### 3. Creating and Managing Files and Directories

| Command | Purpose |
|---|---|
| `mkdir` | Creates directories. |
| `touch` | Creates an empty file if it does not exist, or updates timestamps on an existing file. |
| `cp` | Copies files and directories. |
| `mv` | Moves or renames files and directories. |
| `rm` | Removes files and, with appropriate options, directories. |

### 4. Reading and Searching File Contents

| Command | Purpose |
|---|---|
| `cat` | Displays or concatenates file contents. |
| `grep` | Searches input for lines matching a pattern. |

### 5. Downloading and Transferring Data

| Command | Purpose |
|---|---|
| `curl` | Transfers data to or from a URL. |
| `wget` | Downloads files from URLs and supports other retrieval operations. |

This list will expand as I learn and practise additional commands.

## Basic Shell Operators

Shell operators control how commands are executed and how their input or output is handled. They are not commands themselves.

| Operator | Purpose |
|---|---|
| `&` | Runs the preceding command in the background. |
| `&&` | Executes the next command only if the preceding command succeeds. |
| `>` | Redirects standard output to a file, replacing its existing contents. |
| `>>` | Redirects standard output to a file, appending to its existing contents. |

Additional operators will be introduced as they become relevant to the exercises.

## Notes and Scope

Commands can accept flags and arguments that modify their behaviour. These will be explained alongside each command, with practical examples rather than as a list to memorise.

This repository focuses on basic Linux commands and relevant everyday usage. More advanced topics, including package management and system administration, may be covered separately as the project develops.

## Project Status

This repository is a work in progress. It is intended to evolve alongside my learning rather than serve as a complete Linux reference from the beginning.

The focus is on understanding commands, practising them in a terminal, and learning through experimentation.

## Getting Started

Clone the repository and navigate into its directory:

```bash
git clone https://github.com/ishaann-007/Linux-Fundamentals.git
cd Linux-Fundamentals
```

Head over to [Getting Started](https://github.com/ishaann-007/Linux-Fundamentals/blob/main/Getting-Started/Getting-Started.md) to begin your Linux Fundamentals Journey!

Practice instructions and exercise files will be added as the repository develops.

## Contributions and Feedback

If you're also learning Linux, feel free to use the material, suggest improvements, or point out inaccuracies. The goal is to keep the repository accessible, practical, and useful for beginners.
