# Ournix

This project implements a touch function for a simple filesystem in C. It allows creating new files while ensuring proper structure and validation. The implementation includes memory management, pointer handling, and directory management. The project also includes a testable main function for demonstration.

## Mock Unix Filesystem

This project implements a basic mock Unix-style filesystem in C. It simulates file creation using a **touch** function, which allows users to create new files while maintaining directory structure and validation.

### Features

- **Unix-like Hierarchical Structure**: Files are organized under directories with parent-child relationships.
- **Memory Management**: Uses dynamic memory allocation to create and manage file structures.
- **File Validation**: Ensures that filenames are valid and do not contain restricted characters (e.g., `/`, `.`, `..`).
- **Directory Management**: Supports subdirectories and file linking within the current working directory.
- **Timestamp Updates**: Simulates file system behavior by incrementing timestamps upon file creation.

### Implementation Details

- **file_system struct**: Represents files and directories, storing metadata such as:
  - Name
  - Type
  - Parent
  - Children
- **Ournix struct**: Acts as the filesystem, tracking the current directory.
- **touch function**: 
  - Ensures files are created correctly and inserted into the directory structure.
  - Avoids duplicates within the same directory.
- **main() function**: Demonstrates the functionality by:
  - Initializing a root directory 
  - Creating sample files for testing purposes.

This project serves as a foundation for understanding file system structures and operations in C.

## Usage

To run and test this filesystem:

1. Clone this repository:
   ```sh
   git clone [https://github.com/LIoccoUMD/Ournix.git]
