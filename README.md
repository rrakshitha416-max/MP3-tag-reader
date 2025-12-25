🎵 MP3 Tag Reader in C

This project is a terminal-based MP3 Tag Reader developed in the C programming language. It parses and extracts metadata information from MP3 files’ ID3 tags, such as song title, artist, album, year, and genre. The system demonstrates file handling, binary data parsing, and structured output display, serving as a foundational multimedia tool.

📌 Project Overview
Manual management of MP3 metadata can be tedious and error-prone. This MP3 Tag Reader automates the process by reading ID3 tags embedded within MP3 files, enabling users to quickly view detailed metadata directly through the command-line interface (CLI). This utility aids in cataloging and organizing digital music collections efficiently without requiring a full media player.

⚙️ Components / Tools Used
C Programming Language

GCC Compiler

Command-line Interface (CLI)

Binary File I/O

Bitwise Operations and Structured Data Parsing

Modular File Structure

📁 File Modules
main.c – Program entry point and user interface

mp3tag.c / mp3tag.h – Core logic for parsing ID3v1 and ID3v2 tags

fileutils.c / fileutils.h – File handling utilities and input validation

utils.c / utils.h – Helper functions for string manipulation and data conversion

Sample MP3 files for testing

README.md – Project documentation

🧠 Working Principle
The system reads MP3 files and identifies embedded ID3 tags—either the older ID3v1 tags at the file’s end or the more complex ID3v2 tags at the beginning. It extracts and decodes key metadata fields such as:

Title

Artist

Album

Year

Genre

Using binary file reading, the program processes fixed-length or variable-length frames and presents the metadata in a formatted terminal output. It supports reading multiple files in batch mode and handles missing or corrupted tags gracefully with appropriate error messages.

🔐 Input Validation & Error Handling
Verifies the file format and ensures it is a valid MP3 file

Checks the presence and version of ID3 tags

Handles incomplete or corrupted tags with user notifications

Validates user inputs for file paths and command-line arguments

Ensures buffer overflows and memory errors are prevented through safe coding practices

💡 Features
✅ Reads and parses ID3v1 and ID3v2 tags from MP3 files

✅ Supports batch processing of multiple files

✅ Clear and formatted display of all key metadata fields

✅ Modular codebase for easy extension and maintenance

✅ Robust file and error handling for real-world usability

✅ Cross-platform compatibility due to standard C libraries

✅ Lightweight and fast execution in CLI environment

