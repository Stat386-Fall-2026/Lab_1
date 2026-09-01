# Lab 1: Getting Set Up

## Objective

Set up the tools that we will be using this semester in STAT 386 and verify that your local reproducible data science environment is working correctly.

## Instructions

Follow the directions below to install and configure Git, GitHub, `uv`, Positron, and Quarto. You will then clone your Lab 1 repository, synchronize the project environment, run the supplied quarto document, commit and push your work, and create a completion Issue on GitHub.

## Submission

To complete Lab 1:

1. Successfully set up the required software.
2. Clone and open your Lab 1 repository.
3. Run the supplied quarto document.
4. Commit and push your final changes to GitHub.
5. Create the Lab 1 completion Issue.

---

# Install Necessary Software

## 1. Git

1. Download and install [Git](https://git-scm.com/) onto your computer.

2. Verify that the installation was successful.

   - On a Mac, open the Terminal and type:

     ```bash
     git --version
     ```

     It should return something similar to:

     ```text
     git version X.XX.XX
     ```

   - On a PC, verify that you have **Git Bash**. Open Git Bash and type:

     ```bash
     git --version
     ```

3. Configure Git on your computer with your name and email:

   ```bash
   git config --global user.name "First Last"
   git config --global user.email "your_email_here"
   ```

---
## 2. uv — Python Environment Manager

Make sure Python is installed on your computer. You can download Python from python.org.

Install uv using the instructions for your operating system.

macOS or Linux

Open Terminal and run:
   ```bash

   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

If curl is not available, you can use:

   ```bash
   wget -qO- https://astral.sh/uv/install.sh | sh
   ```

Windows

Open Windows PowerShell.

You can search for PowerShell from the Start menu, then run:

   ```bash
   powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
   ```

If you already have winget installed, you can alternatively run:
   ```bash

   winget install --id=astral-sh.uv -e
   ```

After installation, close and reopen Terminal or PowerShell if necessary.

Verify that uv was installed:

   ```bash
   uv --version
   ```
---

## 3. Positron

1. Download and install [Positron](https://positron.posit.co/download).

2. Install the following extensions. To install an extension, click the **Extensions** icon on the left toolbar, search for the extension name, and click **Install**.

   - GitHub Pull Requests and Issues
   - Python (by Microsoft)
   - Jupyter (by Microsoft)

3. Sign in to GitHub through Positron by clicking the **GitHub** icon on the left toolbar and selecting **Sign in**.

   > You will first need to create a GitHub account if you do not already have one.
   > You could go to "5. Set Up GitHub" to get your account set up in this README.md.
---

## 4. Quarto

1. Download and install Quarto from the official [Quarto website](https://quarto.org/docs/get-started/).

2. Verify the installation by opening a terminal or Git Bash and running:

   ```bash
   quarto check
   ```

   You should see a summary confirming that Quarto is installed.

3. Optional but recommended: install the **Quarto** extension in Positron.

---

## 5. Set Up GitHub

1. Create a [GitHub](https://github.com/) account if you have not already done so.

2. Set up your GitHub profile.

   Consider adding:

   - a profile picture;
   - your name;
   - a brief bio;
   - a [profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

3. Grant GitHub access to your computer.

   In order to push changes from your computer to GitHub, GitHub needs to recognize your computer as having permission to access your account.

   Use one of the following authentication methods:

   - OAuth;
   - [SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

---

# Get the Lab 1 Repository

Clone your Lab 1 repository to your computer.

```bash
git clone <your-lab-1-repository-url>
```

Move into the repository:

```bash
cd <your-lab-1-repository-name>
```

Verify that Git recognizes the repository:

```bash
git status
```

You should now be working inside your local copy of the Lab 1 repository.

---

# Set Up the Project Environment

The Lab 1 repository contains the project configuration needed for this assignment.

From inside the repository, run:

```bash
uv sync
```

This command creates or updates the project environment and installs the Python packages required by the lab.

Open the Lab 1 repository folder in Positron and make sure Positron is using the environment associated with the project.

---

# Run the Supplied Quarto Document

Open main.qmd in Positron.

The document contains supplied Python code that checks the installed version of uv and writes the result to a file named:

finished.txt

You are not expected to write or modify the Python code for this lab. The goal is to verify that Quarto, Python, and uv are set up correctly on your computer.

Open a terminal in Positron and run:

   ```bash
   quarto preview main.qmd
   ```

Confirm that the document runs without errors and that finished.txt is created.

# Commit Your Changes

After confirming that the document runs successfully, stop the Quarto preview by pressing Ctrl + C in the terminal.

Then commit and push your work:

```bash
git add .
git commit -m "Fix Me"
git push
```

After pushing your changes, request a review from the collaborator as instructed.
---

# Create a Lab 1 Completion Issue

After your final work has been pushed, go to the **Issues** tab of your Lab 1 repository.

Create a new Issue using the **Lab 1 Complete** Issue template if it is available.

Use the following information:

**Title**

```text
Lab 1 complete
```

**Message**

```text
@local-llm-user process config-dir: lab01/ in instructor-repo: test-llm-editor-org/sample_instructor_repo
```

The course collaborator should create a new issue asking several questions about your experience. Answer the questions by commenting on the newly created issue.
 
This is the only collaborator interaction required for Lab 1. No code review, file modification, branch, or Pull Request is required from the collaborator.

---

# Before You Finish

Make sure that all of the following are complete:

* [ ] Git is installed and configured.
* [ ] `uv` is installed.
* [ ] Positron is installed and connected to GitHub.
* [ ] Quarto is installed.
* [ ] Your Lab 1 repository is cloned locally.
* [ ] `uv sync` completes successfully.
* [ ] The supplied Quarto document runs without errors.
* [ ] `finished.txt` is created successfully.
* [ ] Your final work is committed.
* [ ] Your final work is pushed to GitHub.
* [ ] You created the Lab 1 completion Issue.
* [ ] You answered the collaborator's questions in the generated Issue.
