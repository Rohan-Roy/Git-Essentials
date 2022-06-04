# Creating Repositories
- Repositories can be created remotely on any Source Code Manager or can be created locally.
## Creating Remote Repository Using GitHub cli 
- To create a remote repository using github cli, use the following steps:
### Login to github:
    1. Login to github: 
        - gh auth login
    2. When prompted for host, provide GitHub.com(unless Enterprise server is being used)
    3. Select protocol: https or ssh
    4. Follow the remaining steps to authenticate using browser/auth token
### Create Repository:
    1. To create a remote repository interactively:
        - gh repo create
    2. To create non-interactively:
        - gh repo create [<name>] [--public / --private / --internal] - - add -c or --clone to clone the new repository locally.
    3. To create a remote repository from an existing local repository:
        - gh repo create [<name>] --source [<source directory>]
        - By default, the remote repository name will be the name of the source directory. Pass --push to push any local commits to the new repository.

## Creating Remote Repository Using Git cli
    1. To start a new repository locally( a project may already exist locally, but it doesn't have Git yet.), initialize the folder as a git repository:
        - git init
    2. Create a remote repository on some SCM like GitHub.com. Then, add the remote URL to your local git repository:
        -git remote add origin <URL>.
        (The above command stores the remote URL under a more human-friendly name, origin.)
    3. Shape your history into at least one commit by using git add to stage the existing files, and git commit to make the snapshot:
        - [git add <file name>] to add specific file
        - [git add .] to add all files
        - git commit -m <"message">
    4. Once there is at least one commit, the changes can be pushed to the remote and set up the tracking relationship for good with:
        - git push -u origin master.
