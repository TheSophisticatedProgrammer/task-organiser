# Persistent Data Organizer

A console-based Python project demonstrating file-handling operations by saving and managing entries in a permanent local text file.

## Features

- **Persistent Local Records**: Syncs runtime data to a local text file seamlessly.
- **Fail-Safe Boot Protocol**: Inspects your file directory before loading data to prevent file-missing crashes.
- **Real-Time Savings**: Commits list changes to disk immediately following any updates or removals.

## Prerequisites

- Python 3.x

## How to Run

1. Save the code to a file named `main.py`.
2. Open your system terminal.
3. Run the application:

## Usage Guide

Type one of the explicit operational commands at the console prompt:

* **add**: Append a text entry to your list and automatically back it up to disk.
* **view**: Output all active entries pulled from your local file storage.
* **delete**: Match and purge an entry from the list, rewriting the storage file immediately.
* **quit**: Safely stop the runtime engine loop and close the script.

## Technical Details

- **File I/O Handlers**: Implements context managers (`with open()`) using read (`r`) and write (`w`) access permissions.
- **String Cleaning**: Employs `.strip()` array iterations to clean up trailing newline breaks (`\n`) during data imports.
