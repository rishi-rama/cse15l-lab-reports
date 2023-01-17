# How to log into ieng6
**Step 1: Install Visual Studio Code**
* Download VS Code for your operatings system from their [website](https://code.visualstudio.com/download)
* Click on the file to install it and follow its instructions

**Step 2: Remotely connect using SSH**
* Find your course specific account by navigating to https://sdacs.ucsd.edu/~icc/index.php
* Enter your information into the fields:
![Screenshot 2023-01-12 110829](https://user-images.githubusercontent.com/122561679/212160770-873ea940-39fa-4be8-95df-2f940f272616.png)
* Select the appropriate course from "Additional Accounts"
* Copy the username that appears here:
![Screenshot 2023-01-12 111040](https://user-images.githubusercontent.com/122561679/212160690-841c6a79-aaad-4c0f-8626-3897142c6bca.png)

* Open Terminal using Terminal --> New Terminal in the top menu, or by entering Ctrl+Shift+`
![Screenshot 2023-01-12 105609](https://user-images.githubusercontent.com/122561679/212157512-515731c9-3ee4-4616-8329-57439246a6a4.png)
* SSH into the ieng6 machine with this command, where "username" is your username:
>  `ssh username@ieng6.ucsd.edu`
* If it is your first time connecting, a message like this will appear. Enter 'yes', then enter your password when prompted
![image](https://user-images.githubusercontent.com/122561679/212160052-eb444f60-ad35-47a1-9639-0ad63d560f73.png)
* You should see a message like this, which confirms you have logged in successfully
* ![image](https://user-images.githubusercontent.com/122561679/212801846-6ea4a109-688d-4afa-b484-1bede1aaabdf.png)


**Step 3: Run some commands**
* Now that you're logged in, you can try running some commands, such as:
```
ls
cd
cp
cat
```

* When you would like to log out of the server, you can run the command `exit`
