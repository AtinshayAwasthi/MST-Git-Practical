# 22BDO10007_MST1_Practical
#### 1. Run the status command. Notice how it tells you what branch you are in.
command : git status
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/1acb7157-7bca-4fd8-9cf5-1d7cc9216096)

#### 2. Use the branch command to create a new branch.
command : git branch branchname
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/b8ad667e-429a-4a6c-988b-f62f845bab59)

#### 3. Use the checkout command to switch to it.
command : git checkout branchname
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/fc821f63-41fd-4d5c-9979-670e92d9d9a8)

#### 4. Make a couple of commits in the branch – perhaps adding a new file and/or editing existing ones.
command : touch file1.txt   vi file1.txt   git status   git add file1.txt   git commit -m "message"
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/2458719c-91c2-49f3-b992-a29a2f6af869)

#### 5. Use the log command to see the latest commits. The two you just made should be at the top of the list.
command : git log
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/8aea12f2-e44c-4c70-b786-f524a75cb522)

#### 6. Use the checkout command to switch back to the master branch. Run log again. Notice your commits don’t show up now. Check the files also – they should have their original contents.
command : git checkout main        git log
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/47b9cd9d-89c1-4ec2-aafa-173daec00796)

#### 7. Use the checkout command to switch back to your branch. Use gitk to take a look at the commit graph; notice it’s linear.
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/ce602b90-4f60-4d05-89da-3443037478f4)

#### 8. Now checkout the master branch again. Use the merge command to merge your branch in to it. Look for information about it having been a fast-forward merge. Look at git log, and see that there is no merge commit. Take a look in gitk and see how the DAG is linear.
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/7f50ee82-2af5-469e-818a-f0a55d497c5f)

#### 9. Switch back to your branch. Make a couple more commits.
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/a21d6d45-48f4-4ba4-b68c-2880f278d7c5)

#### 10. Switch back to master. Make a commit there, which should edit a different file from the ones you touched in your branch – to be sure there is no conflict.
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/7781bd94-2c65-4dec-9af2-cc4e360a530f)

#### 11. Now merge your branch again. (Aside: you don’t need to do anything to inform Git that you only want to merge things added since your previous merge. Due to the way Git works, that kind of issue simply does not come up, unlike in early versions of Subversion.)
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/0a06ce83-5962-4ca7-9898-fcbb03aebdb8)

#### 12. Look at git log. Notice that there is a merge commit. Also look in gitk. Notice the DAG now shows how things forked, and then were joined up again by a merge commit.
![image](https://github.com/AtinshayAwasthi/MST-Git-Practical/assets/157672307/ac36e24e-8018-43cc-9d13-948ed02d6836)



