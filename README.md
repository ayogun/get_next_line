<h1 align="center">
	📖 get_next_line
</h1>



<p align="center">
	<b><i>:yawning_face: Reading a line on a fd is way too tedious.</i></b><br>
</p>

<p align="center">
<img src="https://github.com/caroldaniel/caroldaniel-utils/blob/6b25474bf78299bc7cded8a9c423eebf35fb1d75/get_next_linem.png"/>
</p>

The goal of this project is to create the function _get_next_line.c_ which, when called in a loop, will then allow the available text in the file descriptor to be read one line at a time until the end of the file. The program must compile with the flag-D BUFFER_SIZE=xx which will be used as the buffer size for the read calls in get_next_line.

## Why is get_next_line important?
Get_next_line is a simple and challenging project which allows you to learn deeply about open(), read() and close() functions as well as static variables and file descriptors.

## Grade 
![image](https://user-images.githubusercontent.com/85964972/132257264-f92eb828-0168-46d7-aa10-15a6bf44ef6e.png)



<h3 align="center">
	<a href="#%EF%B8%8F-about">About</a>
	<span> · </span>
	<a href="#%EF%B8%8F-usage">Usage</a>
	<span> · </span>
	<a href="#-testing">Testing</a>
</h3>

---

## 💡 About the project

> _The aim of this project is to make you code a function that returns a line, read from a file descriptor._

	You will understand how files are opened, read and closed in an OS,
	and how they are interpreted by a programming language for further analysis.
	This task is crucial to understand for a future programmer since much of the time is based
	on manipulating files for data management and persistence.
	This project consists of coding a function that returns one line at a time from a text file.

For more detailed information, look at the [**subject of this project**](https://github.com/Surfi89/42cursus/tree/main/Subject%20PDFs).


## 🛠️ Usage

### Requirements

The function is written in C language and thus needs the **`gcc` compiler** and some standard **C libraries** to run.

### Instructions

**1. Using it in your code**

To use the function in your code, simply include its header:

```C
#include "get_next_line.h"
```

and, when compiling your code, add the source files and the required flag:

```shell
get_next_line.c get_next_line_utils.c -D BUFFER_SIZE=<size>
```

## 📋 Testing

You only have to edit the get_next_line.c file and uncomment the main function and headers inside it.
You can edit test.txt files to put another text if you wish to test othe cases.
Then simply run this command (change "xx" with desired buffer size) :

```shell
gcc -Wall -Werror -Wextra -D BUFFER_SIZE=xx get_next_line.c get_next_line_utils.c && ./a.out
```

Or you can also use this third party tester to fully test the project

* [Tripouille/gnlTester](https://github.com/Tripouille/gnlTester)
