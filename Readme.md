# Overview
-   Git has three states, that the files can reside in:
    - **Modified**: means that the file has changed but it has not been committed to the database yet.
    - **Staged**: means that one has marked a modified file in its current version to go into the next commit snapshot.
    - **Committed**: means that the data is safely stored in the local database.
-   Accordingly Git projects have three main sections:
    - **Working Tree**: It's a single checkout of one version of the project. These files are pulled out of the compressed database in the Git directory and placed on disk to use or modify.
    - **Staging Area**: The staging area is a file, generally contained in the Git directory, that stores information about what will go into the next commit. Its technical name in Git parlance is the “index”, but the phrase “staging area” works just as well.
    - **Git Directory**: The Git directory is where Git stores the metadata and object database for the project. This is the most important part of Git, and it is what is copied when one clones a repository from another computer.

