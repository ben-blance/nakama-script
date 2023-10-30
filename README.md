# nakama-script

![Nakama Script Logo](nakama-logo.png)

## Installation

To use Nakama Script, you need to set up the interpreter or environment on your system. Here are the installation instructions:

### System Requirements

Nakama Script is designed to be lightweight and should work on most systems. However, you need the following:

- Operating System: Any modern OS (Windows, macOS, Linux)
- Nakama Script Interpreter (Download from [GitHub](https://github.com/ben-blance/nakama-script))

## Installation

To get started with Nakama Script, follow these installation steps:

1. **Clone the Repository:** Start by cloning the Nakama Script repository to your local machine:

   ```shell
   git clone https://github.com/nakama-script
   ```
   1. Navigate to the Directory
   2. Copy Necessary Files: Copy the essential Nakama Script files, including shell.py, basic.py, and strings_with_arrows.py, to your project directory.
   3. Create Your Nakama Script File: In your project directory, create your own .ns file, for example, example.ns. This file will contain your Nakama Script code.
   4. Run the Nakama Script Shell: Execute the shell.py script using Python to start the Nakama Script shell
   5. Use the run Function: Inside the Nakama Script shell, you can run your example.ns script using the built-in run() function. For example:
      ```
      run("example.ns")
      ```

This will execute your Nakama Script file, and you will see the output in the shell.
Now you have Nakama Script installed and can create and run your own scripts. Happy coding!

  
      


## Getting Started

Once Nakama Script is installed, you can start writing and running Nakama Script programs. Here's a quick overview:

- **Running Nakama Script Programs:** Use the `run` command to run Nakama Script programs. For example, `run("my_program.ns")`.

### Hello, World

Here's a simple "Hello, World" program in Nakama Script:

```ns
gears hello_world() ->
    print("Hello, World")
end

hello_world()
```
### Output
```ns
"Hello, World"
```
## Syntax

- **Variable Declaration:** Variables are declared with the `nakama` keyword.

- **Function Definitions:** Functions are defined using the `gears` keyword.

- **Conditional Statements:** Supports `if`, `elif`, and `else` conditional statements.

- **Loops:** Includes `for` and `while` loops.

- **End** End the lines with the `end` keyword

## Built-In Functions

Nakama Script provides a set of built-in functions that you can use to perform various tasks. Here's an overview of the available built-in functions:

### `print(...)`

- **Description:** Prints one or more values to the standard output.
- **Usage:** `print("Hello, World")`

### `print_ret(...)`

- **Description:** Prints one or more values to the standard output and appends a newline character.
- **Usage:** `print_ret("This is a line of text")`

### `input(prompt)`

- **Description:** Reads a line of text from the user and returns it as a string.
- **Usage:** `user_input = input("Enter your name: ")`

### `input_int(prompt)`

- **Description:** Reads an integer value from the user and returns it.
- **Usage:** `age = input_int("Enter your age: ")`

### `clear()` or `cls()`

- **Description:** Clears the console screen.
- **Usage:** `clear()` or `cls()`

### `is_number(value)`

- **Description:** Checks if the given value is a number (integer or floating-point).
- **Usage:** `is_number(42)` returns `TRUE`

### `is_string(value)`

- **Description:** Checks if the given value is a string.
- **Usage:** `is_string("Hello, World")` returns `TRUE`

### `is_list(value)`

- **Description:** Checks if the given value is a list.
- **Usage:** `is_list([1, 2, 3])` returns `TRUE`

### `is_function(value)`

- **Description:** Checks if the given value is a Nakama Script function.
- **Usage:** `is_function(my_function)` returns `TRUE`

### `append(list, value)`

- **Description:** Appends a value to the end of a list.
- **Usage:** `my_list = [1, 2, 3]` followed by `append(my_list, 4)`

### `pop(list, index)`

- **Description:** Removes and returns an element from a list at the specified index.
- **Usage:** `my_list = [1, 2, 3]` followed by `popped_element = pop(my_list, 1)`

### `extend(list, other_list)`

- **Description:** Appends all elements from another list to the end of the given list.
- **Usage:** `list1 = [1, 2, 3]` followed by `extend(list1, [4, 5, 6])`

### `exit()`

- **Description:** Exits the Nakama Script interpreter.
- **Usage:** `exit()` //Best Function

### `len(list)`

- **Description:** Returns the number of elements in a list.
- **Usage:** `my_list = [1, 2, 3]` followed by `length = len(my_list)`

### `run(script)`

- **Description:** Runs another Nakama Script script.
- **Usage:** `run("my_other_script.ns")`

These built-in functions are available for your use and provide essential functionality for your Nakama Script programs.

## Example

Here's a simple example of a Nakama Script program that calculates the Fibonacci sequence:

```ns
gears fibonacci(n) ->
    if n <= 0 then
        return 0
    elseif n == 1 then
        return 1
    else
        return fibonacci(n - 1) + fibonacci(n - 2)
    end
end

nakama n = 10
nakama result = fibonacci(n)
print("Fibonacci sequence ")
print(n)
for i = 1 to n then
    print(fibonacci(i))
end
```
## Output
```
Fibonacci sequence 
10
1
1
2
3
5
8
13
21
34
```

## Contributing
We welcome contributions to Nakama-Script. If you have suggestions, bugs to reports, or want to contribute to the development of the language.

## License
Nakama Script is open-source and released under the MIT License.

## Contact
If you have any questions or need assistance, feel free to contact us at [sahilandhare2004@gmail.com].

Happy coding with Nakama Script! Dont really expect too much of a performance its only my first language so ya it sucks :D
