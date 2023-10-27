# Git Workshop Activity

## Key Points to Cover:

- Initialize and set up a new GitHub repository
- Understand the concept of local and remote repositories
- Learn about committing and pushing changes
- Explore creating and managing branches
- Discuss merging using pull/merge requests
- Cover pulling changes from the remote repository
- Addressing and resolving code conflicts

### Initialize local repository

Create a new folder called norse_mythology. Navigate to the folder using GitBash. Initialize a new GIT repo in the folder (git init).

### Set up GitHub account

Head over to [GitHub](https://github.com/) and set up a new account. 

### Link Local Repo to GitHub Repo

**Create a GitHub Repository:**
   - Head over to [GitHub](https://github.com/).
   - Log in to your GitHub account if you haven't already.
   - Click the "+" icon in the upper right corner and select "New repository."
   - Name your repository (in this case, name it `norse_mythology` to match your local repository).
   - You can choose to set the repository as public or private, add a README, add a .gitignore file, and add a license if needed. These are optional but can be helpful.

**Create an SSH Key (If Not Already Done):**
   - If you haven't already, you'll need to create an SSH key for secure communication between your local repository and the GitHub repository.
   - You can generate an SSH key using the following command in Git Bash or the terminal:
     ```shell
     ssh-keygen -t ed25519 -C "your_email@example.com"
     ```
   - Follow the prompts to generate the key and set a passphrase if desired.

**Add Your SSH Key to GitHub:**
   - Copy your public SSH key using the following command (replace with your actual key):
     ```shell
     cat ~/.ssh/id_ed25519.pub
     ```
   - Go to your GitHub account settings, then "SSH and GPG keys," and add the copied key.

**Add GitHub as a Remote:**
   - In your local Git repository's directory, use the following command to add the GitHub repository as a remote. Replace `repository-url` with the URL of your GitHub repository:
     ```shell
     git remote add origin repository-url
     ```

**Verify the Connection:**
   - To verify that your local repository is connected to the GitHub repository, use the following command:
     ```shell
     git remote -v
     ```
   - This should display the URL of your GitHub repository.

**Push Your Local Repository to GitHub:**
   - Finally, you can push your local repository to GitHub using the following commands:
     ```shell
     git branch -M main # Renames the default branch to 'main' if necessary
     git push -u origin main
     ```

### Create files

Create two .txt files. Name one Characters and the other Locations.
In the Characters file, add Odin, Thor, and Loki on separate lines.
In the Locations file, add Asgard and Midgard on separate lines.
Make sure to save both files.

### Initial commit

Using GitBash, add and commit the new files to the main branch. Use "Initial commit" as the commit message.

### Make changes to files

Amend the Characters file by removing Loki and saving.
Amend the Locations file by removing Midgard and saving.
Add and commit the modified files using an appropriate commit message.

### Push changes to remote

Push the new commits to the remote repository.
Confirm the changes have been pushed by checking on GitHub.

### Create a new local branch

Create a new local branch named new_characters.
Add the name Loki back onto a new line in the characters file.
Commit and push changes on the new branch to the remote repository.

### Set up a pull request on GitHub

Using the new branch, which has been pushed to the remote repo, set up a pull request and show how this can be done.
Discuss code reviewing and what that looks like.
Finally, approve changes and merge new_characters into the main.

### Pull changes to the local repo main branch

Using a git pull, get the changes made to the remote main branch and apply them to the local repo’s main branch.
Delete the new_characters branch from the local repo.

### Create a conflict between two branches

Create new branches called new_location_1 and new_location_2 from the local repo’s main branch.
Checkout new_location_1 and add Midgard on a new line in the Locations file. Save the file and commit the changes.
Switch to new_location_2 and instead of Midgard, add Vanaheim on a new line, save the file, and commit the changes.
Add, commit, and push new_location_1 to the remote repo.
Make a pull request for new_location_1 and merge it into the main branch.
Pull changes to the local main branch once the pull request is complete.

### Get the local repo up-to-date

Pull the changes made to the main branch to the local repo’s main branch.
Delete the local branch new_location_1.
Make sure that new_location_2 is also up-to-date by checking out the branch and merging in the main branch.
This should cause conflicts, which then need to be resolved.
Resolve conflicts. May need to discuss different ways of doing this depending on the IDE used.
Add, commit, and push the newly fixed new_location_2 branch to the remote repository.
Complete a pull request for new_location_2 into the remote repo’s main branch.
Remove any unnecessary local branches and pull changes to the local repository.
