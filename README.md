# Writing a Compiler in Go

Exercise source code from *Writing a Compiler in Go* by Thorsten Ball. This is an extension of my source code from the first book in this series, *Writing an Interpreter in Go*.

The compiler and virtual machine are an extension of the interpreter built in Go. Monkey source code is still lexed and parsed in a similar fashion, but now compiled to bytecode that gets translated and executed by a virtual machine.

Running a benchmark test with a Fibonacci program written in Monkey confirms that this version of Monkey code execution is about 2.5 times faster!

## Features

The Monkey programming language supports the following:
- Data types: Integers, booleans, and strings
- Data structures: Arrays and hashes
- Functions: User-defined and built-in

Additionally, the Monkey programming language supports closures.

## Usage

To start the REPL and try the Monkey programming language out for yourself, navigate to the `src/monkey` directory and use:
```bash
make repl
```

This will build and compile the REPL and its supporting files.
