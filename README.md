🌟 Overview
PythonTool is a cross-platform graphical user interface (GUI) application built with PyQt6 that simplifies the management of Python packages using pip. It provides an intuitive, visually appealing dark-themed interface for installing, updating, and removing Python libraries without needing to touch the command line.

Whether you are a beginner setting up your first Python environment or an experienced developer who wants a quick overview of installed packages and easy bulk operations, this tool makes package management effortless.

✨ Features
📦 Install All Popular Packages – One-click installation of a curated list of the most commonly used Python libraries (requests, django, numpy, pandas, tensorflow, etc.).

🔄 Update All Packages – Automatically detects outdated packages and upgrades them with a single click.

📚 Browse by Category – Explore libraries grouped by categories: Web Development, Data Science, Machine Learning, Testing, Databases, Networking, GUI.

🔍 Search & Check on PyPI – Quickly verify if a package exists on PyPI using the official API.

🧩 Multi-Selection Install – Select multiple libraries from the list and install them together.

⌨️ Manual Installation – Enter any pip command or a Git repository URL (GitHub/GitLab) to install packages not in the list.

✅ Installed Packages Management – View all installed packages with versions, update selected ones, or uninstall them (with confirmation).

📋 Real-time Log Console – All pip output is displayed in a dedicated log window, so you can monitor the progress and errors.

🌙 Dark Theme – A modern dark interface that is easy on the eyes during long coding sessions.

🌐 Bilingual Support – Available in both English and Russian (separate executables).

🚀 Installation
Prerequisites
Python 3.6 or higher installed on your system.

The pip package manager (usually comes with Python).

Steps
Download and extract the archive containing the tool.

Ensure PyQt6 is installed – If not, run the provided PythonToolInstaller.bat (Windows) or install manually:

bash
pip install PyQt6
Launch the application:

For English interface: run PythonToolEnglish.exe

For Russian interface: run PythonToolRussian.exe

💡 If you prefer to run the Python script directly, you can execute PythonToolRussian.py or PythonToolEnglish.py with Python.

🖥️ How to Use
The interface is divided into three tabs:

🏠 Main Tab
Contains buttons for Install all libraries and Update all libraries.

A real‑time log area shows all pip command outputs.

A progress bar appears during operations.

📚 Libraries Tab
Search bar – filter the list of popular packages.

Categories panel – click a category to see only relevant packages.

Libraries list – select one or more packages and click Install selected.

Manual installation – enter a pip command (e.g., pip install requests) or a Git URL (e.g., https://github.com/psf/requests) and click Install.

✅ Installed Tab
Displays all currently installed packages (with versions).

Refresh to update the list.

Select packages and use Update selected or Uninstall selected.

Select all to quickly mark everything.

🔍 Insights from the Code
Threading for Responsiveness – All pip commands run in a separate QThread (PipWorker) so the GUI never freezes.

Queue‑based Logging – Output from the worker is queued and displayed periodically via a timer, ensuring thread‑safe updates.

Smart Command Parsing – The manual input handles plain package names, full pip commands, and Git URLs – it automatically converts them to the appropriate pip install syntax.

Fallback to Subprocess – Uses subprocess.Popen to capture real‑time output, making the log feel live.

Dark Palette – The application overrides the default Qt palette to achieve a consistent dark look, even on Windows.

💡 Why Use This Tool?
Time‑saving – Instead of typing pip install for dozens of packages, install them all at once.

Beginner‑friendly – No need to remember command‑line flags; everything is a click away.

Environment Setup – Perfect for quickly provisioning a new Python development environment with the most essential libraries.

Safe – All operations use standard pip commands under the hood – nothing is hidden or dangerous.

Open Source – The code is transparent and can be modified to suit your needs.

📦 Included Popular Packages (partial list)
requests, django, flask, numpy, pandas, matplotlib, scikit‑learn, tensorflow, torch, beautifulsoup4, selenium, opencv‑python, fastapi, sqlalchemy, pytest, jupyter, scipy, seaborn, plotly, keras, transformers, boto3, celery, redis, pymongo, psycopg2, black, flake8, mypy, and many more.

🧑‍💻 Author’s Note
This tool was created to make Python package management more visual and accessible. The two‑language support (English and Russian) reflects the goal of reaching a wider audience. Future updates may include virtual environment management, requirements.txt import/export, and integration with Conda.

Feel free to contribute or report issues!
