# Introduction
평소 라이브러리에서 자주 꺼내쓰던 함수들을 골라, 그 구조를 파악하고 똑같은 기능을 수행하는 나만의 함수를 직접 만들어본다. 

-------------------------


# Function Overview

**Function	Description**

|               함수명               |                                       기능                                   |
| :---------------------------------: | :--------------------------------------------------------------------------: |
|   ft_atoi  | 	Reads a String, and, after ignoring spaces with ft_isspace, saves the string into an integer  |   
|   ft_bzero  | 	 Writes n zeroes to the string s  | 
|   ft_calloc  |   Reserves x blocks of y bits of memory  | 
|   ft_isalnum  | 	Returns 1 if the input is a number or a letter in the ASCII table  | 
|   ft_isalpha  | 	Returns 1 if the input is a letter in the ASCII table  | 
|   ft_isascii  | 	Returns whether or not a value belongs to the ASCII table  | 
|   ft_isdigit  | 	Returns 1 if the input is a number in the ASCII table  | 
|   ft_isprint  | 	Returns whether a character is printable  | 
|   ft_itoa  | 	Saves the given number as a string (char array)  | 
|   ft_memccpy  | 	Copies from one memory point to another, until the specified character is copied or until n bytes are copied  | 
|   ft_memchr  | 	Looks for a matching character inside a part of the memory  | 
|   ft_memcmp  | 	Compares two parts of memory, returning 0 if they're the same, or else a nonzero value  | 
|   ft_memcpy  | 	Copies from one part of memory to another, ignoring possible overlaps  | 
|   ft_memmove  | 	Copies from one part of memory to another, preventing possible overlaps  | 
|   ft_memset  | 	Assigns a character n times to a part of the memory  | 
|   ft_putchar_fd  | 	Prints a character to the given file descriptor  | 
|   ft_putendl_fd  | 	 Prints a string followed by a new line \n to a given file descriptor  | 
|   ft_putnbr_fd  | 	Prints number to the given file descriptor  | 
|   ft_putstr_fd  | 	Prints string to the given file descriptor  | 
|   ft_split  | 	Splits a string according to a given separator character  | 
|   ft_strchr  | 	 Looks for a specific character inside a given string  | 
|   ft_strdup  | 	Saves enoug space and duplicates a string  | 
|   ft_strjoin  | 	 Concatenates two strings allocating enough space first  | 
|   ft_strlcat  | 	 Concatenates two strings ensuring it ends with \0  | 
|   ft_strlcpy  | 	Copies n - 1 bytes from a source string to a destination string  | 
|   ft_strlen  | 	Returns length of a string  | 
|   ft_strmapi  | 	Applies a function (mapping) to every element in a string  | 
|   ft_strncmp  | 	Compares two strings up to the n-th character  |
|   ft_strnstr  | 	Tries to find a substring (needle) in a second string (haystack) before the n-th char is reached  | 
|   ft_strrchr  |	Looks for a given character in a string, reading it from back to front  | 
|   ft_strtrim  |	Removes occurrences of characters in a string from the start and end of another one  | 
|   ft_substr  |	Copies from the n-th char of a string  | 
|    ft_tolower  |	Makes every uppercase character in a string lowercase  | 
|    ft_toupper  |	Makes every lowercase character in a string uppercase  | 

 
# Bonus

아래는 연결리스트를 사용하는 함수라 아래의 구조와 같은 구조체를 정의하여 함수 구현을 진행하였다.

```
typedef	struct	s_list
{
	void		*content;
	struct	s_list	*next;
}			t_list;
Bonus functions to implement
```

**Bonus Function	Description**

|               함수명               |                                       기능                                   |
| :---------------------------------: | :--------------------------------------------------------------------------: |
|  ft_lstnew  |  Creates new node allocating with malloc  |
|  ft_lstadd_front  |	Adds new node at the beginning of the linked list  |
|  ft_lstsize  |	Returns number of elements of linked list  |
|  ft_lstlast  |	Retrieves last node of the list  |
|  ft_lstadd_back  |	Adds new node at the end of the linked list  |
|  ft_lstdelone  |	Deletes, frees, and applies function del to content of a given node  |
|  ft_lstclear  |	Deletes a given element and every element after that  |
|  ft_lstiter  |	Applies a function to the content of every node of the linked list  |
|  ft_lstmap  |	Applies function to a copy of the list, freeing when necessary  |
