---
title: 'Malloc and Free'
layout: 'single-portfolio'
permalink: /posts/malloc/
author_profile: true
excerpt_separator: <!--more-->
tags:
  - C
  - malloc
header:
   teaser: 
---

To try to learn a bit more about what goes on under the hood when I'm writing code I wrote a memory allocation and freeing module in C.
C requires memory management and has it's own functions to help with this, eg. malloc(), realloc(), calloc(), free().
To try to understand a bit more about how these worked, I decided to write my own versions of malloc() and free().
<!--more-->

The code, which is available at my [Github](https://github.com/kennege/malloc/blob/master/malloc.c), uses the same system call sbrk(), that malloc used to determine the location of the top of the memory heap. 
The challenge for this task isn't writing malloc-ing, its free-ing, specifically, keeping track of what memory can be freed, and what has been freed.

To do this I used a singly linked list to store the location of each allocated memory chunk, the size of the chunk, and a flag to indicate if it had been freed. 
Then, when malloc() is called, I use sbrk() to search a memory address where I can store both the new data, and an element of this.
I then store the list element at the beginning of the allocated chunk, and return a pointer to the end of the list element.
It seems that this approach of allocating additional memory for tracking purposes is how free() is also how free() is implemented in the standard C library.

When free() is called, the list can be searched for the chunk that is to be freed, and the flag is set.
Then, later calls to malloc can overwrite this chuck, if they fit within it.