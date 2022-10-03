### Task 1: Demonstrate minimum 15 basic Git command with explanation and screenshot.
<!-- git clone  -->
<details><summary><b>  1. git clone 'github repository url'</b></summary>  
  
```
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
<details><summary><b>  1. git init</b></summary>  
  
```
    1. This command is used to initialize the repository. 
    2. Once hit enter after this command, a hidden folder '.git' will be created in the target folder. 
    3. It contains all the backlog references of the current git directories history.
```  
![git_init_image](https://user-images.githubusercontent.com/114586341/193465368-f105958e-6df1-4ad2-b334-5fc54ef652e4.png)
</details>

<!-- git config --global user.name  -->
<details><summary><b>  2. git config --global user.name "user_name"</b></summary>

```    
1. This command is used to configure the user name of the github account which we going to work with.
2. Executing this command is the one time activity required at inital phase of git configuration. If required, can change at any time.
```  
![git_config_user_name](https://user-images.githubusercontent.com/114586341/193466984-2194ef38-24fc-4525-a0c9-3c3fa2e0ccd3.png)
</details>



<!-- git config --global user.email "user email id"  -->
<details><summary><b>  3. git config --global user.email "user email id"</b></summary>
  
```
1. This command is used to configure the user email ID of the github account which we going to work with.
2. Executing this command is the one time activity required at inital phase of git configuration. If required, can change at any time.
```
![git_config_user_email](https://user-images.githubusercontent.com/114586341/193468251-51fac83a-5409-4d41-9999-a8a70b35295a.png)
</details>

<!-- git status -->
<details><summary><b>  4. git status </b></summary>
  
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
<details><summary><b>  git add 'file_name'  or git add .</b></summary>
  
```
1. This command is used to add the changes from working directory to staging area (pre-commit area).
2. To add all changes at once, we use (git add .) commad
3. To add changes of particular file, we use (git add 'file_name') command. Here, 'file name' should be mentioned with extention.

```
![git_add](https://user-images.githubusercontent.com/114586341/193468917-7d166a35-66d4-4bab-834a-9ed17d8e5f34.png)
</details>

<!-- git commit -->
<details><summary><b>  git commit (or) git commit -m 'message'</b></summary>
  
```
1. This command is used to confirm the changes and tells git that the file is ready to push to remote location (github)
2. After this command, git will move the file(s) from 'staging area' to 'committed area'
3. Now the file is ready to push from git to remote respository.

```
![git_commit](https://user-images.githubusercontent.com/114586341/193469160-71b77ea5-4a6b-4b11-bbbd-fb1027e61fcf.png)
</details>

<!-- git push -->
<details><summary><b>  git push 'remote name' 'target repository branch'</b></summary>
  
```
1. This command is used to push the committed changes to remote repository
2. Eg.1, git push origin main.
    - It means, git will push the committed changes to 'main' branch in the 'origin' remote.
   Eg.2, git push origin sub_branch.
    - It means, git will push the committed changes to 'sub_branch' in the 'origin' remote.

```
![git_push](https://user-images.githubusercontent.com/114586341/193552798-c98ee82c-6a76-4fcd-9c1d-ba9c64ab670b.png)
</details>


<!-- git pull -->
<details><summary><b>  git pull 'remote name' 'source repository branch'</b></summary>
  
```
Scenraios:
1. Sometimes, we made changes in files at remote itself via browser. Like adding a new line in README.md file at github itself. In such case, it is essential to merge the changes and maintain same details at both git (local files) and github repository.
2. Also, whenever we made changes in other branch of own repository or files in forks repositories, it is necessary to pull the changes to source respository files (by pull requests) to maintain the same level data.

Command:
1. It is the combination of 'fetch' and 'merge' actions. 
2. This command is used to pull the committed changes from remote repository to local git.
2. Eg., git pull origin main.
    - It means, git will fetch the changes from 'main' branch and merge it to the current directory at local git.
3. Before executing the command, we should switch the branch, at which we want to pull the repository details.
```
![git_pull](https://user-images.githubusercontent.com/114586341/193469169-099a86a3-b733-4e5d-aafd-661cd7a8f335.png)
</details>
