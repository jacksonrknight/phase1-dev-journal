# Git Command Notes

## Git Flow 
- Need to start with 'git init'
    - initializes new git repositroy

### Step                     Command                    What it does
1.  Check whats changed     'git status'                Shows staged/untraced files

2.  Stage a file            'git add "filename"'        Prepares it for commit

3.  Commit the change       'git commit -m "Message"'   Saves the change to version history 

4.  Push to GitHub          'git push'                  Uploads everything to GitHub


## Branching
### Overview
- branches = parallel timelines
- main branch = official working version
- feature branches = experimental copies where you can try new things
    - experiment works --> merge back to the main
    - doesnt work --> delete it nbd

- Webstie Example
    - 'main branch' = live working website
    - 'add-shopping-cart' branch = experimental new feature
    - 'fix-login-bug' branch = fixing a speific problem

- Why branching metters for devops
    - safety - never brak main codebase 
    - collaboration - multiple people work on different dfeatures simultaneously
    - testing - test features before merging to production
    - rollbacks - easy to undo back changes 

### Basic Commands
    - 'git branch'                      # see all branches (* shows the current)
    - 'git checkout -b new-feature'     # creaste and switch to new branch
    - 'git checkout main                # switchback to main branch
    - 'git merge new-feature            # merge branch into main
    - 'git -d new-feature'              # delete branch after merging