# Hello World

## Story

No debate that your first programming exercise must be a [Hello, World!](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) implementation. However, we don't want to bore you - let's be bold and and make your "Hello, World!" shine!

## What are you going to learn?

- Write strings to the console (that is, _printing_).
- Define and call functions.
- Use return values.
- Get user input.
- Call functions with arguments.
- Separate concerns.

## Tasks

1. Modify `helloworld.sh` so that it prints out `Hello, World` to the console. Do not write any functions yet.
    - Running `helloworld.sh` prints out `Hello, World!` to the console.
    - The source code of `helloworld.sh` contains no function definitions.

2. Create and call a function in `hellofunction.sh` which prints `Hello, World!` to the console.
    - Running `hellofunction.sh` prints out `Hello, World!` to the console.
    - The source code of `hellofunction.sh` defines and calls a `say_hello()` function which is responsible for printing the `Hello, World!` message.

3. Create and call two functions in `helloreturn.sh` - one should return the `Hello, World!` string to the another which prints this message to the console.
    - Running `helloreturn.sh` prints out `Hello, World!` to the console.
    - The source code of `helloreturn.sh` defines a `get_hello_message()` function which does not print anything but `echo` the `Hello, World!` message.
    - The source code of `helloreturn.sh` defines and calls a `say_hello()` function which is responsible for printing the message returned by `get_hello_message()`.

4. Create and call two functions in `helloinput.sh` - one should ask for the name of the user and an another which prints the custom greeting message to the console.
    - Running `helloinput.sh` prints `What's your name?`, asks for user input, and using the input prints `Hello, <name>!` to the console.
    - Running `helloinput.sh` asks `What's your name?`, and if the user does not enter anything, it prints `Hello, World!` to the console.
    - The source code of `helloinput.sh` defines a `get_hello_message()` function which prints `What's your name?`, and returns `Hello, <name>!` using the user input (or `Hello, World!` for an empty input).
    - The source code of `helloinput.sh` defines and calls a `say_hello()` function which is responsible for printing the message returned by `get_hello_message()`.

5. Capitalize the user's diplayed name in a reorganized `helloargument.sh` that separates the input collection and the message assembly parts.
    - Running `helloargument.sh` prints `What's your name?`, asks for user input, and using the input prints `Hello, <Name>!` to the console (`<Name>` is capitalized).
    - Running `helloargument.sh` asks `What's your name?`, and if the user does not enter anything, it prints `Hello, World!` to the console.
    - The source code of `helloargument.sh` defines a `get_user_name()` function which prints `What's your name?`, and returns the capitalized version of the user's input string.
    - The source code of `helloargument.sh` defines a `get_hello_message()` function which returns `Hello, <name>!` using the incoming argument (or `Hello, World!` for an empty argument).
    - The source code of `helloargument.sh` defines and calls a `say_hello()` function which is responsible for printing the message after collecting the returned values from the other two functions.

## General requirements

None

## Hints

- If you know how to compile your source and run your class files from the command line,
you are very close to writing a starter script. Here are the steps to follow:
  - Create a new file in a text editor and name it as required (`make.sh` / `make.ps1`).
  - If you are using Linux, put `#!/bin/sh` as the first line (this tells the system how to run this file).
  - Copy the two commands into the next two lines that you used for compilation and running.
  - Save the file, and make it runnable on your OS.
  - Run it!
  - Try to fix the above script to pass an "outside" argument to the command that starts your application. You can find more about this in the Background materials section.


## Background materials

- <i class="far fa-exclamation"></i> [A step-by-step solution guide](project/curriculum/materials/pages/guides/hello-world--general.md)
- <i class="far fa-exclamation"></i> [Variables](https://www.shellscript.sh/variables1.html)
- <i class="far fa-exclamation"></i> [Functions](https://www.shellscript.sh/functions.html)
- <i class="far fa-exclamation"></i> [Variables part2](https://www.shellscript.sh/variables3.html)
- <i class="far fa-book-open"></i> [Quick reference](https://www.shellscript.sh/quickref.html)

