🧹 Python Code Formatter
A command-line tool to automatically format Python code in a directory using popular formatters like black, yapf, or autopep8. It also creates backups before modifying files and supports dry runs, directory and file exclusions, and report generation.

📦 Features
Format Python files recursively in a given directory

Choose from black, yapf, or autopep8

Create timestamped backups before changes

Optional dry-run mode (see what would change)

Exclude specific files or directories

Generate a report of formatting activity

🚀 Usage
bash
Copy
Edit
python main.py [directory] [options]
Positional Arguments
directory: Directory to format (default: current directory)

Options
--tool {black,yapf,autopep8}: Code formatter to use (default: black)

--dry-run: Show what would be formatted without making changes

--exclude-dirs dir1 dir2 ...: List of directories to exclude

--exclude-files file1.py file2.py ...: List of files to exclude

Example
bash
Copy
Edit
python main.py ./my_project --tool yapf --exclude-dirs venv tests --exclude-files setup.py --dry-run
📂 Backups
All original files are backed up in a .backups directory with timestamps before formatting.

📄 Report
If not in dry-run mode, a format_report_<timestamp>.txt file is generated listing the formatting activity.

🛠 Requirements
Python 3.6+

One or more of the following tools installed:

black

yapf

autopep8

Install via pip:

bash
Copy
Edit
pip install black yapf autopep8
📌 License
MIT License
