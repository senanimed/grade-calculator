# Student Grade Calculator

A simple Python application that calculates a student's average grade,
determines whether the student passes, and assigns a grade category.

## Installation

Install the required dependencies:

python -m pip install -r requirements.txt

## Usage

Example in Python:

from calculator import calculate_average, is_passing, get_grade_category

average = calculate_average()[10][12][14]

print(average)                      # 12.0
print(is_passing(average))          # True
print(get_grade_category(average))  # Good

An average of 10 or higher is a passing grade.

Grade categories:
- Excellent: average >= 16
- Good: 12 <= average < 16
- Average: 10 <= average < 12
- Fail: average < 10

## Run Tests

python -m pytest -v

## Run Linting

python -m flake8 .

## Continuous Integration

GitHub Actions runs linting and tests on pull requests targeting main
and on pushes to main.

Changes to main require a pull request, an approval, and a successful
quality-gate check.