# Python Virtual Environment Setup and Dependency Installation

This guide will help you create a Python virtual environment, install dependencies from a `requirements.txt` file, and manage your environment effectively. It is written with junior developers in mind.

## Prerequisites

Ensure you have installed:
- **Python 3.6 or later**
- **pip**: The Python package installer (usually comes with Python)

## Step 1: Create a Virtual Environment

Navigate to your project directory and run the following command:

```bash
python3 -m venv venv
```

This command creates a virtual environment named `venv`.

## Step 2: Activate the Virtual Environment

Activate your virtual environment with the following commands:

- **On Unix or macOS:**

  ```bash
  source venv/bin/activate
  ```

- **On Windows:**

  ```bash
  venv\Scripts\activate
  ```

When activated, your terminal prompt will display `(venv)` indicating that you are now working inside the virtual environment.

## Step 3: Install Dependencies

If a `requirements.txt` file exists in your project directory, install all required packages with:

```bash
pip install -r requirements.txt
```

This command reads the file and installs each package along with its specified version.

## Step 4: Deactivate the Virtual Environment

When you’re done working, exit the virtual environment by running:

```bash
deactivate
```

Your terminal prompt will return to normal, indicating that you have exited the virtual environment.

## Additional Tips

- **Creating a `requirements.txt` File:**

  To generate a `requirements.txt` file listing all installed packages, run:

  ```bash
  pip freeze > requirements.txt
  ```

- **Upgrading a Package:**

  To upgrade a package to the latest version, run:

  ```bash
  pip install --upgrade package-name
  ```

## Additional Resources

- [Python Virtual Environments Documentation](https://docs.python.org/3/tutorial/venv.html)
- [pip Documentation](https://pip.pypa.io/en/stable/)

