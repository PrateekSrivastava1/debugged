# Styling guidelines for code written in The C Programming Language

```C
#include <stdio.h>
int main()
{
  printf("Hello, world!\n");
  return 0;
}
```

Above snippet is probably the first C program you ever wrote in your life.

But, as you ease into the world of programming and write more intricate and long code, you'll need to keep its readability in your mind.
Written below, are some conventions that are recommended to be followed while writing programs in C. They're not rules, just a set of guidelines to help you write cleaner code.

### Naming:
Functions and variables names should follow the snake case convention.
For example, consider the following names:
- `num_of_letters`
- `array_1_size`
- `find_largest_num()`

Constant should follow the same convention, except that the characters should be all caps
- `float MATH_PI = 3.14159;`

### Indentation
[Allman Indentation Style](https://en.wikipedia.org/wiki/Indentation_style#Allman_style) should be used throughout the program.

### Spacing
There should be a space **before** and **after** every operators, like this:
- `int x = 0`
- `for (int i = 0; i < size; i++)`

These should be a space **after** every comma, like this:
- `int x, y, z = 0;`
- `scanf("%s", string);`

There should be a space after a construct name, and the opening parantheses, like this:
- `for (initiation; condition; update)`
- `while (condition)`
- `if (condition)`

Insert a space after the comment symbol like this:
- `// Comment with a space between '//' and description`

### Comments
Every program should have a multiline **header comment** explaining the program.

Every function should have an accompanying comment on top, like this:

```C
// Returns the largest element from the parameter array
int find_largest(int array[], int size)
```

Complex constructs should have an accompanying comment explaining their work on top, like this:

```C
int max = array[0]
// Find the largest element
for (int i = 0; i < size; i++)
{
  // If a larger element than current found, store that as largest
  if (max < array[i]
  {
    max = array[i]
  }
}
```

As a rule of thumb, comment lines that others may take more than 5-10 seconds to understand while reading. Try to write comments that explain *WHY* instead of *WHAT*
