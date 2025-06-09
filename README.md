# Halide Ray Tracer

A fun tool to experiment with [Halide](https://halide-lang.org/) by generating ray-traced images. This project leverages the Halide language to create visually interesting ray tracing effects while exploring Halide’s capabilities in image processing and computational photography.

> **Note:** This project is written entirely in Rust and uses Halide as a conceptual or experimental backend. It’s intended as a playful exploration rather than a production-ready ray tracer.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage Tutorial](#usage-tutorial)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Features

- **Ray Tracing with Halide:** Explore how Halide’s scheduling and image processing capabilities can be applied to ray tracing.
- **Rust-based Implementation:** Benefit from Rust’s safety and performance while experimenting with Halide ideas.
- **Interactive UI:** The project includes a basic UI (located in the `ui` folder) to help visualize the ray tracing process.
- **Modular Design:** Separated codebase into logical modules:
  - `raytracer`: Core ray tracing logic.
  - `ui`: User interface components for visualization.
  - `offline`: Additional tools or experimental offline processing utilities.

## Prerequisites

Before running the project, ensure you have the following installed on your system:

- **Rust:** [Install Rust](https://www.rust-lang.org/tools/install) (preferably the latest stable version).
- **Cargo:** Comes with Rust – used for building and managing the project.
- **Halide (Optional):** While this project experiments with Halide concepts, full Halide integration is optional. Visit [Halide's website](https://halide-lang.org/) for more information.

## Installation

Clone the repository and navigate into the project folder:

```bash
git clone https://github.com/Yash-Singh-Pathania/Halide-Ray-Tracer.git
cd Halide-Ray-Tracer
```

Build the project using Cargo:

```bash
cargo build --release
```

This command compiles the project in release mode, optimizing performance for the ray tracing application.

## Usage Tutorial

### 1. Running the Ray Tracer

After building the project, run the ray tracer executable:

```bash
cargo run --release
```

You should see output in the terminal as the ray tracer starts processing. Depending on the implementation, it may generate an image file or display a preview window.

### 2. Interacting with the UI

If the project UI is enabled (check the `ui` directory for additional instructions):

- **Launch the UI:**  
  The ray tracer might open a window where you can adjust parameters like camera position, lighting, and rendering settings.
  
- **Adjust Settings:**  
  Use the on-screen controls to tweak ray tracing parameters in real time. Experiment with various settings to see how Halide’s processing affects the final rendered image.

- **Saving Outputs:**  
  Once you’re satisfied with the rendered image, use the provided UI button (or command line flag) to save the output to your desired location.

### 3. Command-line Options

The project may support additional command-line flags. For instance:

- `--config <file>`: Load a custom configuration file.
- `--output <path>`: Specify a custom output directory for rendered images.
- `--help`: Display help information regarding available commands and options.

Run the following to see a full list of options:

```bash
cargo run -- --help
```

### 4. Experimentation and Customization

Feel free to explore and modify the code:

- **In `raytracer`:**  
  Review the core logic of ray tracing, including scene setup, light calculations, and Halide scheduling.
- **In `ui`:**  
  Customize the user interface to better suit your workflow or integrate additional controls.
- **In `offline`:**  
  Use offline utilities for batch rendering or to experiment with different Halide pipelines.

## Project Structure

- **`raytracer/`**  
  Contains the core ray tracing algorithms and Halide integration. This is where most of the computation happens.
  
- **`ui/`**  
  Houses the user interface code. This may include modules for window management, user input handling, and visualization.
  
- **`offline/`**  
  Contains scripts or modules used for non-interactive, batch processing.
  
- **`Cargo.toml` & `Cargo.lock`**  
  Rust’s package management files that define project dependencies and versions.
  
- **`README.md`**  
  This document, providing an overview and usage instructions for the project.

## Contributing

Contributions are welcome! If you have suggestions, feature requests, or improvements, please open an issue or create a pull request. Follow the repository’s guidelines for contributing, and make sure to adhere to the coding standards in place.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- **Halide Community:** For inspiring experimental projects and creative uses of Halide.
- **Rustaceans:** For building a fast and safe language that makes projects like this possible.
- **Contributors:** Thank you to everyone who has contributed ideas or code improvements to this repository.
