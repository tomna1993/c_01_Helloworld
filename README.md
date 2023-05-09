c_01_HelloWorld
========================

## DESCRIPTION

The program prints out "Hello, world".

> #include <stdio.h> 

This line includes a header file named stdio.h -> Standart Input Output.  
We need to include this when we want to use the printf function which is declared in this library.   

> int main(void) 

This is the program's main function, we will discuss it later on. 

> printf("Hello, world\n"); 

The printf function takes one argument, the "Hello, world\n" string and outputs it in the terminal when we run the program.  
The "\n" at the end of the string is a newline character so the cursor will move to the next line after printing out the text.  
There are more like the \n character, they are called **escape sequences**:

| Escape sequence 	| Properties 	|
|-------------------|---------------|
| \"				| double quote	|
| \\				| single backslash |
| \a				| bell/alert	|
| \b				| backspace		|
| \r				| carriege return |
| \n				| newline		|
| \s				| space			|
| \t				| tab			|

We have to use the comma character (;) to end the line. We don't always use it to end the line, there are special cases f.e. the inlcude line or the
main function but these rules will be clear after a while.

The last things in our program are the curly braces, they are used to signify the start and end of a series of statements.

## INSTALL LIBRARIES

The source code uses the cs50 library what you can download [HERE](https://github.com/cs50/libcs50).

To install the cs50 library follow the steps:

1. Open git bash terminal and change the current working directory to `src`:   
  	> cd ./libsc50/src

2. Compile the cs50.c source into .o with:
	> gcc -c cs50.c -o cs50.o

3. Make the library archive:  
  	> ar rcs libcs50.a cs50.o

4. Copy the `libcs50.a` file into your compiler's `lib` directory

5. Copy the `cs50.h` file into your compiler's `include` directory

## COMPILE AND RUN THE CODE

The code is written in C, the compiler used to generate the exe is: `gcc Rev10, Built by MSYS2 project 12.2.0`

Run the below code in terminal (git bash) to compile the source:

> gcc commandLineArgument.c -lcs50 -o ./build/commandLineArgument

To run the executable run the below code in terminal (git bash):

> ./build/commandLineArgument.exe
