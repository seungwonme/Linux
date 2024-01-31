- [Command Structure](#command-structure)
- [Shortcut](#shortcut)
- [Linux-Command](#linux-command)
	- [Manual](#manual)
		- [type](#type)
		- [which](#which)
		- [help](#help)
		- [man](#man)
	- [Basic](#basic)
		- [clear](#clear)
		- [date](#date)
		- [cal](#cal)
		- [ncal](#ncal)
		- [history](#history)
	- [File System](#file-system)
		- [open](#open)
		- [pwd](#pwd)
		- [ls](#ls)
		- [cd](#cd)
		- [touch](#touch)
		- [file](#file)
		- [mkdir](#mkdir)
		- [rm](#rm)
		- [rmdir](#rmdir)
		- [mv](#mv)
		- [cp](#cp)
		- [cat](#cat)
		- [less](#less)
		- [tac](#tac)
		- [rev](#rev)
		- [head](#head)
		- [tail](#tail)
		- [wc](#wc)
		- [sort](#sort)
  

# Command Structure

```bash
> command [options] [arguments]
```

- `command` : command name
- `options` : option
  - `-` : short option
  - `--` : long option

# Shortcut

- `⌘ + ←, →` : Move cursor to the beginning(or end) of the line
- `⌥ + ←, →` : Move cursor to the beginning(or end) of the word
- `⌘ + K` : Clear terminal
- `⌃ + A, E` : Move cursor to the beginning(or end) of the line
- `⌃ + L` : Clear terminal
- `⌃ + U` : Delete line
- `⌃ + K` : Delete from cursor to the end of the line
- `⌃ + W` : Delete word
- `⌃ + Y` : Paste deleted text
- `⌃ + R` : Search history
- `⌃ + G` : Cancel search history
- `⌃ + D` : Delete character
- `⌃ + F` : Move cursor forward
- `⌃ + B` : Move cursor backward
- `⌃ + P, ↑` : Show previous command
- `⌃ + N, ↓` : Show next command

# Linux-Command

## Manual

### type

4 command types
- executable program(binary)
- shell built-in command
- shell function
- alias

### which

`which` command is used to find executable program(binary) path

### help

`help` command is used instead of `man` for shell built-in command
(zsh doesn't support `help` command, so use `man zshbuiltins`)

### man

```bash
> man [command name]
```

- `q` : quit
- `space(or f)` : next page
- `b` : previous page
- `h` : help
- `/` : search
- `n` : next search

```bash
> man echo

echo [-n] [string ...]
```

- `[]` : optional
- `...` : repeatable

## Basic

### clear

```bash
> clear
```

### date

```bash
> date
Wed Jan 31 18:19:27 KST 2024
```

### cal

```bash
> cal
    January 2024      
Su Mo Tu We Th Fr Sa  
    1  2  3  4  5  6  
 7  8  9 10 11 12 13  
14 15 16 17 18 19 20  
21 22 23 24 25 26 27  
28 29 30 31  
```

### ncal

```bash
> ncal
    January 2024      
Mo  1  8 15 22 29   
Tu  2  9 16 23 30   
We  3 10 17 24 31   
Th  4 11 18 25      
Fr  5 12 19 26      
Sa  6 13 20 27      
Su  7 14 21 28     
```

### history

`history` command is used to show command history

- `![history number]` : command is used to execute command history
- `!!` : command is used to execute previous command
- `$HISTSIZE` : environment variable is used to set command history size

## File System

### open

`open` command is used to open file or directory 

- `/` : root directory
- `~` : home directory
- `.` : current directory
- `..` : parent directory

### pwd

Print working directory

### ls

List directory contents

### cd 

Change directory

### touch

`touch` command is used to create file

### file

`file` command is used to check file type
Warning : [Characters to watch out for when naming files](https://en.wikipedia.org/wiki/Filename)

### mkdir

MaKe DIRectory

### rm

ReMove file or directory

### rmdir

ReMove DIRectory

### mv

MoVe file or directory

```bash
> mv <source...> <destination>
```

### cp

CoPy file or directory

### cat

conCATenate files and print on the standard output

### less

`less` command is used to show file contents

### tac

`cat` command is used to show file contents reversely

### rev

REVerse lines of a file

### head

`head` command is used to show first 10 lines of file

### tail

`tail` command is used to show last 10 lines of file

### wc

Word Count

### sort

`sort` command is used to sort lines of text files

```
> sort -k2 -n 
strawberry 5$
apple 2$  
banana 1.5$
grape 3$
---output---
banana 1.5$
apple 2$  
grape 3$
strawberry 5$
```
