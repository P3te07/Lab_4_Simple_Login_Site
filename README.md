# Login Site User Manual
### This program does not work on online compilers!!!

### How to setup your system for the local Flask server:
1. Download the latest Python version. (3.11 is used in this project)
2. Download a compiler. (VS Code works fine for this project)
3. Create a folder where you want your project to be set in.
4. Open VS Code, install any Python drivers (tutorial: https://www.youtube.com/watch?v=cUAK4x_7thA&ab_channel=HarsivoEdu)
5. Open the folder via VS Code. (Open VS Code->Ctrl+O->Select your folder->Click Open/Press Enter)
6. Create a new termial, either from the top tool bar, or you can do it by pressing Ctrl + `.
7. Once the terminal was created, type the following commands:
   ```
   pip install Flask
   ```
   ```
   python -m venv venv
   ```
   Next you have to activate the virtual environment by using the following command.
   On windows:
   ```
   ./venv/Scripts/activate
   ```
   On MacOs or Linux:
   ```
   source venv/bin/activate
   ```
   You may have to disable some windows Powershell restrictions:
 1. Open Windows PowerShell as an admin.
 2. Run the command:
      ```
      Set-ExecutionPolicy RemoteSigned
      ```
   And with that, the server setup is done, now your system acts like a server for the site.

   ### How to setup the database
   For this project, I used neon.tech postgresql database.
  1. Access neon.tech and log in or register.
  2. Create your database
  3. Once you've created the database, in the SQL Editor tab in the left of the screen, make a new wuerry andenter the following code:
      ```
      drop table if exists Users;
Create table Users(
username VARCHAR(255),
email VARCHAR(255) UNIQUE,
password_hash varchar(255)
);
      ```
    Be careful, this code will delete your Users table from the database and create it again, so any data left in there is going to be deleted.
    That's all with the database, we'll come back to it soon.

   ## How to setup the HTML pages.
 1. In the same folder as the project, create 2 more folders, one named templates, and other named static.
 2. In the static folder, move the styles.css file
      ![image](https://github.com/P3te07/Lab_4_Simple_Login_Site/assets/157983079/93df8838-e1b0-4dfc-b883-07a59cac2639)
 3. In the templates folder, move all the HTML files
    ![image](https://github.com/P3te07/Lab_4_Simple_Login_Site/assets/157983079/c2ff895c-10b2-4324-96ac-bdd3ce8ea864)

### This is how you folder is supposed to look like:
![image](https://github.com/P3te07/Lab_4_Simple_Login_Site/assets/157983079/380fd4eb-63c6-4c74-a322-4962725da003)




      

   
       




