# iu
Repository for the IU Assignment

#Some Git Commands
git clone https://github.com/krrish9973/iu.git
git status
git push origin main

git config --global user.email "er.krishna12@gmail.com"
git config --global user.name "Krishna Joshi"
git commit -m "Initial Commit"
git push origin main


#Create a New Branch
git branch develop
git checkout -b develop
git push origin develop  # Push Develop Branch Remotely
git branch --set-upstream-to=origin/develop   #Set develop as a Default Branch


#List Local and remote Branches:
git branch -a

#Check Remote Branches only
git branch -r

#Check Current Branch
git branch
OR
git status



# Clone the repository and switch to the develop branch
git clone <repository-url>         # Clone the repository
cd <repository-name>               # Navigate into the project directory
git checkout develop               # Switch to the develop branch

# Add a new function (local changes assumed)
git add .                          # Stage the changes
git commit -m "Add new function"   # Commit the changes with a descriptive message

# Push the changes to the remote develop branch
git push origin develop            # Push the committed changes to the develop branch

# Create a Pull Request
# (This step is typically done on the Git hosting platform, such as GitHub/GitLab)


# Clone the repository and switch to the develop branch
git clone <repository-url>         # Clone the repository
cd <repository-name>               # Navigate into the project directory
git branch                         # List all branches
git checkout develop               # Switch to the develop branch

# Make local changes (e.g., add a new function)
git status                         # Check the status of the working directory
git add .                          # Stage all changes
git commit -m "Add new function"   # Commit the changes with a message

# Push the changes to the remote repository
git push origin develop            # Push the committed changes to the remote develop branch

# If the push fails due to an outdated branch
git pull origin develop --rebase   # Pull and rebase the latest changes from the remote branch
git push origin develop            # Push your changes again after the rebase
