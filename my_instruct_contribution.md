# Instruction for contribution  
- 1. Make fork in my personal repository.
- 2. Clone my forked repository to your local machine.
    ```bash
    git clone https://github.com/ilbaks/some-forked-repo.git
    cd some-forked-repo
    git remote add upstream https://github.com/original-author/some-forked-repo.git
    ```
- 3. Periodically pull changes from the original repository.
    ```bash
    git fetch upstream
    git merge upstream/main
    ``` 
- 4. Conflict resolution.