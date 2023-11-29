# link_xcode
Link Xcode project with GitHub

## Check global gitconfig file

- `git config --global --list`
- If the file doesn't exist, create a text file `.gitconfig` in that location
  - `touch .gitconfig`
  - `git config --global user.name "github_username"`
  - `git config --global user.email "github_email"`

## Create a personal access token

- After GitHub login, go to GitHub > Settings > Developer Settings > Personal access tokens > Generate new token (classic)
- Git it a description name, and select at least the required scopes:
  - admin:public_key
  - write:discussion
  - repo
  - user
- Once your token is generated save it somewhere safe since you won't be able to see it again.

## Add your GitHub account to Xcode

- Open Xcode and go to Settings
- In the account tab, click + (add icon) at the bottom left and select `GitHub` from the list
- Enter your username and the personal token, and sign in
- You can see GitHub account has been added

## Create a new Xcode project

- Go to File > New > Project
- Choose a template for the project
- Name the project as you wish and click Next
- Check Create Git repository on my Mac and click Create

## Create remote GitHub repository

- Open Source Control navigator (the second icon in the left top of Xcode), on the Repository tab, right-click on Remotes and then click New "App_Name" Remote
- Fill in the repository name, add a simple description, select the project visibility (public or private) and click Create
- The new repository should appear on you GitHub profile, under Repositories tab

## Add your first commit

- On the menu bar, Integrate > Commit
- The changes will display
- Enter commit message,
- If you want to stage some of them, click M next to the filename, and then click Commit and Push
- Or all of them, click Commit and Push, and then click Stage All and Commit
- M changed to U
- Click Push
