# COMP3104_Group23_Assignment

Group assignment for COMP3104 DevOps at George Brown Polytechnic, Fall 2026.

## Group Members
- **Leader:** Ramtin Loghmani (101595929) - [GitHub](https://github.com/RamtinLm)
<!-- each member adds their own line below, same format -->

## Project Description
<!-- Kamand writes this section -->

## Setup Instructions
<!-- Mina writes this section -->

## CI/CD Pipeline
This project uses **GitHub Actions** for continuous integration. The workflow is defined in `.github/workflows/ci.yml`.

- **Triggers:** runs on every push to any branch and on every pull request
- **Runner:** `ubuntu-latest` (a Linux machine hosted by GitHub)
- **Steps:**
  1. Prints which event triggered the job and which OS the runner uses
  2. Checks out the repository with `actions/checkout@v7`
  3. Prints a message confirming the repo was cloned to the runner
- **Results:** every run shows up in the **Actions** tab. On pull requests, the result appears as a check (green = passed) before merging.

## Branching Strategy
<!-- Ghazaleh writes this section -->

## Pull Request Template
<!-- Ramtin writes this section -->

## Merge Conflicts
<!-- whoever fixes a conflict adds one line: who, which file, what clashed, how it was fixed -->
