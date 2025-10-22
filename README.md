# Static Web Application: Data Processing and Visualization

## Summary

This static web application processes data from an Excel file (`data.xlsx`), converting it into a CSV format and generating JSON results. Powered by Python, with a focus on data manipulation using Pandas, the processed results are published directly to GitHub Pages. Continuous integration is implemented to ensure code quality and consistency via automated checks.

## Setup

1. **Prerequisites**:
   - Ensure you have Python 3.11+ installed.
   - Ensure you have Pandas 2.3 installed.
   
2. **Repository Setup**:
   - Clone the repository to your local machine.
   - Fix any issues in `execute.py` and commit your changes.

3. **File Conversion**:
   - Convert `data.xlsx` to `data.csv` and commit the CSV file.

4. **GitHub Actions Workflow**:
   - Add the CI workflow under `.github/workflows/ci.yml` with the steps to run Ruff, execute the Python script, and deploy the result to GitHub Pages.
   
5. **Publish to GitHub Pages**:
   - In your GitHub repository, go to Settings > Pages.
   - Set the source to the appropriate branch (usually `main` or `gh-pages`).

## Usage

- **Accessing the Page**:
  - Navigate to the GitHub Pages URL associated with your repository to view the results.

- **Configuration Options**:
  - At the current stage, the application processes data without additional configuration or query parameters.

- **Key Features**:
  - Automatic data processing and conversion from Excel to CSV.
  - Dynamic JSON result generation upon code commits.
  - Automated deployment to GitHub Pages showcasing the latest results.

## Code Explanation

- **Technical Overview**:
  - The application uses a Python script (`execute.py`) for data processing.
  - A CI/CD pipeline automates code checks and deployment using GitHub Actions.

- **Key Libraries**:
  - **Pandas**: Utilized for data manipulation and transformation tasks.

- **Important Algorithms/Logic**:
  - **Data Conversion**: The raw data from `data.xlsx` is read, cleansed, and written into `data.csv`.
  - **Data Execution**: The `execute.py` script processes the CSV into a structured JSON format, which is then published.

## License

This project is licensed under the MIT License.