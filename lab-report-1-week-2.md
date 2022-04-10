# Welcome to CSE15L lab

In this this you will first learn how to access to the remote ssh key first and I will walk you through with several steps, and they are:

1. Installing VScode
2. Remotely Connecting
3. Trying Some Commands
4. Moving Files with scp
5. Setting an SSH Key
6. Optimizing Remote Running

**First**, Let's go with how to install VScode first, you will have to go to the website [VScode](https://www.google.com/search?q=vscode&oq=vscode&aqs=chrome..69i57j0i512l4j69i60l3.1329j0j4&sourceid=chrome&ie=UTF-8) and follow to instruciton provided in the website to instal VScode in your computer. 
And after installation, you should be able to see a screen like this: <img width="1027" alt="Screen Shot 2022-04-10 at 12 50 57 PM" src="https://user-images.githubusercontent.com/71100835/162637146-28206563-035c-487a-8804-ff60c7e11d8e.png">

**Second** remotely connecting with ssh key, 
You should be able to find your user specific account in the [Account Lookup Website](https://sdacs.ucsd.edu/~icc/index.php) but before that you have to install [openSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) to enable you connect to other computer remotely. 
Once you find the specific user account, do `ssh cs15lsp22zz@ieng6.ucsd.edu` with zz = your specific account username. Once you log in, you should be able to see a screen like this:<img width="570" alt="Screen Shot 2022-04-10 at 1 04 02 PM" src="https://user-images.githubusercontent.com/71100835/162637620-70b01087-5ad2-44c3-85b4-d979e4a34cd2.png">

**Third**, Try some commends here wich bascially move you between different directory of your computer or the computer you have been accessed to. 


**Fourth** After you successfully log in, here I would teach you how to use scp commends to move a file from your local to your remote directioy.
Via using javac and java commends you would be able to creat a two files with .class and .java file, use the commend scp WhereAmI.java cs15lsp22avz@ieng6.ucsd.edu:~/ with WhereAmI = the name you gave for the file and avz = your specific account username. And after long in, using ls you can see the file being successfully moved in to your remote directory. 
<img width="1019" alt="Screen Shot 2022-04-10 at 1 26 24 PM" src="https://user-images.githubusercontent.com/71100835/162638399-99facb6e-6a41-4111-ad9f-610d216c9ea9.png">
**Fifth** it's always kinda annoyed to insert you password again and agains everytime you try to log in to your remote server right? We are actually able to setup a shortcup and help us to avoid this annoyed process via using **ssh-keygen**
Here are the steps: 
First, in your own cilent, do ssh-keygen
and (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa with user-name = your own computer username
Next it will ask you to enter the passphrase which we will enter none, then it will pop up with something like this: 

<img width="575" alt="Screen Shot 2022-04-10 at 1 35 54 PM" src="https://user-images.githubusercontent.com/71100835/162638711-a7ec0155-73de-4a1d-92a4-d2df0f087283.png">


