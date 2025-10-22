# Analyze

Analyze is a static website application that processes data from an Excel file and generates a JSON result using a Python script. This project includes a CI/CD pipeline using GitHub Actions to ensure code quality and deployment.

## Features
- Converts `data.xlsx` to `data.csv`
- Executes `execute.py` to process the data
- Publishes the result as `result.json` on GitHub Pages
- Integrates code quality checks using Ruff

## Requirements
- Python 3.11+
- Pandas 2.3

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/analyze.git
   cd analyze
   ```
2. Install the required Python packages:
   ```bash
   pip install pandas
   ```

## Usage
1. Ensure `data.xlsx` is in the root directory.
2. Run the script:
   ```bash
   python execute.py
   ```
3. The output will be generated as `result.json` in the CI/CD pipeline.

## GitHub Actions
The CI/CD pipeline is defined in `.github/workflows/ci.yml`. It includes steps to:
- Run Ruff for code quality checks
- Execute the Python script
- Deploy the result to GitHub Pages

## License
This project is not licensed.
