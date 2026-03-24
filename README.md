# CI/CD Starter Repo (Python + pytest + GitHub Actions)

This starter repository is designed for students learning **CI/CD with an emphasis on testing**.

## What's Included
- A small Python package with a few simple functions
- Unit tests using `pytest`
- A GitHub Actions workflow that runs tests on every push and pull request

## Project Structure
```text
ci-cd-starter-repo/
├── .github/
│   └── workflows/
│       └── ci.yml
├── app/
│   ├── __init__.py
│   └── calculator.py
├── tests/
│   └── test_calculator.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Local Setup
1. Create and activate a virtual environment
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run tests:
   ```bash
   pytest -v
   ```

## GitHub Actions
The workflow file lives at:
```text
.github/workflows/ci.yml
```

It will:
- check out the repository
- set up Python
- install dependencies
- run `pytest`

## Suggested Student Extensions
- Add more functions and tests
- Add linting with `flake8` or `ruff`
- Add code coverage
- Add a failing test, then fix the code
