# math456-project
This repo contains the files used in our research project

This guide walks you through installing the required tools, setting up SSH access to GitHub, cloning the repository, and opening the project correctly in RStudio.

 1. Install Required Software
• 	Install RStudio
• 	Install Git - [https://git-scm.com/install/](https://git-scm.com/install/)

 2. Create an SSH Key for GitHub
Open a terminal (Git Bash or RStudio Terminal) and run:
ssh-keygen -t ed25519 -C "your_email@example.com"
Press Enter three times unless you want a custom location or passphrase.

 3. Add Your SSH Key to GitHub
Show your public key:
cat ~/.ssh/id_ed25519.pub
Copy the output.
Then go to:
GitHub → Settings → SSH and GPG Keys → New SSH Key
Paste the key and save.

 4. Clone the Repository
    
Click on the green button in the top right corner - (<> Code). Click on the ssh section.

In RStudio:
Tools → Terminal → New Terminal
(or press Alt + Shift + R)
Go to the directory where you want to clone the repo
Run:
git clone git@github.com:your_username/math456-project.git
You can also clone using a normal system terminal. 

 6. Open the Project in RStudio
In RStudio:
File → Open Project…
Navigate to the cloned folder and open the  file.
This activates Git integration and sets the correct working directory.

 7. Configure Git Identity (First Time Only)
In the RStudio Terminal:

git config --global user.name "Your Name"

git config --global user.email "your_github_email@example.com"

This ensures your commits are linked to your GitHub account.

 9. Start Working
You can now:
• 	Edit the file
• 	Use the Git tab to commit and push
• 	Pull updates from teammates
• 	Work inside a clean reproducible RStudio project environment






