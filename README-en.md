 <div align="center">
  <img src="https://raw.githubusercontent.com/15Galan/42_project-readmes/refs/heads/master/banners/cursus/projects/libft-light.png#gh-light-mode-only" />
  <img src="https://img.shields.io/badge/status-finished-green" />
  <img src="https://img.shields.io/badge/score-125-blue" /> <br/>
  <b>English</b> · <a href="../README.md">Español</a>
</div> 

---

# 📖 Introduction
Libft is a project from the 42 School program that consists of creating a library of functions in C. The main goal is to replicate and extend common functions from the C standard library (`libc`), as well as develop new useful functions for future projects.

This is the [subject](Libft_es.subject.pdf) of the project.

---

## Table of Contents
- ⚙️[Requirements](#requirements)
- 🛠️[Installation](#installation)
- 🚀[Usage](#usage)
- 📚[Implemented Functions](#implemented-functions)

---

## ⚙️Requirements

- **Operating System**: Linux or macOS
- **Compiler**: `gcc` with support for the C99 standard or higher
- **Tools**: `Makefile` for compilation, doxygen(optional)

---

## 🛠️Installation

1. Clone this repository to your local machine:
```bash
git clone https://github.com/your_user/libft.git
cd libft
```
2. Compile the library by running the command:
```bash
make
```
3. This will generate a file called `libft.a`, which you can include in your projects.

---

## 🚀Usage

To use libft in your project, include the header file and link the library when compiling:
```c
#include "libft.h"
```
Compile your program by linking the library:
```c
gcc -o mainprogram.c -L. -lft
```

---

## 📚Implemented Functions

In **libft**, functions are divided into several categories based on their functionality and purpose.

---

### Part 1 - libc Functions

These functions are custom implementations of some of the most common functions in the C standard library. They are used for string manipulation, memory manipulation, and more.

- **Memory manipulation:**
- `ft_memset` - Fill a memory region with a specific byte.
- `ft_bzero` - Fill a memory region with zeros.
- `ft_memcpy` - Copy a block of memory from one location to another.
- `ft_memccpy` - Copy bytes of memory until a specific character is found.
- `ft_memmove` - Copy blocks of memory, handling overlaps.
- `ft_memchr` - Search for a byte in a memory region.
- `ft_memcmp` - Compare two memory regions.

- **String manipulation:**
- `ft_strlen` - Calculate the length of a string.
- `ft_strlcpy` - Copy a string with a limited size.
- `ft_strlcat` - Safe concatenation of strings with a size limit.
- `ft_strchr` - Search for the first occurrence of a character in a string.
- `ft_strrchr` - Finds the last occurrence of a character in a string.
- `ft_strncmp` - Compares two strings up to a specified number of characters.
- `ft_strnstr` - Finds the first occurrence of a substring within another, limited by size.
- `ft_strdup` - Creates a dynamic copy of a string.

- **Conversion and utilities:**
- `ft_atoi` - Converts a string to an integer.
- `ft_isalpha` - Checks if a character is alphabetic.
- `ft_isdigit` - Checks if a character is a digit.
- `ft_isalnum` - Checks if a character is alphanumeric.
- `ft_isascii` - Checks if a character belongs to the ASCII set.
- `ft_isprint` - Checks if a character is printable.
- `ft_toupper` - Converts a character to uppercase.
- `ft_tolower` - Convert a character to lowercase.

---

### Part 2 - Additional Functions

These functions extend the standard functionality and provide useful tools for manipulating dynamic strings and structures.

- **String manipulation:**
- `ft_substr` - Extract a substring from a given string.
- `ft_strjoin` - Join two strings into a new string.
- `ft_strtrim` - Remove specific characters from the ends of a string.
- `ft_split` - Split a string into an array of strings based on a delimiter.
- `ft_itoa` - Convert an integer to a string.
- `ft_strmapi` - Apply a function to each character in a string and generate a new string.

- **Dynamic memory manipulation:**
- `ft_calloc` - Allocate zero-initialized memory.
- `ft_free` (optional depending on your implementation) - Safely free memory.

---

### Part 3 - Bonus Functions

This section is focused on working with linked lists, a basic data structure.

- **Creating and manipulating lists:**
- `ft_lstnew` - Creates a new node for a linked list.
- `ft_lstadd_front` - Adds a node to the front of a list.
- `ft_lstadd_back` - Adds a node to the end of a list.
- `ft_lstdelone` - Removes and frees a node from the list.
- `ft_lstclear` - Removes and frees all nodes from the list.
- `ft_lstiter` - Iterates over a list and applies a function to each node.
- `ft_lstmap` - Creates a new list by applying a function to each node of the original.

---

This classification makes it easier to understand and reuse the implemented functions. You can browse the `libft.h` file to see definitions and prototypes for all functions.  
You can use the Doxygen Documentation Generator to view more information about functions as you use them.
