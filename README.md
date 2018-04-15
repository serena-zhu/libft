# <a name="top">Libft</a>

Libft is a static library of C programming functions.

## Contents

[Language & Functions Used](#language_functions) | [Installation & Usage](#installation_usage) | [List of Functions](#functions)

## <a name="language_functions">Language & Functions Used</a>

Functions in libft are written in C, using only the following functions from the standard C libraries:

* malloc
* free
* write

<a href="#top">↥ back to top</a>

## <a name="installation_usage">Installation & Usage</a>

#### `Step 1` - clone the repo at the root of your project folder

```bash
$ git clone https://github.com/serena-zhu/libft.git
```

#### `Step 2` - compile library

```bash
$ make
```

The Makefile will compile a static library called libft.a, which can be compiled with your program source files as follows:

```bash
$ gcc -Wall -Wextra -Werror -o program_name source_file -L ./libft -lft
```
	
<a href="#top">↥ back to top</a>

## <a name="functions">List of Functions</a>

#### `Standard C Library Functions Recoded`

The function names are prefixed by "ft_". 

* [memset](/ft_memset.c)
* [bzero](/ft_bzero.c)
* [memcpy](/ft_memcpy.c)
* [memccpy](/ft_memccpy.c)
* [memmove](/ft_memmove.c)
* [memchr](/ft_memchr.c)
* [memcmp](/ft_memcmp.c)
* [strlen](/ft_strlen.c)
* [strdup](/ft_strdup.c)
* [strcpy](/ft_strcpy.c)
* [strncpy](/ft/strncpy.c)
* [strcat](/ft_strcat.c)
* [strncat](/ft_strncat.c)
* [strlcat](/ft_strlcat.c)
* [strchr](/ft_strchr.c)
* [strrchr](/ft_strrchr.c)
* [strstr](/ft_strstr.c)
* [strnstr](/ft_strnstr.c)
* [strcmp](/ft_strcmp.c)
* [strncmp](/ft_strncmp.c)
* [atoi](/ft_atoi.c)
* [isalpha](/ft_isalpha.c)
* [isdigit](/ft_isdigit.c)
* [isalnum](/ft_isalnum.c)
* [isascii](/ft_isascii.c)
* [isprint](/ft_isprint.c)
* [toupper](/ft_toupper.c)
* [tolower](/ft_tolower.c)

<a href="#top">↥ back to top</a>

#### `Additional Functions`

<table>
	<tr>
		<td colspan="2">[ft_memalloc](/ft_memalloc.c)</td>
	</tr>
	<tr>
		<td>Prototype</td>
		<td>void * ft_memalloc(size_t size);</td>
	</tr>
	<tr>
		<td>Description</td>
		<td>Allocates (with malloc(3)) and returns a “fresh” memory area. The memory allocated is initialized to 0. If the allocation fails, the function returns NULL.</td>
	</tr>
	<tr>
		<td>Param. #1</td>
		<td>The Size of the memory that needs to be allocated.</td>
	</tr>
	<tr>
		<td>Return value</td>
		<td>The allocated memory area.</td>
	</tr>
</table>

*
*

<a href="#top">↥ back to top</a>

#### `List Functions`

*
*
*

<a href="#top">↥ back to top</a>