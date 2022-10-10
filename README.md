# FMMI
https://medium.com/linkit-intecs/how-to-upload-large-files-to-github-repository-2b1e03723d2

Step 01

Download and install Git on your pc.

Download link:- https://git-scm.com/downloads

Step 02

Then download and install GitLFS on your pc.

Download link: https://git-lfs.github.com/

Step 03

Now clone your GitHub repository to your local machine.
Next, create a new folder in your pc wherever you prefer: this is to clone the copy of your GitHub repository to your pc.

Then right-click the background and click ‘Git Bash Here’ as follows.
Then run the following command in the bash terminal opened.

     $ git clone link you copied
Eg:- $ git clone https://github.com/Newuser/NewRepository.git
Close the bash terminal and, now you have successfully cloned your GitHub repository to your local machine.

Step 04

Go to inside the cloned repository. (If you want to upload the file to another folder already created inside the repository, then go to that folder)

Right-click the background and again click ‘Git Bash Here’.

Run the following command

    $ git lfs track “.fileextension”
Eg: If I want to upload a pdf file, then
    $ git lfs track “.pdf”
Step 05

Then copy the file you want to upload, into repository or folder in the repository.

Step 06

Then run the command,

     $ git add filename.fileextension
Eg:- $ git add TheGuid.pdf
Step 07

We should log into GitHub to push the file to the repository, run the following commands.

     $ git config --global user.email “you@example.com”
Eg:- $ git config --global user.email “123abc@gmail.com”
For this use your email address used in Github account.

     $ git config --global user.name “your name”
Eg:- $ git config --global user.name “George Bernard”
For this use your name in Github account. You can find your email and name in the settings of the Github account.

Then a window will pop out asking your Github email/user name and password. Enter the credentials and submit them.

Step 08

Now run the following command.

     $ git commit -m "commit message"
Eg:- $ git commit -m “add TheGuid.pdf”
Next run,

     $ git push origin master
This command will start the uploading the file.
You will notice the progress of the uploading in the bash terminal as follows

progress of file upload shown in bash terminal
Figure 05: Progress of file upload (Image source: Screenshot by the Author)
After uploading is finished, you may notice the file is uploaded to your GitHub repository, successfully.



