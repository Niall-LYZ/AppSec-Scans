# AppSec-Scans

This repository provides automated security scanning for Python projects using Bandit and pip-audit.

## Features
- **Bandit**: Scans Python source code for common security issues.
- **pip-audit**: Checks dependencies listed in `requirements.txt` for known vulnerabilities.

## Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

## Installation
1. Clone the repository:
   ```powershell
   git clone https://github.com/Niall-LYZ/AppSec-Scans.git
   cd AppSec-Scans
   ```
2. (Optional) Create and activate a virtual environment:
   ```powershell
   python -m venv venv
   .\venv\Scripts\activate
   ```
3. Install required tools:
   ```powershell
   pip install bandit pip-audit
   ```
   > If you encounter long path errors, enable Windows Long Path support as described [here](https://pip.pypa.io/warnings/enable-long-paths).

## Usage

### 1. Scan source code with Bandit
```powershell
bandit -r src
```

### 2. Audit dependencies with pip-audit
```powershell
pip-audit -r requirements.txt --strict --progress-spinner off
```

## Troubleshooting
- If you see errors about missing commands, ensure Bandit and pip-audit are installed and your Python environment is activated.
- For long path errors, enable Windows Long Path support.

## Contributing
Pull requests and issues are welcome!

## License
This project is licensed under the MIT License.
