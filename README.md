# GitSampleRepo
A sample git repo
<br>
This is a sample file to learn basics of git and its working.
If it is the first time you are using  the git, first you have to configure git. To configure Git for the first time, you'll need to set up your identity and preferences globally or per project. Here's how to do it:

1.Set Up Your Identity (Name and Email)(If you have already configured git globally you can skip this part)
  Git requires a name and email address to associate with your commits. These settings are typically done globally, which means they apply to all repositories on your system.Open the terminal and in the bash in VS code(What I have used) - 
    Set your name: 
      git config --global user.name "Your Name"
    Set your email:
      git config --global user.email "your-email@example.com"
If we type, git config --list ,it will show all configurations we have set. 

Now we have completed the configuration part. Let's do initializing a local git repository in our project.
1. Initialize a Local Git Repository
   a.Navigate to your project directory:
     cd /path/to/your/project
   b.Initialize Git:
     git init
2. Create a .gitignore File
   Create a .gitignore file using below command:
     touch .gitignore
  Add the following contents:
    node_modules/
    .env
3. Stage Your Files
   stage all your files to include them in the next commit using
     git add .
4. Commit Your Changes
   git commit -m "your comment/message"
5. Create a Remote Repository on GitHub
    - Click on the "New" button to create a new repository.
    - Give your repository a name (e.g., mern-stack-project).
    - Set the visibility (public or private).
    - You can uncheck the 'Add a README file' column and we can seperatly create it in our project by ourselves.
    - Click on "Create repository."
6. Link the Local Repository to the Remote Repository
  Copy the repository URL from GitHub and run the following command in your bash:
    git remote add origin <your url>
7. Rename the brach to main
     If you look to the brach name in your VS code it will be  named as 'master'. But in our git repo the brach name is main. So we have to rename master to main.
      git branch -M main
8. Push changes to the remote repo
     We can push the changes using :
     'git push origin main'
        or
     'git push -u origin main'
         -u means to set upstream, if we are working with the same project we no need to repeatedly write 'origin main'. Once we write this full line, next time we only need to write 'git push'.
     
     


