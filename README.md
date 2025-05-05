# ft_printf

*Oh bold artisan of code, set forth on your quest to master the symphony of formatted output!*

Within this project lies the challenge of crafting a versatile `printf` function from scratch, a testament to your ingenuity and precision in C programming.

## Prelude

*Oh brave architect of algorithms, venture into the intricate world of `ft_printf`!* 

Here, you will reconstruct the legendary `printf` function, exploring the depths of variable arguments, formatting flexibility, and the magic of pointers.

## Table of Contents

- [The Quest](#the-quest)
- [Features](#features)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Supported Conversion Specifiers](#supported-conversion-specifiers)
- [Testing](#testing)
- [Acknowledgments](#acknowledgments)

## The Quest

*Set sail, O daring coder, on this epic journey!*

Your mission is to replicate the functionality of the standard `printf` function, adhering to the following goals:
- Support a rich subset of format specifiers.
- Utilize `stdarg.h` to elegantly manage variable arguments.
- Ensure robustness through careful handling of edge cases.
- Strive for efficiency and accuracy in your implementation.

## Features

*Marvel at the capabilities of ft_printf:*

- **Custom Implementation**: Build a robust alternative to `printf` from first principles.
- **Dynamic Argument Handling**: Master the use of `va_list` to process flexible input.
- **Versatile Formatting**: Handle strings, integers, pointers, and more with precision.
- **Extensibility**: Expand the function with additional specifiers to suit your needs.

## Requirements

*To construct this masterpiece, arm yourself with these essentials:*

- **Compiler**: GCC or Clang.
- **Libraries**: Standard C library (`<unistd.h>`, `<stdarg.h>`, `<stdlib.h>`).
- **Makefile**: Automate your build process with targets `all`, `clean`, `fclean`, and `re`.

## Getting Started

*Raise the anchor and chart your course!*

Clone this repository and navigate to the `ft_printf` directory:
```bash
git clone https://github.com/nsilva-n/42CC-1-ft_printf.git
cd 42CC-1-ft_printf
make
```

## Supported Conversion Specifiers

*With these tools, command the art of formatted output:*

| Specifier | Description                        |
|-----------|------------------------------------|
| `%c`      | Print a single character           |
| `%s`      | Print a string                     |
| `%p`      | Print a pointer address            |
| `%d`      | Print a decimal integer            |
| `%i`      | Print an integer                   |
| `%u`      | Print an unsigned integer          |
| `%x`      | Print a hexadecimal number (lower) |
| `%X`      | Print a hexadecimal number (upper) |
| `%%`      | Print a percent sign               |

*Enhance the function as you progress through your coding journey!*

## Testing

*Verify the strength of your creation with rigorous testing:*

Create your own test cases to compare `ft_printf` against the standard `printf`.

Example:
```c
#include "ft_printf.h"
#include <stdio.h>

int main() {
    int num = 42;
    int original_printf_len;
    int ft_printf_len;
    ft_printf_len = ft_printf("My number: %d\n", num);
    original_printf_len = printf("Expected: My number: %d\n", num);
    printf("ft length = %d vs original length = %d\n", ft_printf_len, original_printf_len);
    return 0;
}
```

## Acknowledgments

*With boundless gratitude to the pioneers of the C Standard Library and the architects of the 42 curriculum, we present this work.*

May your journey through the labyrinth of `ft_printf` lead you to enlightenment and mastery over the art of formatted output.
