# Todo CLI

Todo CLI is a simple command line application written in C++ that allows users to manage a list of tasks directly from the terminal. The program stores tasks in a file and allows users to add, remove, and rearrange them easily.

## How it Works

The program keeps all tasks in a file named `.todo.db` located in the user's home directory.  
Each time the program runs, it reads the tasks from this file, applies the requested command, and then saves the updated list back to the file.

If the file cannot be opened for writing, the program prints an error message.

Default file location:

/home/<username>/.todo.db

## Compilation

The project can be compiled using GCC.

Run:

make

This will generate the executable file `todo`.

## Usage

### Display Tasks

Running the program without any arguments shows all tasks currently stored.

Example:

./todo

Output example:

1: Feed the cat  
2: Buy groceries  
3: Clean the floors

### Add a Task

To add a new task, use the `add` command followed by the task description.

Example:

./todo add Feed the dog

Output:

1: Feed the cat  
2: Buy groceries  
3: Clean the floors  
4: Feed the dog

### Swap Two Tasks

The `swap` command exchanges the positions of two tasks.

Example:

./todo swap 2 4

Output:

1: Feed the cat  
2: Feed the dog  
3: Clean the floors  
4: Buy groceries

### Mark a Task as Done

The `done` command removes a task from the list once it is completed.

Example:

./todo done 2

Output:

1: Feed the cat  
2: Clean the floors  
3: Buy groceries

### Invalid Commands

If an incorrect command is entered, the program ignores it and no changes are made to the task list.

## Language Used

C++

## Author

Shashi Yadav
