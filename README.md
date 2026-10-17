# COMP3104_Group23_Assignment

Group assignment for COMP3104 DevOps at George Brown Polytechnic, Fall 2026.

## Group Members
- **Leader:** Ramtin Loghmani (101595929) - [GitHub](https://github.com/RamtinLm)
- **Member:** Mina Fahim (101507439) - [GitHub](https://github.com/mii1na)
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
Every new pull request is pre-filled from `.github/PULL_REQUEST_TEMPLATE.md`. It has 3 parts:

- **Description:** a short summary of what changed
- **Type of Change:** bug fix, new feature, or documentation update
- **Checklist:** self-review, comments, docs, warnings and tests

Each member fills it in before merging their branch into `main`.

## Merge Conflicts
<!-- whoever fixes a conflict adds one line: who, which file, what clashed, how it was fixed -->
