# GitSampleRepo
A sample git repo
<br>
This is a sample file to learn basics of git and its working. <br>
If it is the first time you are using  the git, first you have to configure git. To configure Git for the first time, you'll need to set up your identity and preferences globally or per project. Here's how to do it:<br>

1.Set Up Your Identity (Name and Email)(If you have already configured git globally you can skip this part)<br>
  Git requires a name and email address to associate with your commits. These settings are typically done globally, which means they apply to all repositories on your system.Open the terminal and in the bash in VS code(What I have used) - <br>
    Set your name: <br>
      git config --global user.name "Your Name"<br>
    Set your email:<br>
      git config --global user.email "your-email@example.com"<br>
If we type, git config --list ,it will show all configurations we have set. <br>

Now we have completed the configuration part. Let's do initializing a local git repository in our project.<br>
1. Initialize a Local Git Repository<br>
   a.Navigate to your project directory:<br>
     cd /path/to/your/project<br>
   b.Initialize Git:<br>
     git init<br>
2. Create a .gitignore File<br>
   Create a .gitignore file using below command:<br>
     touch .gitignore<br>
  Add the following contents:<br>
    node_modules/<br>
    .env<br>
3. Stage Your Files<br>
   stage all your files to include them in the next commit using<br>
     git add .<br>
4. Commit Your Changes<br>
   git commit -m "your comment/message"<br>
5. Create a Remote Repository on GitHub<br>
    - Click on the "New" button to create a new repository.
    - Give your repository a name (e.g., mern-stack-project).
    - Set the visibility (public or private).
    - You can uncheck the 'Add a README file' column and we can seperatly create it in our project by ourselves.
    - Click on "Create repository."<br>
6. Link the Local Repository to the Remote Repository<br>
  Copy the repository URL from GitHub and run the following command in your bash:<br>
    git remote add origin <your url><br>
7. Rename the brach to main<br>
     If you look to the brach name in your VS code it will be  named as 'master'. But in our git repo the brach name is main. So we have to rename master to main.<br>
      git branch -M main<br>
8. Push changes to the remote repo<br>
     We can push the changes using :<br>
     'git push origin main'<br>
        or<br>
     'git push -u origin main'<br>
         -u means to set upstream, if we are working with the same project we no need to repeatedly write 'origin main'. Once we write this full line, next time we only need to write 'git push'.
     
     


