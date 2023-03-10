# How to log into ieng6
**Step 1: Install Visual Studio Code**
* Download VS Code for your operating system from their [website](https://code.visualstudio.com/download)
* Click on the file to install it and follow its instructions

**Step 2: Remotely connect using SSH**
* Find your course specific account by navigating to the [Account Lookup Tool](https://sdacs.ucsd.edu/~icc/index.php)
* Enter your information into the fields:
![Screenshot 2023-01-12 110829](https://user-images.githubusercontent.com/122561679/212160770-873ea940-39fa-4be8-95df-2f940f272616.png)
* Select the appropriate course from "Additional Accounts", which should begin with "cs15l"
* Note the username that appears here:
![Screenshot 2023-01-12 111040](https://user-images.githubusercontent.com/122561679/212160690-841c6a79-aaad-4c0f-8626-3897142c6bca.png)
* Click the "change your password" button
* Once you've entered your new password, select the last field and press enter
* Install [Git for Windows](https://gitforwindows.org/)
* Open Visual Studio Code
* Open Terminal using Terminal --> New Terminal in the top menu, or by entering Ctrl+Shift+`
![Screenshot 2023-01-12 105609](https://user-images.githubusercontent.com/122561679/212157512-515731c9-3ee4-4616-8329-57439246a6a4.png)
* SSH into the ieng6 machine with this command, where "username" is your username:
>  `ssh username@ieng6.ucsd.edu`
* If it is your first time connecting, a message like this will appear. Enter 'yes', then enter your password when prompted
![image](https://user-images.githubusercontent.com/122561679/212160052-eb444f60-ad35-47a1-9639-0ad63d560f73.png)
* You should see a message like this, which confirms you have logged in successfully
![image](https://user-images.githubusercontent.com/122561679/212801846-6ea4a109-688d-4afa-b484-1bede1aaabdf.png)


**Step 3: Run some commands**
* Now that you're logged in, you can try running some commands, such as:

* `ls`: lists files and directories
* ![image](https://user-images.githubusercontent.com/122561679/215671943-68c554f9-507c-4ffd-a770-42699cffa362.png)
* `pwd`: show current working directory
* ![image](https://user-images.githubusercontent.com/122561679/215672049-d1f84db4-08e0-482c-aa9b-88aca056ae12.png)
* `cd`: change the current working directory
* ![image](https://user-images.githubusercontent.com/122561679/215672356-0f78a837-564c-4d0e-92bb-ecd186e34cbc.png)
* `cp`: copy files to directory
* ![image](https://user-images.githubusercontent.com/122561679/215672507-63967e85-fb1c-4a84-9d9f-db6b584a7469.png)
* `cat`: print contents of one or several files
* ![image](https://user-images.githubusercontent.com/122561679/215672587-9f1bedf1-ff74-437e-83e3-1b324f4c0300.png)

* When you would like to log out of the server, you can run the command `exit`
* ![image](https://user-images.githubusercontent.com/122561679/215673438-4aa111de-70f2-4e17-a914-0916e84b2abd.png)
