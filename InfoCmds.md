# Informational Commands

## Objectives - Be able to display the following:
- System and user information
- User and group identity info
- Information about running processes and system resource usage
- The current date and time

In this project, we exhibit the use of some basic commands for providing system and
user information and then provide images to show the results of running these commands. 
We are using a test Linux environment to run these commands, to keep certain info private. 

### Display current user, OS and user/group ID information
We run the `whoami` command to return the username of the current user profile of the test 
environment. This is useful to know which user is currently logged into a system. Then
We run `uname -a` to return the full details of the system's operating system, kernel and 
hardware information. This information is useful to fully understand what system you are 
working with. Then, the `id` command is entered to return user ID and group ID to get 
further identifying information of the current user.

<img width="409" alt="userInfo" src="https://github.com/user-attachments/assets/c11a5741-84fc-4915-96aa-99728ae7fdc1" />

### Display available disk space 
The command `df -h` is ran to display the disk availability in this enviroment. It shows how much
space is being used by the specified mounted file systems.

<img width="614" alt="df" src="https://github.com/user-attachments/assets/0a440eb9-fe9c-463f-8123-b4bda1fbd643" />

### Display information on current running processes and system resources 
We run the `ps -e` command to display all processes running on the system and corresponding
process ID to go with it. We are also able to see how long each process has been running.
Along with `ps`, we run the `top -n 10` command to display a dynamically updating table of the 
top 10 running processes which use the most CPU. This table also let's us observe the usage
of other resources, like memory and running time. We use our personal machine for this data.

<img width="589" alt="ps" src="https://github.com/user-attachments/assets/3b968877-4a8a-4abb-8b12-4db2542f9532" />

<img width="580" alt="top" src="https://github.com/user-attachments/assets/094e02f9-bd20-4e3e-99e6-ea63c5fc98da" />

### Display current date and time
The `date` command is used to display current time and date in different formats. We want to 
displaytime in 24 hour format and give the full date so we use the following command: 
`date "+It's %T on %m/%d/%Y"`.

<img width="500" alt="date" src="https://github.com/user-attachments/assets/07cd93df-732b-4764-a3f9-37f0f67ef741" />
