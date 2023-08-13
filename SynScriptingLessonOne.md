Hello Syn! Thanks for accepting the challenge.

You know about terminal and console commands. You have begun to practice using them independently. You've been introduced to BASH. And you have already practiced using BASH syntax and tricks like tab complete, as well as pipes '|' and redirects '>' to manage command output. And finally, you know how to invoke a program by package name and provide initialization values for runtime to it through console.

That's awesome. You're doing great. But I want you to do even greater. I think you can do it, and I'll help if you get stuck.

Note: In the rest of the document, '!username' should be replaced with your actual account username. 

Step 1. Open terminal. Type 'cd \~/Documents/' and hit Return.
'cd' is 'change directory' and lets you move your console working path.
'~' is a path shortcut to user home directory. In this case, '/home/!username/'
It can be said that you are changing your console working directory path into the Documents folder that is located in your user home directory.


[Remember, the account you are interacting through needs read permissions to a directory to navigate into or see its contents. Since your account owns your /home/!username directory, you can both read and write to the contents with no problem, as well as execute scripts and programs that live there.

1a. Go back up one directory level using 'cd ..' (change directory to the directory above the current directory) and run 'ls -l' (list current directory contents, long list mode.) This will show you, among other things, what a permissions string looks like. Sometimes the account you're "borrowing" doesn't have proper permissions to do what you want to do.

In that case, sometimes, the output of the commands 'group !username' or 'id !username' (list group/id memberships of a user account,) combined with 'ls -l' (list contents in current directory, use long list output) will give you enough knowledge, and if you have the power, you can just add the account you're using to a valid group or vice versa. Other times, you will need to "borrow" a second, more privileged account to make that change. Don't forget to put things you "borrow" back how you found them once you're done :)

1b. For now, just run 'id !username' to see your membership. Then 'cd Documents' to go back into where you came from.

A fun thing about permissions - even if you don't have read to a directory, you can still view permissions for a directory you can see but can't access. After all, how else would your account be able to know that it's been told it can't go in, if it can't read groups and see permissions? ;) If you have (or "borrow") write permissions, 'chmod' (change mode) command will let you edit other permissions values.

1c. For extra credit, 'man chmod' to open the change mode command manual page, and tell me why 'chmod 777' is easy but sloppy.]


Step 2. From this location, the path of which can be printed using 'pwd' (present working directory,) use the command string 'mkdir scripts && cd scripts' (make directory named scripts - and right away, change the working path from the current location into the local directory called scripts.)

It's a good idea to double check where you think you are against where you actually are using 'pwd' (present working directory) before beginning some data operation.


Step 3. Did you 'pwd' to double check you were in /home/!username/Documents/scripts/ ? Good. Is that where you are? Even better. So now, 'touch autoNmap.sh' (create a file header in the present working directory of the file system called autoNmap.sh, and leave the content of the file blank.) 'touch' can also be useful to update the "last modified" timestamp without opening the file.

The file extension .sh is indicative of a shell script. In the next lesson, we are going to create a shell script to ask the user a few questions, autorun nmap based on the answers, automatically document the resulting output into a folder with the run date name and a file with the run time name, then display a little happy face to the user, but not in the file, before ending.


Step 4. Run 'more autoNmap.sh' to see the empty file contents.  'more' is very useful to print the contents of a file to console without opening an editor.  Try running 'more /etc/hosts' to see if your hosts file has any local hostname-to-IP mappings.  Because you just used an absolute path string to reference the file location, you didn't actually move the console's present working directory.  You told it to look somewhere else, but without going there first. An alternative using relative paths would be to 'cd /etc/ && more ./hosts' (change directory to /etc/, then 'more' the file called hosts looking in that directory.) './' indicates, "look at the path starting in the current working directory" - similar to how '../' indicates "look at the path starting in the directory above the current directory."


Step 5. Let's add text to the empty file we created and double check the content. Run 'cat >> ./autoNmap.sh sharky' (concatenation of text "sharky" into the file in the local present working directory named autoNmap.sh) once, then 'more autoNmap.sh' once again.


Good work!

And now in the future, I can just send you "run 
'cd ~/Documents && mkdir scripts && cd scripts && pwd' then 'touch autoNmap.sh && cat >> autoNmap.sh sharky && more autoNmap.sh'," 
or, 
tell you to "move into your home Docs folder, make a scripts dir and touch autoNmap.sh there, then concatenate sharky into the new file and output the file to console for verification." You know enough about both ways!


Let me know when you are ready to continue.

PS.  the Linux filesystem is case-sensitive.  'autoNmap.sh' 'autonmap.sh' and 'Autonmap.sh' can all exist in the same directory at one time, causing no problem for the computer but lots of issues for you if you don't think about it.  As they say - There may be a PEBKAC - Problem Exists Between Keyboard and Chair.

PPS.  /etc/hosts is a file with no file extension.  if you 'mkdir /etc/hosts' both a file named './hosts' will still exist, and the directory named './hosts/' will be created. Both can live in the same directory, in this case, '/etc/' and you might need to do 'sudo mkdir /etc/hosts' because you may not have naked write permissions.

Good luck, happy hunting!

