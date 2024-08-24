# To-Do List Application

This is a simple To-Do List application built using OpenGL and GLFW with custom UI components from the `leif` library. The application allows users to manage tasks with varying priorities and track their completion status.

## Features

- **Task Management**: Add, view, and delete tasks.
- **Task Filtering**: Filter tasks by priority (Low, Medium, High) or completion status (In Progress, Completed).
- **Task Prioritization**: Assign priority levels to tasks and sort them accordingly.
- **Custom UI**: Uses a custom UI built with the `leif` library.

## Getting Started

### Prerequisites

- **OpenGL**: Ensure that your system has OpenGL installed.
- **GLFW**: Install GLFW for window creation and context management.
- **CGLM**: CGLM is used for vector math.
- **leif**: A custom UI library for handling UI elements.

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/binoymanoj/task-management-system.git
    cd todo-app
    ```

2. **Build the project**:
    Make sure you have all necessary dependencies installed, then compile the project using your preferred C compiler:
    ```bash
    gcc -o todo todo.c -lglfw -lGL -lleif -lclipboard -lm -lxcb -lX11
    ```

3. **Run the application**:
    ```bash
    ./todo
    ```

## Usage

- **Dashboard**:
  - View all tasks.
  - Filter tasks using the filter bar.
  - Click the "New Task" button to add a new task.
- **New Task**:
  - Enter a task description.
  - Set the priority level (Low, Medium, High).
  - Click the "Add" button to add the task.

## Task Serialization

The application can serialize tasks to a file for persistence. This is done by calling the `serialize_todo_list` function with the desired filename.

## Dependencies

- OpenGL
- GLFW
- CGLM
- leif
