# __Linux Command Line Notes:__

## pwd
- The full form for pwd is 'print working directory'
- It's function is to print the path in which the user is working at that time.
- Through this command we can find the directory we are working in right now.

## cd 
- the full form for cd is 'change directory'
- As the name suggests, through this command we can change the directory we are working in. But there are different ways to use this command.
- If we simply just write the command cd and press enter, it'll change the working directory to the home directory i.e. usually '/home/'.
- We can use cd in the following ways:
	* cd < path >: 
	- Write the path of the directory you wan't to work after 'cd'. 
	- Then your working directory will be changed to the directory the path you entered lead to.
	- Now use the 'pwd' command you just learned to see are you actually in that directory.
	- for eg: cd /home/Documents/
	
	* cd / :
	- Through this command your current directory will be changed to the root directory which is symbolically represented as '/' according to linux Filesystem Hierarchy Standard(FHS).
	
	* cd .. :
	- Through you can change the current directory to the previous directory according to the hierarchy.
	- This command changes the directory to the file above it, not to the file that you ver previously working on as it can be in completely different path.

	* cd < filename >:
	- This command can be used to change the working directory to any directory that is in the working directory.
	- We can only use this command when the directory we want to go to is inside the present directory.
	- for eg: My current directory is /home/, and i want to go the the 'Downloads' directory. {Downloads directory exists inside the home directory}
		''cd Downloads''

	* cd - :
	- Remember that the 'cd ..' does not take you to the previous directory you were in {here previous directory means the past directory you were working on}. This command solves that problem.
	- Through this command we can change the present directory to the past directory we were working in.
	
- Dont worry if you dont understand some commands, you will fully understand them if you after reading this see the example folder in the repo inside TryHackMe and you actually practice them on a linux 
terminal.
- I personally changed my daily os to Linux from Windows to get to linux more deeply.

## ls
- The full form for the command is 'list directory'.
- By simply using this command, you can list the directories or files i.e. contents present in the directory you are working in.
- Some different ways to use this command are:
	* ls < path >:
	- To do so you enter the path of any directory you want to list contents of in front of the 'ls' command.

	* ls -a:
	- Through this command, you can list all the files, including the hidden ones(their names start with '.') in the directory.

	* ls -l:
	- We can use this command to list the info of each directory the command lists.
	- We can see directories in a long listing format.

	* ls -r:
	- When ever you wan't to list a directory but you want the sorting to be reversed. 
	- By default directories are sorted in an alphabetical order, so by using this command you can list files starting from z to a (reverse alphabetical order).

	* ls -R:
	- Use this when you even want to list the subdirectories of every directory that is listed.
	- It really looks cool when you use this command in the root directory, looks like you are hacking something.

	* ls -t:
	- Using this command we can list the directories sorted according to time (newest to oldest).

- You can mix all these command to create a new one.
	for eg: ls -al or ls -la (both work the same way)
		ls -rl or ls -lr

## touch
- The primary purpose of this command was to change time stamps of files, but now it's mostly used to create files too.
- ways to use this command are as follows:
	* touch < filename >
	- So this command's functioning depends. 
	- If the file you entered already exists, it'll edit it's time stamp to the current one.
	- And if the file you entered does not exists, then the file will be created.
	- you can also use this command on multiple files simulteously.

	* touch -r < reference-filename > < filename >:
	- This command can be used to change the time stamp of last file you entered to that of the reference file.
	
	* touch -d "date-and-time" < filename >:
	- This command allows for presise time stamp management.
	- Use this command to change the time stamp of the file you entered to the date and time you entered in the command.

## file
- The command is used to see the file descryption.

## cat
- The command is primarly used for seeing the contents on file or linking.
	* cat < filename >:
	- See the contents of any file irrespective of it's type, because in linux everything is a file.
	- If you write the names of more than one file, then you will see the combined content of all those files in the order they are written.(concatenation of files)

	* cat > < filename >:
	- Use this command to edit the file contents.
	- After writing the command, press enter and then write whatever you wanna add in the file.
	- When you are done press Ctrl + D to finish.
 
	* Common Option:
	- *-n* -> numbers all the output lines from 1.
	- *-b* -> numbers only the non-empty lines.

## less
