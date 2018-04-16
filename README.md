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

<ul>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_memalloc.c">ft_memalloc</a></td>
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
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_memdel.c">ft_memdel</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_memdel(void **ap);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Takes as a parameter the address of a memory area that needs to be freed with free(3), then puts the pointer to NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>A pointer’s address that needs its memory freed and set to NULL.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strnew.c">ft_strnew</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strnew(size_t size);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns a “fresh” string ending with ’\0’. Each character of the string is initialized at ’\0’. If the allocation fails the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The size of the string to be allocated.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The string allocated and initialized to 0.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strdel.c">ft_strdel</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_strdel(char **as);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Takes as a parameter the address of a string that need to be freed with free(3), then sets its pointer to NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string’s address that needs to be freed and its pointer set to NULL.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strclr.c">ft_strclr</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_strclr(char *s);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Sets every character of the string to the value ’\0’.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string that needs to be cleared.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_striter.c">ft_striter</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_striter(char *s, void (*f)(char *));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Applies the function f to each character of the string passed as argument. Each character is passed by address to f to be modified if necessary.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to iterate.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The function to apply to each character of s.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_striteri.c">ft_striteri</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_striteri(char *s, void (*f)(unsigned int, char *));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Applies the function f to each character of the string passed as argument, and passing its index as first argument. Each character is passed by address to f to be modified if necessary.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to iterate.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The function to apply to each character of s and its index.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strmap.c">ft_strmap</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strmap(char const *s, char (*f)(char));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Applies the function f to each character of the string given as argument to create a “fresh” new string (with malloc(3)) resulting from the successive applications of f.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to map.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The function to apply to each character of s.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The “fresh” string created from the successive applications of f.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strmapi.c">ft_strmapi</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strmapi(char const *s, char (*f)(unsigned int, char));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Applies the function f to each character of the string passed as argument by giving its index as first argument to create a “fresh” new string (with malloc(3)) resulting from the successive applications of f.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to map.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The function to apply to each character of s and its index.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The “fresh” string created from the successive applications of f.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strequ.c">ft_strequ</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>int ft_strequ(char const *s1, char const *s2);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Lexicographical comparison between s1 and s2. If the 2 strings are identical the function returns 1, or 0 otherwise.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The first string to be compared.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The second string to be compared.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>1 or 0 according to if the 2 strings are identical or not.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strnequ.c">ft_strnequ</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>int ft_strnequ(char const *s1, char const *s2, size_t n);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Lexicographical comparison between s1 and s2 up to n characters or until a ’\0’ is reached. If the 2 strings are identical, the function returns 1, or 0 otherwise.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The first string to be compared.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The second string to be compared.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>1 or 0 according to if the 2 strings are identical or not.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strsub.c">ft_strsub</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strsub(char const *s, unsigned int start, size_t len);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns a “fresh” substring from the string given as argument. The substring begins at indexstart and is of size len. If start and len aren’t refering to a valid substring, the behavior is undefined. If the allocation fails, the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The from which the substring is created.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The start index of the substring.</td>
		</tr>
		<tr>
			<td>Param. #3</td>
			<td>The size of the substring.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The substring.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strjoin.c">ft_strjoin</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strjoin(char const *s1, char const *s2);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns a “fresh” string ending with ’\0’, result of the concatenation of s1 and s2. If the allocation fails the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The prefix string.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The suffix string.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The “fresh” string result of the concatenation of the 2 strings.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strtrim.c">ft_strtrim</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_strtrim(char const *s);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns a copy of the string given as argument without whitespaces at the beginning or at the end of the string. Will be considered as whitespaces the following characters: ’ ’, ’\n’ and ’\t’. If s has no whitespaces at the beginning or at the end, the function returns a copy of s. If the allocation fails the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to be trimed.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The “fresh” trimmed string or a copy of s.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_strsplit.c">ft_strsplit</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char ** ft_strsplit(char const *s, char c);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns an array of “fresh” strings (all ending with ’\0’, including the array itself) obtained by spliting s using the character c as a delimiter. If the allocation fails the function returns NULL. Example: ft_strsplit("*hello*fellow***students*", ’*’) returns the array ["hello", "fellow", "students"].</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to split.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The delimiter character.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The array of "fresh" strings as a result of the split.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_itoa.c">ft_itoa</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>char * ft_itoa(int n);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocate (with malloc(3)) and returns a “fresh” string ending with ’\0’ representing the integer n given as argument. Negative numbers must be supported. If the allocation fails, the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The integer to be transformed into a string.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The string representing the integer passed as argument.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putchar.c">ft_putchar</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putchar(char c);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the character c to the standard output.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The character output.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putstr.c">ft_putstr</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putstr(char const *s);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the string s to the standard output.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to output.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putendl.c">ft_putendl</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putendl(char const *s);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the string s to the standard output followed by a ’\n’.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to output.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putnbr.c">ft_putnbr</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putnbr(int n);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the integer n to the standard output.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The integer to output.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putchar_fd.c">ft_putchar_fd</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putchar_fd(char c, int fd);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the char c to the file descriptor fd.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The character to output.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The file descriptor.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putstr_fd.c">ft_putstr_fd</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putstr_fd(char const *s, int fd);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the string s to the file descriptor fd.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to output.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The file descriptor.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>	
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putendl_fd.c">ft_putendl_fd</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putendl_fd(char const *s, int fd);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the string s to the file descriptor fd followed by a ’\n’.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The string to output.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The file descriptor.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>	
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_putnbr_fd.c">ft_putnbr_fd</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_putnbr_fd(int n, int fd);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Outputs the integer n to the file descriptor fd.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The integer to output.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The file descriptor.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>	
</ul>

#### `List Functions`

The structure of the links for the following list functions is in the [libft.h](/libft.h) file and shown below:

```
typedef struct 		s_list
{
	void 		*content;
	size_t 		content_size;
	struct s_list 	*next;
}
```

<ul>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstnew.c">ft_lstnew</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>t_list * ft_lstnew(void const *content, size_t content_size);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Allocates (with malloc(3)) and returns a “fresh” link. The variables content and content_size of the new link are initialized by copy of the parameters of the function. If the parameter content is nul, the variable content is initialized to NULL and the variable content_size is initialized to 0 even if the parameter content_size isn’t. The variable next is initialized to NULL. If the allocation fails, the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The content to put in the new link.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The size of the content of the new link.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The new link.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
		<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstdelone.c">ft_lstdelone</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_lstdelone(t_list **alst, void (*del)(void *, size_t));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Takes as a parameter a link’s pointer address and frees the memory of the link’s content using the function del given as a parameter, then frees the link’s memory using free(3). The memory of next must not be freed under any circumstance. Finally, the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel in the mandatory part).</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The address of a pointer to a link that needs to be freed.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstdel.c">ft_lstdel</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_lstdel(t_list **alst, void (*del)(void *, size_t));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Takes as a parameter the adress of a pointer to a link and frees the memory of this link and every successors of that link using the functions del and free(3). Finally the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel from the mandatory part).</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The address of a pointer to the first link of a list that needs to be freed.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstadd.c">ft_lstadd</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_lstadd(t_list **alst, t_list *new);</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Adds the element new at the beginning of the list.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>The address of a pointer to the first link of a list.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The link to add at the bginning of the list.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstiter.c">ft_lstiter</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>void ft_lstiter(t_list *lst, void (*f)(t_list *elem));</td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Iterates the list lst and applies the function f to each link.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>A pointer to the first link of a list.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The address of a function to apply to each link of a list.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>None.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
	<li><table>
		<tr>
			<td colspan="2" align="center"><a href="ft_lstmap.c">ft_lstmap</a></td>
		</tr>
		<tr>
			<td>Prototype</td>
			<td>t_list * ft_lstmap(t_list *lst, t_list * (*f)(t_list *elem)); </td>
		</tr>
		<tr>
			<td>Description</td>
			<td>Iterates a list lst and applies the function f to each link to create a “fresh” list (using malloc(3)) resulting from the successive applications of f. If the allocation fails, the function returns NULL.</td>
		</tr>
		<tr>
			<td>Param. #1</td>
			<td>A pointer to the first link of a list.</td>
		</tr>
		<tr>
			<td>Param. #2</td>
			<td>The address of a function to apply to each link of a list.</td>
		</tr>
		<tr>
			<td>Return value</td>
			<td>The new list.</td>
		</tr>
	</table></li>
	<a href="#top">↥ back to top</a>
</ul>

