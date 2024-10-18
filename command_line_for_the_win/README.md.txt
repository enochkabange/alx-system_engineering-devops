To upload my screenshots to the sandbox environment, I followed these steps:

First, I took all the necessary screenshots of the completed levels as required. Once I had them saved on my local machine, I opened my terminal (or Command Prompt, depending on my operating system) to begin the upload process.

Next, I connected to the sandbox environment using the SFTP command. I typed in sftp username@hostname, replacing username and hostname with the credentials provided to me. After entering my password, I was successfully logged into the SFTP session.

Once connected, I navigated to the specific directory where I wanted to upload my screenshots. I used the command cd /root/alx-system_engineering-devops/command_line_for_the_win/ to change to that directory.

Now it was time to upload the screenshots. I used the put command for each screenshot, like this: put screenshot1.png and put screenshot2.png. If I had multiple screenshots to upload, I could have also used put *.png to transfer all PNG files at once.

After uploading, I confirmed the transfer was successful by using the ls command to list the files in the current directory. I checked to see if my screenshots were there, and they appeared as expected.

Once I verified that everything was uploaded correctly, I exited the SFTP session by typing bye.

Finally, I navigated to my local GitHub repository where the screenshots were saved. I ran git add . to stage the changes, followed by git commit -m "Add screenshots of completed levels" to commit the files. Finally, I pushed the changes to GitHub with git push origin main, making sure to adjust the branch name as needed.

This process allowed me to successfully upload my screenshots to the sandbox environment and keep my GitHub repository updated!