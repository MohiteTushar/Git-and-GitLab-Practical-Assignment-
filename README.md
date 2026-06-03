# Git-and-GitLab-Practical-Assignment
This document explains the steps taken to successfully complete the Git and GitLab practical assignment. It covers everything from basic repository setup to advanced tasks like merge conflict resolution and repository mirroring.

Task Execution Details
Task 1: Create a GitHub Repository
Created a new repository on GitHub named git-practice-task.
Set the visibility to Public and initialized it with a default README file.
Screenshot
Task 1: Create a GitHub Repositor
### Task 1: Create a GitHub Repository

#### Steps Performed

* Logged in to GitHub.
* Created a new repository named **git-practice-task**.
* Selected **Public** visibility.
* Initialized the repository with a **README.md** file.
* Created the repository successfully.

#### Verification

✅ GitHub repository created

✅ Repository named **git-practice-task** created

✅ README.md file initialized

✅ Repository set to Public

# Screenshot
<img width="1366" height="768" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/e260062f-4b02-405d-b5bc-9c5981728e08" />


### Task 2: Clone the Repository

#### Steps Performed

* Copied the GitHub repository URL.
* Opened Git Bash.
* Cloned the repository to the local machine using the `git clone` command.
* Verified that the repository was cloned successfully.
* Navigated to the project directory using the `cd` command.

#### Commands Used

```bash
git clone <repository-url>
cd git-practice-task
```

#### Verification

✅ Repository cloned successfully

✅ Repository available on local machine

✅ Navigated to the project directory

✅ Repository contents verified


Task 3: Initial Development on Main Branch
Steps Performed
Opened the cloned repository in the local system.
Updated the README.md file.
Added the assignment title, student name, batch name, and course name.
Saved the changes.
Added the modified file to the staging area.
Committed the changes with an appropriate commit message.
Pushed the changes to the GitHub repository.
Commands Used
git add README.md
git commit -m "Update README with assignment details"
git push origin main
Verification

✅ README.md file updated

✅ Changes committed successfully

✅ Changes pushed to GitHub

✅ Updated content visible in the GitHub repository

Screenshot
<img width="1366" height="768" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/4c32674c-def7-4d77-917d-df14104e3758" />

### Task 4: Create Feature-A Branch

#### Steps Performed

* Created a new branch named `feature-A`.
* Switched to the `feature-A` branch.
* Created a new file named `index.html`.
* Added sample HTML content to the file.
* Saved the file.
* Added the file to the staging area.
* Committed the changes with an appropriate commit message.
* Pushed the `feature-A` branch to GitHub.

#### Commands Used

```bash
git checkout -b feature-A

git add index.html

git commit -m "Add index.html in feature-A"

git push -u origin feature-A
```

#### Verification

✅ feature-A branch created

✅ index.html file added

✅ Changes committed successfully

✅ Branch pushed to GitHub

✅ feature-A branch visible on GitHub
# screenshot
<img width="1366" height="768" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/4789cbef-a483-4593-bce3-e3844fd77638" />

### Task 5: Create a Pull Request

#### Steps Performed

* Opened the GitHub repository.
* Navigated to the Pull Requests section.
* Clicked on **New Pull Request**.
* Selected `feature-A` as the source branch.
* Selected `main` as the target branch.
* Reviewed the changes.
* Added a title and description for the Pull Request.
* Created the Pull Request without merging it.

#### Verification

✅ Pull Request created successfully

✅ Source branch: feature-A

✅ Target branch: main

✅ Changes available for review

✅ Pull Request remains open (not merged)

### Task 6: Create Feature-B Branch

#### Steps Performed

* Created a new branch named `feature-B`.
* Switched to the `feature-B` branch.
* Opened the existing `index.html` file.
* Modified the same lines that were changed in the `feature-A` branch.
* Saved the changes.
* Added the modified file to the staging area.
* Committed the changes with an appropriate commit message.
* Pushed the `feature-B` branch to GitHub.
* Created a Pull Request from `feature-B` to `main`.

#### Commands Used

```bash
git checkout main

git checkout -b feature-B

git add index.html

git commit -m "Modify index.html in feature-B"

git push -u origin feature-B
```

#### Verification

✅ feature-B branch created

✅ index.html modified

✅ Changes committed successfully

✅ feature-B branch pushed to GitHub

✅ Pull Request created from feature-B to main
# screenshot
<img width="1366" height="768" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/da4a7b3d-b346-4d6a-b5f8-d44b64612ab6" />

### Task 7: Merge Feature-A

#### Steps Performed

* Opened the Pull Request created from `feature-A` to `main`.
* Reviewed the changes in the Pull Request.
* Verified that the changes were correct.
* Clicked on **Merge Pull Request**.
* Confirmed the merge.
* Checked the `main` branch to verify that the changes were successfully merged.

#### Verification

✅ Pull Request reviewed

✅ feature-A merged into main

✅ Merge completed successfully

✅ index.html available in main branch

✅ Changes visible in GitHub repository


### Task 8: Handle Merge Conflict

#### Steps Performed

* Attempted to merge the `feature-B` Pull Request into `main`.
* Observed a merge conflict because the same lines in `index.html` had been modified in both branches.
* Pulled the latest changes from the `main` branch.
* Opened the conflicted file and reviewed the conflict markers.
* Manually resolved the conflict by keeping the required changes.
* Added the resolved file to the staging area.
* Committed the conflict resolution.
* Pushed the updated `feature-B` branch to GitHub.

#### Commands Used

```bash
git checkout feature-B

git pull origin main

git add index.html

git commit -m "Resolve merge conflict"

git push origin feature-B
```

#### Verification

✅ Merge conflict detected

✅ Conflict resolved manually

✅ Changes committed successfully

✅ Updated branch pushed to GitHub

✅ Pull Request ready for merge
# Screenshot :conflict
<img width="1366" height="768" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/e53949b0-6343-42e9-a601-890385848d33" />

#Screenshot :resolve Conflict
<img width="1366" height="768" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/59462301-857d-4b3c-bfc3-f9d983167f1a" />
### Task 9: Complete the Merge

#### Steps Performed

* Opened the Pull Request for `feature-B`.
* Verified that all merge conflicts had been resolved.
* Reviewed the updated changes.
* Clicked on **Merge Pull Request**.
* Confirmed the merge operation.
* Checked the `main` branch to ensure the merged changes were available.
* Verified that changes from both `feature-A` and `feature-B` were present.

#### Verification

✅ Merge conflict resolved successfully

✅ feature-B Pull Request merged

✅ Changes from feature-A available in main

✅ Changes from feature-B available in main

✅ Main branch updated successfully
 screemshot
 <img width="1366" height="768" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/9815affc-2ea7-4af0-bde9-ef50232e0c99" />


### Task 10: Fork and Contribute

#### Steps Performed

* Selected a public GitHub repository.
* Clicked the **Fork** button to create a personal copy.
* Cloned the forked repository to the local machine.
* Opened the repository and modified the `README.md` file.
* Added a small update to the documentation.
* Committed the changes with an appropriate commit message.
* Pushed the changes to the forked repository.
* Created a Pull Request from the updated branch to the fork repository.

#### Commands Used

```bash
git clone <fork-repository-url>

cd <repository-name>

git add README.md

git commit -m "Update README file"

git push origin main
```

#### Verification

✅ Public repository forked successfully

✅ Fork cloned to local machine

✅ README.md updated

✅ Changes committed and pushed

✅ Pull Request created successfully


 Screenshot 
 <img width="1366" height="768" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/f80e2c2c-6967-4434-88f4-65a83aea319d" />

 ### Task 11: GitLab Repository Setup

#### Steps Performed

* Logged in to GitLab.
* Created a new private repository.
* Generated and configured an SSH key for GitLab authentication.
* Cloned the GitLab repository locally using the SSH URL.
* Created the required project structure.
* Added the project files.
* Committed the changes to the local repository.
* Pushed the changes to the GitLab repository.

#### Project Structure

```text
project/
├── src/
│   └── app.py
├── docs/
│   └── guide.md
└── README.md
```

#### Commands Used

```bash
git clone git@gitlab.com:username/project.git

cd project

mkdir src docs

touch src/app.py
touch docs/guide.md
touch README.md

git add .

git commit -m "Add project structure"

git push origin main
```

#### Verification

✅ Private GitLab repository created

✅ Repository cloned using SSH

✅ Project structure created

✅ Files committed successfully

✅ Changes pushed to GitLab

✅ Repository contents visible on GitLab


 Screenshot
 <img width="1366" height="768" alt="Screenshot (85)" src="https://github.com/user-attachments/assets/e651f8a6-471e-4abe-ac66-0e4cd5d893c8" />

### Task 12: Repository Mirroring

#### Steps Performed

* Opened the GitLab repository settings.
* Navigated to **Settings → Repository → Mirroring Repositories**.
* Configured the GitHub repository as the mirror target.
* Selected **Push Mirroring**.
* Added GitHub authentication credentials (Personal Access Token or SSH key).
* Saved the mirroring configuration.
* Made a change in the GitLab repository.
* Committed and pushed the changes to GitLab.
* Verified that the changes were automatically synchronized to GitHub.

#### Verification

✅ Repository mirroring configured

✅ GitHub repository added as mirror target

✅ Changes pushed to GitLab

✅ Changes automatically synchronized to GitHub

✅ Mirroring status successful


Scerrnshot
<img width="1366" height="768" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/cab98c41-687a-4c0b-98f2-9f1250fd6a85" />
<img width="1366" height="768" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/71e505bc-f883-4c2c-a635-766b9a31cdbd" />

### Task 13: Branch Protection

#### Steps Performed

* Opened the repository settings.
* Navigated to the Branch Protection Rules section.
* Created a protection rule for the `main` branch.
* Restricted direct pushes to the `main` branch.
* Enabled the requirement for changes to be merged through Pull Requests.
* Saved the branch protection settings.
* Attempted to push changes directly to the `main` branch.
* Verified that the push was blocked by the protection rule.

#### Verification

✅ Branch protection rule created

✅ Main branch protected

✅ Direct pushes restricted

✅ Pull Requests required for changes

✅ Unauthorized direct push blocked successfully

Screenshot
<img width="1366" height="768" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/2654d1a7-25ff-4c1e-baa0-b6bb8277c8bf" />
## Assignment Completion Status

| Task | Description                        | Status      |
| ---- | ---------------------------------- | ----------- |
| 1    | GitHub Repository Creation         | ✅ Completed |
| 2    | Repository Clone                   | ✅ Completed |
| 3    | Initial Development on Main Branch | ✅ Completed |
| 4    | Feature-A Branch Creation          | ✅ Completed |
| 5    | Pull Request (feature-A → main)    | ✅ Completed |
| 6    | Feature-B Branch Creation          | ✅ Completed |
| 7    | Merge Feature-A                    | ✅ Completed |
| 8    | Merge Conflict Resolution          | ✅ Completed |
| 9    | Merge Feature-B                    | ✅ Completed |
| 10   | Fork and Contribution              | ✅ Completed |
| 11   | GitLab Repository Setup            | ✅ Completed |
| 12   | Repository Mirroring               | ✅ Completed |
| 13   | Branch Protection Configuration    | ✅ Completed |
| 14   | Final Verification                 | ✅ Completed |








