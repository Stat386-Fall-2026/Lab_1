# Lab 1: Getting Set Up

Objective:  Setup the tools that we'll be using this semester in Stat 386.

Instructions: Follow the direction below to get Git, GitHub, uv, and Positron up and running.

Submission: Add a file called complete.txt (this can be an empty file) to the repository. Commit and push to github.

## Install necessary software

### 1. Git
1. Download and install [git](https://git-scm.com/) onto your computer
    * Verify that the installation was successful:
        - On a mac: Open the terminal and type `git --version`.  It should return `git version X.XX.XX` (with the version number)
        - On a PC: Verify that you have "git bash".  Open "git bash" and type `git --version` to verify your version number.

2. Configure git 
    * Configure git on your computer with your name, email, and text editor of choice.
        - git config --global user.name "first last"  
        - git config --global user.email "your_email_here"

---
### 2. uv (Python environment manager)
1. Make sure you have Python 3.11 installed. You can download it from python.org.
2. Install uv
   ```curl -LsSf https://astral.sh/uv/install.sh | sh```
3. Create a new folder for this project (e.g., stat386-lab1) and initialize a virtual environment:
    * In the terminal (Mac) or git bash (Windows) type
    ```mkdir stat386-lab1```
    * Change directories
    ```cd stat386-lab1```
    * Create a new virtual environment
    ```uv venv```
    * Activate the environment:
        * Linux / Mac
          ```source .venv/bin/activate```
        * Windows
          ```.venv\Scripts\activate```
---
### 3. Positron
1. Download and install [Positron](https://positron.posit.co/download)
2. Install the following extensions.  To install an extension, click on the "Extensions" icon on the left most toolbar, search for the extension name in the search bar, and click the "Install" button.  
    * GitHub Pull Requests and Issues
    * Python (by Microsoft)
    * Jupyter (by Microsoft)
3. Sign into GitHub through Positron by clicking on the "GitHub" icon on the left most toolbar and clicking "Sign in". (*Note: You will first need to sign up for a [GitHub](https://github.com) account if you don't have one already*.)

---
### 4. Quarto
1. Download and install Quarto from the official [website](https://quarto.org/docs/get-started/)
2. Verify installation
    * Open a terminal or Git Bash and type
    ```quarto check```
    * You should see a summary confirming that Quarto is installed and integrated with Positron and Jupyter
3. (Optional but recommended) Install the Quarto Positron Extension
    * Search for "Quarto" in the Positron Extensions tab and click "install"

---
---
## Setup Github
1. Create a [Github](https://github.com/) account (if you haven't already done so)
2. Setup your Github profile:
    * Add a picture
    * Add your name
    * Add a brief bio
    * Create a [profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
3. Grant Github access to your computer:
    In order for you to be able "push" changes from your computer to Github, your Github needs to recognize your computer as having permission to do so.  You will need to use ONE of the following methods:
    * OAuth token
    * [SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)


    


