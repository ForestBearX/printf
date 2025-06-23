# 42 Project - ft_printf

This project is a custom implementation of the `printf` function in C, created as part of the 42 curriculum. The goal is to implement a function that mimics the standard `printf` with basic format specifiers and improve understanding of variable argument lists in C.

## Features

- Implements common `printf` format specifiers:
  - `%c` - Character
  - `%s` - String
  - `%p` - Pointer address
  - `%d` / `%i` - Integer (decimal)
  - `%u` - Unsigned integer
  - `%x` / `%X` - Hexadecimal (lowercase/uppercase)
  - `%f` - Floating-point numbers
- Handles edge cases like null strings and negative values.

## Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/ft_printf.git
   cd ft_printf
   ```

2. Compile the project using `make`:
   ```bash
   make
   ```

   This will generate the `libftprintf.a` static library.

## Usage

To use `ft_printf`, include the header `ft_printf.h` in your program and link with the `libftprintf.a` library:

```c
#include "ft_printf.h"

int main() {
    ft_printf("Hello, world! %s %d\n", "42", 42);
    return 0;
}
```

When compiling, link the library like this:

```bash
gcc main.c -L. -lftprintf -o my_program
```

## Functionality

### ft_printf

```c
int ft_printf(const char *format, ...);
```

- `format` is the format string with format specifiers (like `%s`, `%d`, etc.).
- `...` represents the variables to be printed according to the specifiers.

**Returns:** the number of characters printed (excluding the null byte `\0`).

## Testing

You can run the provided test suite to check the implementation. Just run:

```bash
make test
```

## Contributing

Feel free to fork the repository and submit improvements. If you find any bugs or have suggestions, open an issue or send a pull request.

## License

This project is open-source and licensed under the MIT License.
