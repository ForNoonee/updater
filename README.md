# Version Updater

A simple C++ application that checks for updates, downloads new versions of a specified file, and supports segmented file downloads with progress indication.

## Features

- **Version Checking:** Automatically checks for updates against a remote JSON file.
- **Multi-threaded Downloading:** Downloads files in parallel segments for improved performance.
- **Progress Reporting:** Displays download progress in the console.
- **File Merging:** Merges downloaded segments into a single file.
- **Easy Integration:** Includes a simple JSON handling library for version management.

## Dependencies

- **C++ Compiler:** Ensure you have a C++11 compatible compiler.
- **nlohmann/json:** A popular JSON library for C++. Make sure to include it in your project.


Configuration
Current Version: You can specify the current version of your application by changing the currentVersion string in the source code.
Version Information JSON: The expected structure of your version.json file should be as follows:
{
    "version": "1.0.1", // The latest version number
    "url": "https://your-domain.com/path/to/your/newfile.exe", // URL to download the new file
    "filename": "newfile.exe" // The filename for the downloaded update file
}
