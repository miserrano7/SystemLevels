There are two commands to use when changing the permissions on your files, those being the chown and chgrp commands. chgrp allows you to change the group of a directory, for example in this assignment we were only supposed to allow permissions for the professor and TA to our folder. If we wanted to do that we could use the command groups followed by their username to check which groups both the professor and TA are part of. Once we find out what group they're part of we can use the command chgrp GROUPNAME Submissions(my folder name), which will change the group to GROUPNAME. Then for group I can change the permissions using the command chmod 750 Submissions. This will give the owner rwx permissions, the group r-x permissions and others will have no permissions (---). If we want to do use the chown command, by using the command chown GROUP Submissions, we're adding the group made up of the TA and professor to be owners of the folder. This will give ownership to them but the folder will still belong to me since i'm the original owner of the folder.
To complete the hunger games portion of this assignment I first accessed the directory of the professor by typing the command âcd /home/cumoja1/3320â once in the directory I used the ls command to view what files were in the directory. The used the cd command to return to my directory, so that I could copy the file into my own directory. I used the following command to do this: cp /home/cumoja1/3320/The*Hunger*Games.txt  /home/mserrano2/My\ Hunger\ Games
What this did was access the hunger games files in the directory of the professor, I included * in-between each word so that it could be read properly. This file was copied into my directory, and at the same time I changed the files name to My Hunger Games by using the \ escape character to hold spaces between each word. I used ls and cat commands to make sure it was actually copied in my directory, with the contents of the file. Once I had the file copied into my directory I used the command vi My\ Hunger\ Games to edit the file. I used esc then the command :%s/Katniss/Michelle/g to replace all instances of Katniss with Michelle. Then I used esc followed by /Michelle to find instances of my name, followed by n to make sure Katniss had been replaced with my own name. Then I moved My Hunger Games file to my Submissions directory by using the following command: my My\ Hunger\ Games /home/mserrano2/Submissions and cd to Submissions then used ls to make sure the file was there.