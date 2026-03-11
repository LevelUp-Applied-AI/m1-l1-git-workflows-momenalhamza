# Hospital Admission Records Analysis

## Team Members
- Momen Alhamza
- Sara Khalid
- Omar Nasser

## Project Overview
This project analyzes hospital admission records to explore patterns in
patient intake and healthcare operations. The goal is to build a clean,
reproducible project environment that allows team members to collaborate
on data analysis and reporting. The project will support exploratory
analysis and future data-driven insights for hospital admission trends.

## Data Sources
This project uses hospital admission records data for analysis.

Data is not tracked in this repository. See the setup instructions below
for how to obtain and place the data files before running any analysis.

Expected location of raw data files:
data/raw/admissions.csv

## Setup Instructions

Clone the repository:

git clone <repo-url>

Move into the project directory:

cd m1-11-git-workflows-momenalhamza

Create a virtual environment:

python -m venv .venv

Activate the environment:

Mac / Linux:
source .venv/bin/activate

Windows Git Bash:
source .venv/Scripts/activate

Windows CMD:
.venv\Scripts\activate.bat

Windows PowerShell:
.venv\Scripts\Activate.ps1

Install dependencies:

pip install -r requirements.txt

Validate the environment:

python test_environment.py

If everything is correct, the script should print:
Environment OK

## Project Structure

m1-11-git-workflows-momenalhamza/
│
├── README.md                Project overview and setup instructions
├── CHANGELOG.md             Record of project changes
├── AGENTS.md                AI contribution policy
├── requirements.txt         Python dependencies
├── setup.sh                 Automated environment setup
├── test_environment.py      Environment validation script
├── .gitignore               Files excluded from Git
│
├── src/                     Production source code
├── notebooks/               Exploratory notebooks
├── data/                    Data directory (not tracked in Git)
│   └── raw/                 Raw input data
│
└── tests/                   Automated tests

## Contributing

Branch naming convention:
- feature/... for new features
- fix/... for bug fixes
- setup/... for environment or tooling updates

Pull Request process:
1. Create a branch for your change.
2. Run `python test_environment.py` to verify the environment.
3. Ensure no data files or secrets are staged.
4. Open a Pull Request describing what changed and why.

Commit messages should be clear and concise, for example:
- "Add setup script for environment initialization"
- "Update README with setup instructions"

On Windows, run `setup.sh` using Git Bash. If using CMD or PowerShell,
run the setup commands manually.