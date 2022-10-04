### Task 1: Demonstrate minimum 15 basic Git command with explanation and screenshot.
collaborators:
1. test1001-github
2. test1002-github

<!-- git clone  -->
<details><summary><b>  1. git clone </b></summary>  
  
```
    syntax: 1. git clone *github repository url*
    1. This command is used to mirroring the github respository to the local system
    2. To clone the repository in local system, 
        - Copy the github repository url
        - Choose the location at local system and open the IDE (vise versa) 
        - Execute the command with copied github respository url.
    3. After this command, the files in repository will cloned to local system.
```  
![git_clone](https://user-images.githubusercontent.com/114586341/193469159-765332cf-39cb-4592-ad9b-1ca12c979934.png)
</details>

<!-- git-init  -->
<details><summary><b>  2. git init</b></summary>  
  
```
    1. This command is used to initialize the repository. 
    2. Once hit enter after this command, a hidden folder '.git' will be created in the target folder. 
    3. It contains all the backlog references of the current git directories history.
```  
![git_init_image](https://user-images.githubusercontent.com/114586341/193465368-f105958e-6df1-4ad2-b334-5fc54ef652e4.png)
</details>

<!-- git config --global user.name  -->
<details><summary><b>  3. git config --global user.name "user_name"</b></summary>

```    
1. This command is used to configure the user name of the github account which we going to work with.
2. Executing this command is the one time activity required at inital phase of git configuration. If required, can change at any time.
```  
![git_config_user_name](https://user-images.githubusercontent.com/114586341/193466984-2194ef38-24fc-4525-a0c9-3c3fa2e0ccd3.png)
</details>



<!-- git config --global user.email "user email id"  -->
<details><summary><b>  4. git config --global user.email "user email id"</b></summary>
  
```
1. This command is used to configure the user email ID of the github account which we going to work with.
2. Executing this command is the one time activity required at inital phase of git configuration. If required, can change at any time.
```
![git_config_user_email](https://user-images.githubusercontent.com/114586341/193468251-51fac83a-5409-4d41-9999-a8a70b35295a.png)
</details>

<!-- git branch master to main  -->
<details><summary><b>  5. git branch -m master main</b></summary>
  
```
1. This command is used to transfer the files from master branch to main.
2. AFter this command, git will create 'main' branch and transfers all files into main and switched to it as active branch.
3. As the main branch in github is named as 'main', it is necessary to match the branch name in git also. 
4. This step is not required, if we select appropriate settings to name the main branch as 'main' during 'git-scm' setup at local machine. 
```
![git_master_to_main](https://user-images.githubusercontent.com/114586341/193469166-d627a269-c9b2-494a-a4fb-b24853855079.png)
</details>

<!-- git status -->
<details><summary><b>  6. git status </b></summary>
  
```
1. Once the file saved in IDE, git start tracking the current stage of the file. That is,  whether the file is in working directory or staging area or committed.
2. This 'git status' command is used to know at which stage the file is at. 
3. After this command, it shows the details with description and files with distinguished colors.
4. Files marked with Red color means, it is in working directory area. We can see the description as "Changes not staged for commit:" 
5. Files marked with Green color means, it is in staging area. We can see the description as "Changes to be committed:"
6. Once committed, we can see the description as "nothing to commit, working tree clean" 
```
![git_status](https://user-images.githubusercontent.com/114586341/193469154-d68d17cb-a2d8-42d6-bf90-cb47be1c5006.png)
![git_status_1](https://user-images.githubusercontent.com/114586341/193548151-5c45c514-5ad8-491b-b391-db5af23e1772.png)
![git_status_2](https://user-images.githubusercontent.com/114586341/193548155-995d03a1-099f-467a-b8ad-e9474ff91d84.png)
</details>

<!-- git add <file_name> <.>  -->
<details><summary><b>7. git add </b></summary>
  
```
1. This command is used to add the changes from working directory to staging area (pre-commit area).
2. To add all changes at once, we use (git add .) commad
3. To add changes of particular file, we use (git add 'file_name') command. Here, 'file name' should be mentioned with extention.

```
![git_add](https://user-images.githubusercontent.com/114586341/193468917-7d166a35-66d4-4bab-834a-9ed17d8e5f34.png)
</details>

<!-- git commit -->
<details><summary><b>  8. git commit -m 'message'</b></summary>
  
```
1. This command is used to confirm the changes and tells git that the file is ready to push to remote location (github)
2. After this command, git will move the file(s) from 'staging area' to 'committed area'
3. Now the file is ready to push from git to remote respository.

```
![git_commit](https://user-images.githubusercontent.com/114586341/193469160-71b77ea5-4a6b-4b11-bbbd-fb1027e61fcf.png)
</details>

<!-- git push -->
<details><summary><b>  9. git push</b></summary>
  
```
syntax: git push 'remote name' 'target repository branch'
1. This command is used to push the committed changes to remote repository
2. Eg.1, git push origin main.
    - It means, git will push the committed changes to 'main' branch in the 'origin' remote.
   Eg.2, git push origin sub_branch.
    - It means, git will push the committed changes to 'sub_branch' in the 'origin' remote.

```
![git_push](https://user-images.githubusercontent.com/114586341/193552798-c98ee82c-6a76-4fcd-9c1d-ba9c64ab670b.png)
</details>


<!-- git pull -->
<details><summary><b>  10. git pull </b></summary>
  
```
Scenraios:
1. Sometimes, we made changes in files at remote itself via browser. Like adding a new line in README.md file at github itself. In such case, it is essential to merge the changes and maintain same details at both git (local files) and github repository.
2. Also, whenever we made changes in other branch of own repository or files in forks repositories, it is necessary to pull the changes to source respository files (by pull requests) to maintain the same level data.

Command:
syntax: git pull 'remote name' 'source repository branch'
1. It is the combination of 'fetch' and 'merge' actions. 
2. This command is used to pull the committed changes from remote repository to local git.
2. Eg., git pull origin main.
    - It means, git will fetch the changes from 'main' branch and merge it to the current directory at local git.
3. Before executing the command, we should ensure the branch, at which we want to pull the repository details.
```
![git_pull](https://user-images.githubusercontent.com/114586341/193469169-099a86a3-b733-4e5d-aafd-661cd7a8f335.png)
</details>

<!-- git branch -->
<details><summary><b>  11. git chekcout -b 'branch name'</b></summary>
  
```
1. It is the combination of creating and switching branch in oneline. Same as
    >> git branch 'branch name'
    >> git checkout 'branch name'
2. After this command, git will create a branch and switched and mark it as active branch.
3. Eg., git checkout -b sub_branch
    - Let us assume, this command executed from 'main' branch.
    - After execution, git created sub_branch and switched and mark it as active branch.
4. To check the list of branches, use command
    >> git branch 
    - The active branch is marked with astrisk (*)
```
![git_branch_switch](https://user-images.githubusercontent.com/114586341/193469158-e562977e-8363-4aeb-8d81-f9251c933b70.png)
</details>

<!-- git restore -->
<details><summary><b>  12. git restore </b></summary>
  
```
syntax: git restore --staged 'file_name' (or) git restore --source 'commit SHA' 'file name'
1. After executing this command, git will move the file from 'staging area' to 'working directory'
2. Eg1:
    >> git restore --staged aboutme.txt
    - It will remove aboutme.txt file from staging area and mark it as 'M'.
  Eg2:
    >> git restore --source 8628daf aboutme.txt
    - It will remove changes made at commit '8628daf' in aboutme.txt file from staging area and mark it as 'M'. 

```
![git_restore](https://user-images.githubusercontent.com/114586341/193469153-df5d7fce-bc8e-493d-9292-5f17b4c3b319.png)
</details>

<!-- git log -->
<details><summary><b>  13. git log </b></summary>
  
```
syntax: git log (or) git log --oneline (or) git log -p
1. This command is used to review all activities which made to repository files.
- git log : listing all changes
- git log --online : list all commits with short notes
- git log -p : list all changes with detailed description of each actions made in files.

```
>> git log --online:
![git_log_oneline](https://user-images.githubusercontent.com/114586341/193469164-411b6a95-dc80-465a-99ed-36e1c58aacb0.png)</details>

<!-- git merge -->
<details><summary><b>  14. git merge 'branch name' </b></summary>
  
```
1. This command is used to merge the content of one branch to another branch
2. To execute this command, firt swtich to target branch
3. Then exectute this command to merge content from source branch to target branch.
4. Eg., git merge sub_branch
    - Let us assume, we going to merge content from sub_branch to main branch
    >> git checkout main (switching to main branch)
    >> git merge sub_branch (merging contents from sub_branch to main branch)

```
![git_merge](https://user-images.githubusercontent.com/114586341/193469168-2401494f-5e4a-41a3-839c-eb4d5a2c7747.png)
</details>

<!-- git diff -->
<details><summary><b> 15. git diff *branch1* *branch2*</b></summary>
  
```
1. This command is used to find the differences between the file of different branches.
2. It is highly useful when we facing merge conflicts

```
![git_diff](https://user-images.githubusercontent.com/114586341/193570126-548bca95-e663-4ed6-ac0c-7666a8a919c3.png)
</details>
