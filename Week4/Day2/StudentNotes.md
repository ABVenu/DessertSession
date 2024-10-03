### Lecture Name

# Version Control and Git Basics

## 1. Introduction to Version Control

### What is Version Control?

- Version control is a system that helps you manage changes to files over time.
- It keeps a record of every modification made to a file, allowing you to revert back to previous versions if needed.

### Importance of Version Control

- **Collaboration**: Multiple people can work on the same project simultaneously without overwriting each other's changes.
- **History Tracking**: It maintains a history of changes, making it easy to track who made what changes and when.
- **Backup and Restore**: If something goes wrong, you can easily restore a previous version of your project.
- **Branching**: Allows you to create separate branches for different features or experiments, without affecting the main project.

---

## 2. Introduction to GitHub

### What is GitHub?

- GitHub is a web-based platform that uses Git for version control.
- It allows developers to store their code in repositories, collaborate on projects, and track changes.

### Features of GitHub

- **Repositories**: A repository (repo) is where your project files are stored. Each repository contains all project files and the revision history.
- **Collaboration**: GitHub facilitates collaboration through features like pull requests, issues, and project boards.
- **Showcasing Work**: Developers can showcase their projects and contributions, making it easier to build a portfolio.

---

## 3. Setting Up Git

### Installing Git

- **Windows**:
  1. Download the Git installer from [git-scm.com](https://git-scm.com/downloads).
  2. Run the installer and follow the instructions.
- **macOS**:
  - Install Git via Homebrew:
    ```bash
    brew install git
    ```
- **Linux**:
  - Use the package manager specific to your distribution, for example:
    ```bash
    sudo apt-get install git   # For Ubuntu/Debian
    ```

### Configuring Git

- Set your username and email for commits:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  ```

---

## 4. Basic Git Commands

### 1. `git init`

- Initializes a new Git repository in your current directory.
- Usage:
  ```bash
  git init
  ```

### 2. `git add`

- Stages changes to be committed.
- You can stage specific files or all changes:
  ```bash
  git add filename.txt      # Stage a specific file
  git add .                 # Stage all changes
  ```

### 3. `git commit`

- Saves your staged changes to the repository.
- Always include a meaningful commit message:
  ```bash
  git commit -m "Your commit message"
  ```

### 4. `git status`

- Displays the state of the working directory and staging area.
- Use this command to see which files are staged, unstaged, or untracked:
  ```bash
  git status
  ```

### 5. `git log`

- Shows the commit history for the repository.
- Use this command to review the changes made over time:
  ```bash
  git log
  ```

---

## 5. Project Documentation

### Importance of Documentation

- Documentation is crucial for helping others understand your project.
- It provides guidance on how to set up, use, and contribute to the project.

### Writing a `README.md`

- A `README.md` file typically includes:
  - **Project Title**: Name of the project.
  - **Description**: A brief overview of what the project does.
  - **Setup Instructions**: Step-by-step guide on how to install and run the project.
  - **Usage Examples**: Code snippets demonstrating how to use the project.

#### Example Structure of a `README.md`:

```markdown
# Project Title

A brief description of your project.

## Installation

Instructions on how to install your project.

## Usage

Examples of how to use the project.

## Contributing

Guidelines for contributing to the project.
```

---

## 6. Hands-On Exercise

### Task:

1. Create a local Git repository.

   - Navigate to your project folder.
   - Run `git init`.

2. Practice the following commands:

   - Use `git add` to stage some changes.
   - Run `git commit` with a descriptive message.
   - Check the status with `git status`.
   - View your commit history using `git log`.

3. Write a `README.md` file for your project.
   - Include a title, description, setup instructions, and usage examples.

---

## 7. Wrap Up and Q&A

- Review the key points discussed in the session.
- Open the floor for any questions to clarify doubts and ensure understanding.

---

Feel free to modify or expand upon any sections as needed!
