# Khateef's Smart File Organizer 🗂️

A lightweight Python command-line tool that sorts files into folders by type. It uses only Python's standard library, so no third-party packages are required.

**Author:** Khateef  
**Language:** Python 3.10+  
**License:** MIT

## Features

- Organizes images, documents, videos, audio, archives, code, installers, and other files.
- Starts in **preview mode** so you can review the plan before anything moves.
- Requires `--apply` to actually move files.
- Avoids overwriting duplicate filenames by adding suffixes such as `(1)`.
- Skips hidden files and only scans the selected folder's direct children.
- Includes automated unit tests.

## Requirements

- Python 3.10 or newer
- No external dependencies

## Run it

Open a terminal in this project folder.

Preview what would happen:

```bash
python file_organizer.py "/path/to/your/folder"
```

Actually organize the files after checking the preview:

```bash
python file_organizer.py "/path/to/your/folder" --apply
```

On Windows, a path can look like:

```powershell
python file_organizer.py "C:\Users\YourName\Downloads"
```

> Tip: Test it on a temporary folder with sample files first. The tool moves files when `--apply` is used; keep a backup of important data.

## Run tests

From the project root:

```bash
python -m unittest discover -s tests -v
```

## Example output

```text
Khateef's Smart File Organizer
================================
PLAN   invoice.pdf -> Documents/invoice.pdf
PLAN   photo.png -> Images/photo.png

Summary:
  Documents: 1
  Images: 1

Preview only. Add --apply to move the listed files.
```

## GitHub upload

1. Create a new GitHub repository named `khateef-smart-file-organizer`.
2. Extract this ZIP on your computer.
3. Upload the files and folders inside the extracted project to the repository (not the ZIP itself).
4. Add a short repository description, such as: `A safe Python CLI tool to organize files by type with preview mode and duplicate protection.`

Project metadata and documentation identify Khateef as the author/maintainer. Review and understand the code before presenting it in your portfolio, and be ready to explain how it works. Replace `YOUR-GITHUB-USERNAME` in `pyproject.toml` with your actual GitHub username after creating the repository.
