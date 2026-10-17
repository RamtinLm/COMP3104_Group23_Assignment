# COMP3104_Group23_Assignment

Group assignment for COMP3104 DevOps at George Brown Polytechnic, Fall 2026.

## Group Members
- **Leader:** Ramtin Loghmani (101595929) - [GitHub](https://github.com/RamtinLm)
- **Member:** Mina Fahim (101507439) - [GitHub](https://github.com/mii1na)
<!-- each member adds their own line below, same format -->

## Project Description
<!-- Kamand writes this section -->

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
<!-- Ghazaleh writes this section -->

## Pull Request Template
Every new pull request is pre-filled from `.github/PULL_REQUEST_TEMPLATE.md`. It has 3 parts:

- **Description:** a short summary of what changed
- **Type of Change:** bug fix, new feature, or documentation update
- **Checklist:** self-review, comments, docs, warnings and tests

Each member fills it in before merging their branch into `main`.

## Merge Conflicts
<!-- whoever fixes a conflict adds one line: who, which file, what clashed, how it was fixed -->
