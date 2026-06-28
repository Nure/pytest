# Pytest CI/CD Automation Project

## Project Overview
This project demonstrates a Python-based calculator application backed by an automated testing suite using `pytest`. From a DevOps perspective, it solves the problem of ensuring code quality and preventing regression bugs through automated **CI/CD validation** on every code commit and pull request.

## Architecture Diagram




## Tools Used
- **Language:** Python 3.x
- **Testing Framework:** Pytest
- **CI/CD Engine:** GitHub Actions
- **Version Control:** Git & GitHub

## Features
- **Automated Testing:** Unit tests covering basic arithmetic operations (Addition, Subtraction, Multiplication, Division).
- **Edge Case Validation:** Error handling validation for critical cases like division by zero.
- **CI/CD Pipeline:** Automated GitHub Actions workflow triggered on every push to validate code stability before merging.

## Local Setup
To run this project locally and execute the tests, follow these steps:

1. Clone the repository:
   ```bash
   git clone [https://github.com/shehabkazi-blip/pytest.git](https://github.com/shehabkazi-blip/pytest.git)
   cd pytest
Create and activate a virtual environment (Optional but recommended):

Bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
Install dependencies:

Bash
pip install pytest
Run the test suite locally:

Bash
pytest -v
Deployment Steps
CI/CD Pipeline Configuration
The automation is handled via GitHub Actions. The workflow file is located at .github/workflows/.

Ensure your local changes are pushed to GitHub.

Navigate to the Actions tab in your GitHub repository to view the automated test runner.

The pipeline will automatically:

Set up the Python environment.

Install dependencies (pytest).

Run the command pytest -v.

Environment Variables
(No secret keys or external environment variables are required for this local testing suite.)

Screenshots
Tip: Run your tests locally or check the GitHub Actions tab, take screenshots, and drop the images into a screenshots/ folder to link them below.

1. Local Pytest Execution Success
2. GitHub Actions CI/CD Pipeline Passing
Troubleshooting Notes
Problem: pytest: command not found

Root Cause: pytest package is not installed globally or the virtual environment is not activated.

Solution: Run pip install pytest or make sure you have activated your virtual environment where pytest was installed.

Problem: Python Version Mismatch

Root Cause: GitHub Actions runner version defaults might mismatch old syntax.

Solution: Explicitly defined python-version: '3.10' in the GitHub Actions configuration to ensure consistency.
