# git_pro

How to start a project with git.

1. Elect a Project Lead
1. Make a list of tasks
1. Distribute the tasks among the team
1. Project lead creates a git repository on github.com
1. Add all team members to the repository
1. protect the main branch with branch protection rules
1. Implement a Git Workflow Procedure to control the development process

## Git Work Flow Procedure for Project Lead

1. Create a new repository on GitHub
   * Go to GitHub and create a new repository.
   * Initialize the repository with a README file.
   * Add a .gitignore file for your project type (e.g., Node, Python, etc.).
   * Add each collaborator as a contributor to the repository.
   * Create a dev branch

   * Add the remote repository
	- ``` git remote add origin <url> ```

1. To Create and add an ingore file using terminal
   * touch .gitignore
   * git add .gitignore

2. Make the initial commit
   * ```git add .gitignore```
   * ```git commit -m "Initial commit"```

1. Push the initial commit to the remote repository
   * ```git push origin dev```


## Git Work Flow Procedure for Collaborator

If the shared repo is on GitHub, the project lead should create a new repo is on github, clone it.
```git clone <url>```

Once the repo is cloned create your feature branch from the dev branch
```
git checkout dev
git checkout -b <branch_name>
```

   

Add pull request to the master branch
	-``` git commit -m "Initial commit" ```

1. Tagging commits
``` git tag -a v"version" -m "msg"```