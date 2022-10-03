### Task 1: Demonstrate minimum 15 basic Git command with explanation and screenshot.
<!-- git-init  -->
<details><summary><b>  1. git-init</b></summary>  
  
```
    1. It is used to initialize the repository. 
    2. Once hit enter after this command, a hidden folder '.git' will be created in the target folder. 
    3. It contains all the backlog references of the current git directories history.
```  
![git_init_image](https://user-images.githubusercontent.com/114586341/193465368-f105958e-6df1-4ad2-b334-5fc54ef652e4.png)
</details>


<!-- git config --global user.name  -->
<details><summary><b>  2. git config --global user.name "user_name"</b></summary>

```    
1. It is used to configure the user name of the github account which we going to work with.
2. It is one time activity required at inital phase of git configuration. If required, can change at any time.
```  
![git_config_user_name](https://user-images.githubusercontent.com/114586341/193466984-2194ef38-24fc-4525-a0c9-3c3fa2e0ccd3.png)
</details>



<!-- git config --global user.email "user email id"  -->
<details><summary><b>  3. git config --global user.email "user email id"</b></summary>
  
```
1. It is used to configure the user email ID of the github account which we going to work with.
2. It is one time activity required at inital phase of git configuration. If required, can change at any time.
```
![git_config_user_email](https://user-images.githubusercontent.com/114586341/193468251-51fac83a-5409-4d41-9999-a8a70b35295a.png)
</details>

<!-- git status -->
<details><summary><b>  git status </b></summary>
  
```
1. Once the file saved in IDE, git start tracking the current stage of the file. That is,  whether the file is in working directory or staging area or committed.
2. This 'git status' command is used to know at which stage the file is at. 
3. After this command, it shows the details with description and files with distinguished colors.
4. Files marked with Red color means, it is in working directory area. We can see the description as "Changes not staged for commit:" 
5. Files marked with Green color means, it is in staging area. We can see the description as "Changes to be committed:"
6. Once committed, we can see the description as "nothing to commit, working tree clean" 
```
![git_status](https://user-images.githubusercontent.com/114586341/193469154-d68d17cb-a2d8-42d6-bf90-cb47be1c5006.png)
</details>


<!-- git add <file_name> <.>  -->
<details><summary><b>  git add 'file_name' </b></summary>
  
```
1. It is used to add the changes from working directory to stagging area (pre-commit stage).
2. To add all changes at once, we use (git add .) commad
3. To add changes of particular file, we use (git add file_name) command. Here, file name should be mentioned with extention.

```
![git_add](https://user-images.githubusercontent.com/114586341/193468917-7d166a35-66d4-4bab-834a-9ed17d8e5f34.png)
</details>