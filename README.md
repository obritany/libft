# libft
My implementation of some of the Standard C Library functions including some additional ones.

### What is libft?
Libft is an individual project that requires us to re-create some standard C library functions including some additional ones that can be used later to build a library of useful functions for the rest of the program.

### What's in it?

1.  **Libc Functions:** Some of the standard C functions
2.  **Additional functions:** Functions will be useful for later projects
3.  **Bonus Functions:** Functions will be useful for linked list manipulation
4.  **Personal Functions:** Functions I believe will be useful later

Libc functions | Additional functions | Bonus Functions | Personal Functions
:----------- | :-----------: | :-----------: | -----------:
memset		| ft_memalloc	| ft_lstnew		| ft_capitalize 
bzero		| ft_memdel		| ft_lstdelone	| ft_countwords 
memcpy		| ft_strnew		| ft_lstdel		| ft_islower    
memccpy		| ft_strdel		| ft_lstadd		| ft_isupper    
memmove		| ft_strclr		| ft_lstiter	| ft_strndup    
memchr		| ft_striter	| ft_lstmap		| ft_lst_reverse
memcmp		| ft_striteri	|				| ft_realloc
strlen		| ft_strmap		|				| ft_strjoinch
strdup		| ft_strmapi	|				| ft_strnchr
strcpy		| ft_strequ		|				| ft_copyuntil
strncpy		| ft_strnequ	|			| ft_strstartswith
strcat		| ft_strsub		| | ft_intlen
strlcat		| ft_strjoin	| | ft_strendswith
strchr		| ft_strtrim	| | ft_pathjoin
strrchr		| ft_strsplit	| | ft_lstaddback
strstr		| ft_itoa		| | get_next_line
strnstr		| ft_putchar	| | ft_putnstr
strcmp		| ft_putstr		| | ft_strreplace
strncmp		| ft_putendl	| | ft_isemptystr
atoi		| ft_putnbr		| | ft_strsplitall
isalpha		| ft_putchar_fd	| | ft_countwordsall
isdigit		| ft_putstr_fd	| | ft_freestrarr
isalnum		| ft_putendl_fd	| | ft_strjoincl
isascii		| ft_putnbr_fd	| | ft_strjoinchcl
isprint		|| | ft_count2darray
toupper		| | | ft_strarrmax
tolower		| | | ft_get_parent_path

### How does it work?

The goal is to create a library called libft.a from the source files so I can later use that library from other projects.

To create that library, after downloading/cloning this project:

	git clone https://github.com/obritany/libft
	cd libft
	make

You should see a *libft.a* file and some object files (.o).

Now to clean up (removing the .o files and the .c files from the root), call `make clean`

### How do I use the library?
 
You have to tell the file where your library resides and which library it is using:

`gcc example.c -L. -lft`

-L takes the path to your library. `.` in this case<br>
-l takes the name of your library. This is the set of characters that come after `lib` in your library name.

That's it. Now run it using `./a.out`
