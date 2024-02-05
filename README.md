# Ft_Printf [42 Project]
This 42 Project challenges us to recreate the well known function `printf()` in C.

## Overview
This project tests our knowledge about `va_list` and String Manipulation. The function is formatted as follow:
```c
int ft_printf(const char *format, ...)
```
The `char *format` will be the string and the variables that you want to print.
The `...` will be a `var_list` containing all the varibles that appear in the format.

## About va_list
In C programing, the `va_list` function allows the user to access the variable arguments passed to a function which accepts a variable number of arguments.
In this case the `...` is the variable number of arguments the function receives.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Dependencies](#dependencies)
3. [Supported Conversions](#supported-conversions)
4. [Supported Flags](#supported-flags)
5. [How to Use](#how-to-use)
6. [Source file Example](#source-file-example)
7. [Contributing](#contributing)

## Project Structure
- `printf/`: Main directory containing the source code, header file and Makefile

## Dependencies
- None

## Supported Conversions
- %c: Character
- %s: String
- %d, %i: Decimal integer
- %u: Unsigned decimal integer
- %p: Address
- %x, %X: Unsigned hexadecimal integer
- %%: Character `%`

## Supported Flags
This project allows the student to make a bonus part, where we need to implement some additional flags in our function. That bonus isn't mandatory, so i decided not to do.
My ft_printf does not support any additional flags.
If you still are curiuos about the additional flags, you can check the [`printf` manual](https://man7.org/linux/man-pages/man3/printf.3.html)

## How to Use
To use the ft_printf, you need to:
1. Clone the repository
2. Go to the `ft_printf` directory `cd ft_printf`
3. Run the command `make`
4. In your source files include the header `#include "ft_printf.h"`
5. Link the library to your program `gcc example.c -L[path_to_ft_printf_dir] -lftprintf`

## Source file Example
Here's an example of a source file using one libft function
```c
/* Example: Printing a "Hello World" using ft_printf() */
#include "ft_printf.h"

int main()
{
    char *str = "World";
    ft_printf("Hello %s\n", str);
    return (0);
}
```

## Contributing
I welcome contributions. If you have any bug fix or improvement, feel free to submit a pull request on the repository.
