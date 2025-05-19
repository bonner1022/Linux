# Installing, Updating and Working with Text Editors

## Objectives
- Use sudo command to enable access to "super-user" system administration tools
- Use the apt(system administration) command to update and install two popular packages for text editing: nano and Vim
- Create and edit text files using nano and Vim
- Use Bash to interpret commands included within a text file


## Tasks
### Perform some fundamental system admin operations

We wamt to update our system's package list, upgrade an existing package(nano) and install a new package(vim). 
Managing system tools requires system administration access, which a user can be granted by using the `sudo` 
command and the system password. When installing packages, enter the command `sudo apt update` to ensure all 
package dependencies are up to date before we change any system packages. 

After this action is completed, we use the `sudo apt upgrade nano` command to upgrade nano to the most
up-to-date version. Then we install vim using the `sudo apt install vim` command. Both actions must confirmed
by inputting the system password when prompted. 

### Create and edit a file using nano 
We use an empty project folder to create a new nano file using `nano helloWorld.txt`. We enter some text into the text editor 
and use `ctrl` + `x` to save and exit the editor. The `cat` command is used to display the contents of the file.

<img width="664" alt="text1" src="https://github.com/user-attachments/assets/5a9c2033-5efc-4b1b-aab6-6d4db5fc5db9" />


<img width="667" alt="nano" src="https://github.com/user-attachments/assets/3ad77e7b-ec3d-43d4-b18d-a6ec4d86dfd6" />


### Create and edit a file using vim
We start vim by typing `vim helloWorld2.txt` in the command line, which puts us in command mode. We enter `:i` to enter text insert mode and 
enter some text. To save the file we press `esc` to get back in command mode, `:w` to save the file and `:q` to exit the editor. Again, `cat` 
is used to show results. 

<img width="487" alt="text" src="https://github.com/user-attachments/assets/304f6469-6f97-46ef-9fd3-2036776169b3" />

<img width="496" alt="vim" src="https://github.com/user-attachments/assets/f3b0aaef-e48e-4d3e-8bc4-7e4de9cfa7ce" />



### Use Bash to execute commands from a text file 
We follow the above steps to create a new file, _output.txt_, using vim. When entering text, we include a `echo` command to indicate we want the 
content of the file to output to the terminal using Bash to execute the file. Once the file is saved and vim mode exited,
we use the command line to enter `bash output.txt` and the contents of the file are displayed in the terminal.

<img width="527" alt="bash" src="https://github.com/user-attachments/assets/e4cdb5cf-3136-4882-b4d4-1fc4b030a345" />
