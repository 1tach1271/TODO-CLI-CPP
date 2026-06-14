# Todo CLI

A simple **C++ command-line Todo application** to manage tasks from the terminal.

## Features

* Add new tasks
* Mark tasks as completed
* Swap task positions
* Automatically saves tasks in `~/.todo.db`

## Build

```bash
make
```

## Usage

```bash
./todo
```

Display all tasks.

```bash
./todo add Buy groceries
```

Add a new task.

```bash
./todo swap 1 3
```

Swap two tasks.

```bash
./todo done 2
```

Remove a completed task.

## Storage

Tasks are stored locally in:

```text
~/.todo.db
```
