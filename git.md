# Creating Repositories
- Repositories can be created remotely on any Source Code Manager or can be created locally.
## Creating Remote Repository
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

