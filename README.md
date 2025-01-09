# codecatalyst-learning
This repository documents my learning journey for Git, GitHub.
Git and GitHub Tasks
1. Introduction to Git:
      What is Git?
      Git is a distributed version control system for tracking changes in source code.
      
      Why use Git for version control?
      Tracks project history.
      Enables collaboration among developers.
      Supports branching for feature development.

2. Setting Up Git
      Git Installed: https://git-scm.com/downloads download here.
      Git Configuration:
      git config --global user.name "Your Name"
      git config --global user.email "Your Email"

3. Git in VS Code:
     Download VS Code:https://code.visualstudio.com/

4. Working with Repositories:
     create a local repository by using terminal:
             mkdir codecatalyst-learning
             cd codecatalyst-learning
             git init

5. create a repository in github.
6. clone github repository into our local system.
      git clone https://github.com/sample/repo.git
7. Git operations used:
       echo "# Codecatalyst Learning" > README.md
       git add README.md
       git commit -m "Added README.md"
       git push
8. Branching and Collaboration:
       git branch secondary-branch
       git switch secondary-branch
       create file in secondary-branch
9.  Merging Changes:
       git switch main
       git merge secondary-branch
10. Merge Conflict:


        i) Create a File and Commit It:
                echo "This is the main branch." > conflict-file.txt
                git add conflict-file.txt
                git commit -m "Initial commit on main branch"
               
        ii)Create a New Branch:
                git branch secondary-branch
                git switch secondary-branch
                
        iii)Edit the File in feature-branch:
                echo "This is a change from the feature branch." > conflict-file.txt
                git add conflict-file.txt
                git commit -m "Change from secondary-branch"
                
        iv)Switch Back to the Main Branch:
                git switch main
                
        v)Edit the Same File in main:
                echo "This is a change from the main branch." > conflict-file.txt
                git add conflict-file.txt
                git commit -m "Change from main branch"
        
        vi)Merge feature-branch into main:
                git merge secondary-branch
    
        viii)add and commit "conflict.txt":
                git add conflict-file.txt
                git commit -m "Resolved merge conflict between main and secondary-branch"
        
        ix) Verify the Merge:
                git log --oneline --graph
     
