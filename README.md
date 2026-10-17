# COMP3104_Group23_Assignment

Group assignment for COMP3104 DevOps at George Brown Polytechnic, Fall 2026.

## Group Members
- **Leader:** Ramtin Loghmani (101595929) - [GitHub](https://github.com/RamtinLm)
- **Member:** Ghazaleh Azimikorf (101564963) - [GitHub](https://github.com/Ghazalehaz)
- **Member:** Mina Fahim (101507439) - [GitHub](https://github.com/mii1na)
- **Member:** Kamand Rostami (101586296) - [GitHub](https://github.com/Kamand1377)
<!-- each member adds their own line below, same format -->

## Project Description
This repository contains our group assignment for COMP3104 DevOps at George Brown Polytechnic, Fall 2026. The goal was to practice the everyday Git and GitHub workflow that real development teams use, in a safe environment where mistakes are part of learning.

Through this project we practiced:
- **Branching:** each member worked on their own `STUDENTID-Name` branch
- **Pull requests:** every branch was merged into `main` through a reviewed PR
- **Merge conflicts:** resolving conflicts locally when several people edited the same file
- **Continuous Integration:** a GitHub Actions workflow that runs automatically on every push

The repository includes each member's three text files (about George Brown, the DevOps course, and DevOps in the SDLC), the CI workflow in `.github/workflows/`, and a pull request template in `.github/PULL_REQUEST_TEMPLATE.md`.

## Setup Instructions

### Prerequisites

Before starting, make sure Git is installed on your computer and you have a GitHub account. You also need to accept the invitation to the group repository.

### Setup Steps

**1. Configure Git**

Set your name and email so your commits are connected to your GitHub account.

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

**2. Clone the repository**

Download the group project to your computer.

```bash
git clone https://github.com/RamtinLm/COMP3104_Group23_Assignment.git
cd COMP3104_Group23_Assignment
```

**3. Switch to your branch**

Each group member should work on their own branch instead of making changes directly to main.

```bash
git checkout 101507439-Mina
```

If the branch does not exist yet, create it using:

```bash
git checkout -b 101507439-Mina
```

**4. Get the latest changes**

Pull the latest updates from the main branch to keep your work up to date.

```bash
git pull origin main
```

**5. Start working**

After completing these steps, you can edit your assigned files, commit changes, and push them to your branch.

This repository contains only documentation and text files, so there are no additional dependencies or packages to install.

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
In our group project, each member has their own branch. We name our branches using our student ID and name. Our branches are 101595929-Ramtin, 101586296-Kamand, 101507439-Mina, and 101564963-Ghazaleh. We make changes and commit them on our own branches, then push them to GitHub. When our work is done, we open a pull request instead of pushing directly to main. We check the CI results and use a merge commit to add our work to main. We also pull updates from main to avoid conflicts. I think this makes it easier for everyone to work on their own part and check the changes before merging.

## Pull Request Template
Every new pull request is pre-filled from `.github/PULL_REQUEST_TEMPLATE.md`. It has 3 parts:

- **Description:** a short summary of what changed
- **Type of Change:** bug fix, new feature, or documentation update
- **Checklist:** self-review, comments, docs, warnings and tests

Each member fills it in before merging their branch into `main`.

## Merge Conflicts
- Ghazaleh and Mina had a conflict in the Group Members section of README.md. I fixed it by keeping both members' information.
