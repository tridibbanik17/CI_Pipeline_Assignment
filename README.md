<div align="center">


<h3 align="center">Quiz Command-Line Utility</h3>

  <p align="center">
    A simple command-line quiz program written in C.
    <br />
     <a href="https://github.com/tridibbanik17/ci_pipeline_assignment">github.com/tridibbanik17/ci_pipeline_assignment</a>
  </p>
</div>

## Table of Contents

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
      </ul>
    </li>
    <li><a href="#architecture">Architecture</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

This project is a simple command-line quiz program written in C. It presents the user with questions about Linux, C programming, and Git, and checks the user's answers. The program is designed to be interacted with through command-line flags. A GitHub Actions workflow is included to automatically build the program on every push to the `main` branch.

### Key Features

- **Interactive Quiz:** Asks the user questions about Linux, C, and Git.
- **Answer Checking:** Determines if the user's answer is correct.
- **Command-Line Interface:** Uses command-line flags for interaction.
- **CI/CD Pipeline:** Automated build process using GitHub Actions.

## Architecture

The project consists of a single C source file (`quiz.c`) that contains the quiz logic. The `build.yml` file in the `.github/workflows` directory defines the GitHub Actions workflow, which uses `gcc` to compile the C code into an executable named `quiz`. The compiled executable is then uploaded as an artifact.

## Getting Started

### Prerequisites

- A C compiler (e.g., GCC)
- A Linux or macOS environment (for running the compiled executable)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/tridibbanik17/ci_pipeline_assignment
   ```
2. Navigate to the project directory:
   ```sh
   cd tridibbanik17-ci_pipeline_assignment
   ```
3. Compile the C code:
   ```sh
   gcc -o quiz quiz.c
   ```
4. Run the quiz:
   ```sh
   ./quiz -1
   ./quiz -1 "vi"
   ./quiz --help
   ```

## Acknowledgments

- This README was created using [gitreadme.dev](https://gitreadme.dev) — an AI tool that looks at your entire codebase to instantly generate high-quality README files.
