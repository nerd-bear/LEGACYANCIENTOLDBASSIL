# ⚠ WARNING! ⚠
**This project is no longer maintained and was not developed to the end. ~~This project may be continued in the future. However, it is more likely that the project will merge as part of another project with https://github.com/nerd-bear/SQS~~ This project has been restared, to see the project visit https://github.com/nerd-bear/Bassil.**


# Bassil Language Project

## Overview

Bassil is a custom programming language project with a lexical analyzer and various utility functions. This project is designed to tokenize and analyze Bassil language code, providing a foundation for further language processing steps.

## Table of Contents

1. [Project Structure](#project-structure)
2. [Features](#features)
3. [Dependencies](#dependencies)
4. [Building the Project](#building-the-project)
5. [Usage](#usage)
6. [File Descriptions](#file-descriptions)
7. [Key Components](#key-components)
8. [Error Handling](#error-handling)
9. [Utility Functions](#utility-functions)
10. [Windows-Specific Features](#windows-specific-features)
11. [Contributing](#contributing)
12. [License](#license)

## Project Structure

The project is organized into several key components:

- `main.cpp`: Entry point of the application
- `lexer.h` and `lexer.cpp`: Lexical analyzer implementation
- `error_report.h` and `error_report.cpp`: Error reporting functionality
- `utils.h` and `utils.cpp`: Utility functions
- `buildInfo.txt`: Compilation and dependency information

## Features

- Lexical analysis of Bassil language code
- Token generation and classification
- Error reporting with line and column information
- Extensive utility functions for string manipulation, file operations, and Windows API interaction
- Console output formatting with ANSI escape sequences
- File association and icon setting for Bassil files

## Dependencies

- Windows operating system (Tested on Windows 10)
- GCC/G++ compiler (Tested with version 13.2.0)
- Windows API libraries: gdi32, user32, shell32

## Building the Project

To build the project, use the following command:

```
g++ ./src/main.cpp ./src/cpp/utils.cpp ./src/cpp/lexer.cpp ./src/cpp/error_report.cpp -o C:/coding-projects/CPP-Dev/bassil/build/Bassil-Main-Build-ORS-A01 -lgdi32 -luser32 -lshell32
```

Optional: Add `-w` flag to remove warnings from the compile message.

## Usage

After building the project, run the executable `Bassil-Main-Build-ORS-A01`. The program will perform lexical analysis on the input file specified in `main.cpp` (default: `C:/coding-projects/CPP-Dev/bassil/input/main.basl`).

## File Descriptions

- `main.cpp`: Contains the `WinMain` function, initializes the application, performs lexical analysis, and handles errors.
- `lexer.h` and `lexer.cpp`: Define token types and implement the lexical analyzer.
- `error_report.h` and `error_report.cpp`: Provide error reporting functionality.
- `utils.h` and `utils.cpp`: Contain various utility functions for string manipulation, file operations, and Windows API interactions.

## Key Components

### Lexical Analyzer

The lexical analyzer in `lexer.cpp` tokenizes input code into the following token types:

- Identifiers
- Keywords (int, char, float, string)
- Literals (integers, floats, strings)
- Operators (arithmetic, comparison, logical)
- Punctuation (parentheses, braces, semicolons, commas)

### Token Structure

Each token contains:

- Type
- Value
- Line number
- Start column
- End column

## Error Handling

The project includes an error reporting system that provides detailed information about lexical errors, including:

- File path
- Line number
- Column number
- Error message

## Utility Functions

The `Utils` namespace in `utils.cpp` provides a wide range of utility functions, including:

- String manipulation (splitting, trimming, formatting)
- File operations (reading, writing, logging)
- Console output formatting with ANSI escape sequences
- Windows API interactions (message boxes, notifications)
- Color and text formatting utilities

## Windows-Specific Features

- Creation of Windows API 32-bit message boxes
- Windows API balloon notifications
- File association and icon setting for Bassil files
- Retrieval of monitor information

## Contributing

Contributions to the Bassil Language Project are welcome. Please ensure that your code adheres to the existing style and includes appropriate documentation and test coverage.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Thanks to all contributors and supporters of the Bassil project.

## Contact
For any queries or suggestions, please open an issue in the GitHub repository.
