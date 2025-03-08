# todo-tracker-cli

# Task Tracker CLI

Task Tracker is a command-line interface (CLI) application designed to help you track and manage your tasks. This project allows you to keep track of tasks you need to do, tasks in progress, and tasks that are completed. It helps you practice your programming skills by working with the filesystem, handling user inputs, and building a simple CLI application.

## Requirements

The application should run from the command line, accept user actions and inputs as arguments, and store the tasks in a JSON file. The user should be able to:

- Add, update, and delete tasks
- Mark a task as in progress or done
- List all tasks
- List tasks by status: done, not done (todo), or in progress

### Constraints:
- You can use any programming language to build this project.
- Use positional arguments in the command line to accept user inputs.
- Use a JSON file to store tasks in the current directory.
- The JSON file should be created if it does not exist.
- Use the native file system module of your programming language to interact with the JSON file.
- Do not use any external libraries or frameworks.
- Handle errors and edge cases gracefully.

## Example Usage

Below are the available commands and their expected behavior:

```sh
# Adding a new task
task-cli add "Buy groceries"
# Output: Task added successfully (ID: 1)

# Updating and deleting tasks
task-cli update 1 "Buy groceries and cook dinner"
task-cli delete 1

# Marking a task as in progress or done
task-cli mark-in-progress 1
task-cli mark-done 1

# Listing all tasks
task-cli list

# Listing tasks by status
task-cli list done
task-cli list todo
task-cli list in-progress
```
## Task Properties
Each task should have the following properties:

- **id**: A unique identifier for the task  
- **description**: A short description of the task  
- **status**: The status of the task (`todo`, `in-progress`, `done`)  
- **createdAt**: The date and time when the task was created  
- **updatedAt**: The date and time when the task was last updated  

These properties should be stored in the JSON file and updated accordingly when changes occur.

---

## Getting Started

### 1. Set Up Your Development Environment
- Choose a programming language (e.g., Python, JavaScript, etc.).
- Ensure you have a code editor or IDE installed (e.g., VSCode, PyCharm).

### 2. Project Initialization
- Create a new project directory for your Task Tracker CLI.
- Initialize a version control system (e.g., Git) to manage your project.

### 3. Implementing Features
Start by creating a basic CLI structure to handle user inputs.  
Implement features incrementally:
- Add a task  
- List tasks  
- Update a task  
- Mark a task as in progress  
- Mark a task as done  
- Delete a task  

### 4. Testing and Debugging
- Test each feature individually to ensure it functions correctly.
- Check the JSON file to verify task storage.
- Debug any issues that arise during development.

### 5. Finalizing the Project
- Ensure all features are implemented and tested.
- Clean up your code and add comments where necessary.
- Write documentation on how to use the Task Tracker CLI.
