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
   * Add a .gitignore template file for your project type (e.g., Node, Python, etc.).
   * Add each collaborator as a contributor to the repository.
   * Create a dev branch

## Git Work Flow Procedure for Collaborator

### Getting Started

Go to the github project and get the clone repo url. And clone it.

```git clone <url>```

### Continued Development

To start a new feature development you need to clone the dev branch into a new feature branch 
```
git checkout dev
git checkout -b <branch_name>
```

Make changes to the code base to meet the requiments of the task.

``` 
//do something 
```

Save your files

Stage and Commit code

```
git add -A
git commit -m "msg"
```

Merge our changes into the most recent version of the dev branch
```
git checkout dev
git pull origin dev
git merge <feature_branch>
```

If code conflicts, resolve them!
> Use the Merge Conflict Tool Reolve conflicts
 Stage and commit conflict resolutions
 ```
 git add -A
 git commit -m "msg"
 ```

 Push our changes to the remote dev branch
 ```
 git push origin dev
 ```

 ### Release Procedure

Tag the release version

``` 
git checkout dev
git tag -a "v1.0.0" -m "msg"
```