# yijia_ids706_miniProj7

# Rust Template

This project is a simple statistical tool built with Rust that calculates the mean and median of a list of numbers. The tool is packaged with a Makefile for easier management of tasks, including building, testing, linting, and formatting. CI/CD is implemented via GitHub Actions.

## CI/CD Badge

## File Structure

- **`.devcontainer/`**: Contains the development container configuration (`devcontainer.json` and a Dockerfile) to ensure a consistent development environment.
- **`Makefile`**: Provides commands for setting up, building, testing, linting, and formatting the project.
- **`.github/workflows/`**: Contains the CI/CD pipeline (GitHub Actions workflow) that triggers on push and pull requests for tasks like linting, formatting, and testing.
- **`src/`**: Contains the source code for the Rust tool, including the main.rs and lib.rs files.
- **`tests/`**: Contains the test cases for the statistical functions, ensuring that the tool works correctly.


## Installation

1. Ensure you have Rust and Cargo installed. If not, visit [rust-lang.org](https://www.rust-lang.org/learn/get-started) to install them.

2. Clone the repository

```sh
make build 
```

## Build and Run
To build the project, run:
```sh
make build 
```
To run the tool:
```sh
make run 
```
The tool will prompt you to enter a list of numbers (separated by spaces) and will return the mean and median of those numbers.

## Usage
Here is a list of available commands using the Makefile:
```sh
make format  # Formats Rust files using `cargo fmt`.
make lint    # Lints Rust files using `cargo clippy`.
make test    # Runs tests using `cargo test`.
make build   # Builds the project in release mode using `cargo build --release`.
```

## CI/CD Pipeline
This project uses GitHub Actions for continuous integration. The pipeline automatically:

1. Checks formatting using cargo fmt.
2. Lints the code with cargo clippy.
3. Runs tests using cargo test.
4. Builds the project in release mode using cargo build --release.
