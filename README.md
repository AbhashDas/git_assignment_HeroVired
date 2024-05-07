# Repository Name: git_assignment_HeroVired

## Steps For Q1
- **Clone the repository in the local using the command:**
  - `git clone https://github.com/AbhashDas/git_assignment_HeroVired.git`

- **Create a branch name 'dev' from 'main' branch:**
  - `git checkout -b dev`
- **Create a "Calculator_Plus.py" python file with the given code.**
- **Add and commit the file in the dev branch:**
  - `git add Calculator_Plus.py`
  - `git commit -m "CalculatorPlus App - Version1"`
- **Merge the dev branch to main:**
  - `git checkout main`
  - `git merge dev`
- **Push all the branch and code in remote GIT repository:**
  - `**From main:** git push` //as main branch is already present in github
  - `git checkout dev`
  - `git push --set-upstream origin dev` //dev branch was only created in local repo. So we need to explicilty create a upstream origin for it.`

- **Invite collaborators to your repository.**
- **Create a new branch "feature/sqrt" to implement the Square root feature for the Calculator_Plus app**
  - `git checkout -b feature/sqrt`
- **Update the "Calculator_Plus.py" python file with the square root functionality**
- **Add and commit the new feature:**
  - `git add Calculator_Plus.py`
  - `git commit -m "Implementing the Square Root Feature in CalculatorPlus App"`
- **When the ValueError Bug is reported, checkout to the dev branch to correct the code:**
  - `git checkout dev`
- **Fix the application by adding the appropriate lines**
- **Add and commit the bug fix**
  - `git add Calculator_Plus.py`
  - `git commit -m "Bug Fix for ValueError Exception: Division by Zero"`

- **Create a pull request from dev--> main branch and add a collaborator for reviewing the code from GitHub** 
- **Get the code reviewed by one of the collaborator"**
- **Merge the code from dev --> main**
- **Create a merge request from feature/sqrt --> dev**
- **Merge dev --> main to release the version2 of Calculator_Plus app.**



## Steps for Q2:

- **Create a new branch 'lfs' from main**
  - `git checkout -b lfs`
- **Make sure to install lfs**
  - `git lfs install`
- **Specify which files you want to track specifically as large file. Please share the path to track or copy the file to the present folder:**
  - `git lfs track "*.mp4"` //you can also create .gitattributes file to track multiple file types by adding it here - `git add .gitattributes`
- **Upload a 200mb plus video to the repository**
  -  `git add .`
  -  `git commit -m "Uploading the large file"`
- **Push the code to Github remote repo**
  -  `git push origin lfs`
- **Login to another machine and clone the repository there.**
  - Login to the AWS Instance and clone the repo in /home/ubuntu/
  - check if the large file is downloaded using ls -ltr
- **checkout the branch lfs**
- **Download the marge mp4 file you downloaded.**


## Steps for Q3:
- **Create a new branch 'geometry-calculator'**
  -  `git checkout -b geometry-calculator`
- **Add and commit the python file - geometry-calculator app**
- **Create a new branch 'feature/circlearea'**
  - `git checkout -b feature/circle-area`
- **update the geometry-calculator app, with the circle area feature.**
  -  Add the file to the staging area
  -  Stash the file - `git stash`
  -  Check the list of statsh created - `git stash list`
  -  Check if the working directory is clean - `git status`
- **Checkout to branch - 'geometry-calculator' and create a new branch 'feature/rectanglearea'**
  -  git checkout -b feature/rectanglearea
- **update the geometry-calculator app, with the rectangle area feature.**
  -  Add the file to the staging area
  -  Stash the file - `git stash`
  -  Check the list of statsh created - `git stash list`
  -  Check if the working directory is clean - `git status`
- **Checkout to the branch 'feature/circlearea'**
  - `git checkout feature/circlearea'`
- **Retrieve the change from stash@{0}**
  - `git stash apply stash@{0}`
  - `git add .`
  - `git commit -m ""Update the Feature - Circle area"`
  - `git push origin feature/circlearea`
- **Checkout to the branch 'feature/rectanglearea'**
  - `git checkout feature/rectanglearea'`
- **Retrieve the change from stash@{1}**
  - `git stash apply stash@{1}`
  - `git add .`
  - `git commit -m ""Update the Feature - Rectangle area"`
  - `git push origin feature/rectanglearea`
- **Go to GitHub and generate below pull requests:**
  - feature/circlearea --> dev
  - feature/rectanglearea --> dev
- **Once, approved by team member, run the final pull request below:**
  -  dev --> main




