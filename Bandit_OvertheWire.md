## Bandit Over The Wire - [LINUX BASICS]


## Level - 0

1. Logged in to the Bandit0 server using the command 'ssh bandit0@bandit.labs.overthewire.org -p 2220' using the password 'bandit0' given in the website.
 
## Level 0 -> 1

1. Logged in to the Bandit0 server using the command 'ssh bandit0@bandit.labs.overthewire.org -p 2220' using the password 'bandit0' given in the website.

2. It was given that the password for the next levelwas stored in a readme file.

3. Searched for the readme file using 'ls' command.

4. Opened the readme file using the command 'cat readme'.

5. The password 'NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL' was displayed.

## Level 1 -> 2
1. Logged in to the Bandit1 server using the command 'ssh bandit1@bandit.labs.overthewire.org -p 2220' using the password 'NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL' given in the previous level.

2. It w given that the password for the next level is stored in a file called - located in the home directory.

3. Searched for the - file using 'ls' command.

4. Opened the - file using the command 'cat ./-'.

5. The password 'rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi' was displayed.
   
## Level 2 -> 3

1. Logged in to the Bandit2 server using the command 'ssh bandit2@bandit.labs.overthewire.org -p 2220' using the password 'rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi' given in the previous level.

2. It was given that the password for the next level is stored in a file called spaces in this filename located in the home directory.

3. Searched for file called 'spaces in this filename' using 'ls' command.

4. Opened the file using the command "cat 'spaces in this filename'".

5. The password 'aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG' was displayed.
   

## Level 3 -> 4

1. Logged in to the Bandit3 server using the command 'ssh bandit3@bandit.labs.overthewire.org -p 2220' using the password 'aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG' given in the previous level.

2. It was given that the password for the next level is stored in a hidden file in the inhere directory.

3. Opened the inhere directory by using the command 'cd inhere'.

4. Searched for hiiden files by using the command 'ls -a'.

5. Opened the hiiden file by using the command 'cat .hidden'.

6. The password '2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe' was displayed.

## Level 4 -> 5

1. Logged in to the Bandit4 server using the command 'ssh bandit4@bandit.labs.overthewire.org -p 2220' using the password '2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe' given in the previous level.

2. It was given that the password for the next level is stored in the only human-readable file in the inhere directory.

3. Opened the inhere directory by using the command 'cd inhere'.

4. Searched for human readable files by using the command 'ls -la'.

5. Opened the file './-file07' which contained ASCII text by using 'cat ./-file07'.

6. The password 'lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR' was displayed.
   
## Level 5 -> 6

1. Logged in to the Bandit5 server using the command 'ssh bandit5@bandit.labs.overthewire.org -p 2220' using the password 'lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR' given in the previous level.

2. It was given that the password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
    human-readable
    1033 bytes in size
    not executable
3. Opened the inhere directory by using the command 'cd inhere'.

4. Searched for the file with gven specifications using the command 'find . -type f -size 1033c ! -executable -exec file '{}' \; | grep ASCII'.

5. Opened the file using the command 'cat ./maybehere07/.file2'.

6. The password 'P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU' was displayed.

## Level 6 -> 7

1. Logged in to the Bandit6 server using the command 'ssh bandit6@bandit.labs.overthewire.org -p 2220' using the password 'P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU' given in the previous level.

2. It was given that the password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size
 
 3. Searched for tbhe file with the given specification usng the command 'find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null'.

 4. Opened the file using the command 'cat /var/lib/dpkg/info/bandit7.password'.

 5. The password 'z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S' was displayed.

## Level 7 -> 8

1. Logged in to the Bandit7 server using the command 'ssh bandit7@bandit.labs.overthewire.org -p 2220' using the password 'z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S' given in the previous level.

2. It was given that the password for the next level is stored in the file data.txt next to the word millionth.

3. The line with the word 'millionth' was taken by the command 'cat data.txt | grep millionth'.

4. The password 'TESKZC0XvTetK0S9xNwm25STk5iWrBvP' was displayed.

## Level 8 -> 9

1. Logged in to the Bandit8 server using the command 'ssh bandit8@bandit.labs.overthewire.org -p 2220' using the password 'TESKZC0XvTetK0S9xNwm25STk5iWrBvP' given in the previous level.

2. It was given that the password for the next level is stored in the file data.txt and is the only line of text that occurs only once.

3. Searched for the only line of text that occurs only once by using the command 'sort data.txt | uniq -u'.

4. The password 'EN632PlfYiZbn3PhVK3XOGSlNInNE00t' was displayed.

## Level 9 -> 10

1. Logged in to the Bandit9 server using the command 'ssh bandit9@bandit.labs.overthewire.org -p 2220' using the password 'EN632PlfYiZbn3PhVK3XOGSlNInNE00t' given in the previous level.

2. It was given that the password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

3. Searched for the line with preceded by several ‘=’ characters by using the command 'strings data.txt | grep ==='.

4. The password 'G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s' was displayed.

## Level 10 -> 11

1. Logged in to the Bandit10 server using the command 'ssh bandit10@bandit.labs.overthewire.org -p 2220' using the password 'G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s' given in the previous level.

2. It was given that the password for the next level is stored in the file data.txt, which contains base64 encoded data.

3. Opened the data.txt by using the command 'base64 -d data.txt'.

4. The password '6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM' was displayed.

## Level 11 -> 12

1. Logged in to the Bandit11 server using the command 'ssh bandit11@bandit.labs.overthewire.org -p 2220' using the password '6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM' given in the previous level.

2. It was given that the password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.

3. Opened the data.txt file by using the command 'cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m''.

4. The pass word 'JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv' was displayed.

## Level 12 -> 13

1. Logged in to the Bandit12 server using the command 'ssh bandit12@bandit.labs.overthewire.org -p 2220' using the password 'JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv' given in the previous level.

2. Made a temp folder and made a copy of the data.txt and renamed to hexdump_data

3. Reverted the hexdump and get the actual data by using the command 'xxd -r hexdump_data compressed_data'.

4. Tried to fnd the type of decompression by looking at the first bytes in the hexdump to find the file signature.

5. Added the correct file ending, by renaming the file and decompress the file with gzip -d.

6. The data was still not fully decompressed so checked the the first bytes again.

7. Renamed the file with the appropriate file ending (.bz2) and decompressed it with bzip2 -d.

8. The file was still compressed. xxd shows that it is ‘gzip’ compressed again. So repeated the previous steps, renaming and decompressing.

9. Used the command 'xxd compressed_data | head ', it displayed ‘data5.bin’ string, which is a filename.

10. Used 'mv compressed_data compressed_data.tar' and 'tar -xf compressed_data.tar ' to extract the file.

11. ‘data5.bin’ seems to be another archive with a file called ‘data6.bin’. So extracted the file again using the command 'tar -xf data5.bin'.

12. The file ‘data6.bin’ seems to be bzip2 compressed again.710

13. ‘data6.bin.out’ shows another file name ‘data8.bin’ again. So extracted this file.

14. Finally, done one more decompression with gzip and gotten a readable file with the password.

15. The password 'wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw' was displayed.
    
## Level 13 -> 14

1. Logged in to the Bandit13 server using the command 'ssh bandit13@bandit.labs.overthewire.org -p 2220' using the password 'wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw' given in the previous level.

2. it was given that the password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on.

3. Logged into the Bandit14 server from Bandit13 server the command 'ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220'.

4. Displayed the content of the /etc/bandit_pass/bandit14 using the command 'cat /etc/bandit_pass/bandit14'.

5. The password 'fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq' was displayed.
 
## Level 14 -> 15

1. Logged in to the Bandit14 server using the command 'ssh bandit14@bandit.labs.overthewire.org -p 2220' using the password 'fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq' given in the previous level.

2. It was given that the password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

3. Runned the command 'nc localhost 30000' and submitted the current level password.

4. The password 'jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt' was displayed.
   
## Level 15 -> 16

1. Logged in to the Bandit15 server using the command 'ssh bandit15@bandit.labs.overthewire.org -p 2220' using the password 'jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt' given in the previous level.

2. It was given that the password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

3. Runned the command 'openssl s_client -connect localhost:30001' and entered the current level password.

4. The password 'JQttfApK4SeyHwDlI9SXGR50qclOAil1' was displayed.

## Level 16 -> 17

1. Logged in to the Bandit16 server using the command 'ssh bandit16@bandit.labs.overthewire.org -p 2220' using the password 'JQttfApK4SeyHwDlI9SXGR50qclOAil1' given in the previous level.

2. It was given that the credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

3. Checked the services provided by each por tusing the command 'nmap -sV localhost -p 31000-32000'.

4. Out of the 5 ports displayed port 31790 looked promissing.

5. So runned the command 'openssl s_client -connect localhost:31790' and entered the current level password.

6. It a displayed a private SSH key which was save dt a temp file and used to login to Bandit17 server using the command 'ssh -i sshkey17.private bandit17@bandit.labs.overthewire.org -p 2220'.

7. Displayed the content of the /etc/bandit_pass/bandit17 using the command 'cat /etc/bandit_pass/bandit17'.

8. The password 'VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e' was displayed.

## Level 17 -> 18

1. Logged in to the Bandit17 server using the command 'ssh bandit17@bandit.labs.overthewire.org -p 2220' using the password 'VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e' given in the previous level.

2. It was given that there are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new.

3. Used 'diff passwords.old passwords.new' command to find the difference between the files.

4. The password 'hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg' was displayed.

## Level 18 -> 19

1. Logged in to the Bandit18 server using the command 'ssh bandit18@bandit.labs.overthewire.org -p 2220' using the password 'hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg' given in the previous level.

2. But simultaneously it was logged out.

3. It was given that  if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19 and the password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

4. So runned the command 'ssh bandit18@bandit.labs.overthewire.org -p 2220 ls' to find the files in the server.

5. Runned the command 'ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme' to display the content of the file.

6. The password 'awhqfNnAbc1naukrpqDYcF95h7HoMTrC' was displayed.
   
## Level 19 -> 20

1. Logged in to the Bandit19 server using the command 'ssh bandit19@bandit.labs.overthewire.org -p 2220' using the password 'awhqfNnAbc1naukrpqDYcF95h7HoMTrC' given in the previous level.

2. It was given that to gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

3. Checked who was the owner of the setuid binary by using the command 'ls -la'.

4. After executing the binary file using the command '/bandit20-do cat /etc/bandit_pass/bandit20' the password was displayed.

5. The password 'VxCazJaVykI6W36BkBU0mJTCM8rR95XT' was displayed.

## Level 20 -> 21

1. Logged in to the Bandit20 server using the command 'ssh bandit20@bandit.labs.overthewire.org -p 2220' using the password 'VxCazJaVykI6W36BkBU0mJTCM8rR95XT' given in the previous level.

2. It was given that there is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

3. Create a connection in server mode by using the command 'echo -n 'VxCazJaVykI6W36BkBU0mJTCM8rR95XT' | nc -l -p 1234 &
[1] 24661'.

4. Executed the command './suconnect 1234'

5. The password 'NvEJF7oVjkddltPSrdKEFOllh9V1IBcq' was displayed.
   
## Level 21 -> 22

1. Logged in to the Bandit21 server using the command 'ssh bandit21@bandit.labs.overthewire.org -p 2220' using the password 'NvEJF7oVjkddltPSrdKEFOllh9V1IBcq' given in the previous level.

2. It was given that a program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

3. Looked at what was in the ‘/etc/cron.d’ folder by using the command 'ls -la /etc/cron.d'.

4. Opened the /etc/cron.d/cronjob_bandit22 file using the command 'cat /etc/cron.d/cronjob_bandit22'.

5. Opened the /usr/bin/cronjob_bandit22.sh file using the command 'cat /usr/bin/cronjob_bandit22.sh'.

6. Opened the /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv file using the command 'cat  /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv'.

7. The password 'WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff' was displayed.

## Level 22 -> 23

1. Logged in to the Bandit22 server using the command 'ssh bandit23@bandit.labs.overthewire.org -p 2220' using the password 'WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff' given in the previous level.

2. It was given that a program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

3. Looked at what was in the ‘/etc/cron.d’ folder by using the command 'ls -la /etc/cron.d'.

4. Opened the /etc/cron.d/cronjob_bandit23 file using the command 'cat /etc/cron.d/cronjob_bandit23'.

5. Opened the /usr/bin/cronjob_bandit23.sh file using the command 'cat /usr/bin/cronjob_bandit23.sh'.

6. Runned the command 'echo I am user bandit23 | md5sum | cut -d ' ' -f 1' and the name of the tmp file was displayed

7. Opened the tmp file using the command 'cat /tmp/8ca319486bfbbc3663ea0fbe81326349'.

8. The password 'QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G' was displayed.
   
## Level 23 -> 24

1. Logged in to the Bandit23 server using the command 'ssh bandit123@bandit.labs.overthewire.org -p 2220' using the password 'QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G' given in the previous level.

2. It was given that a program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

3. Looked at what was in the ‘/etc/cron.d’ folder by using the command 'ls -la /etc/cron.d'.

4. Opened the /etc/cron.d/cronjob_bandit24 file using the command 'cat /etc/cron.d/cronjob_bandit24'.

5. Opened the /usr/bin/cronjob_bandit24.sh file using the command 'cat /usr/bin/cronjob_bandit24.sh'.

6. Made a tmp file using the command 'mkdir /tmp/rand'.

7. Created a shell script file using the command 'nano bandit24_pass.sh'.

8. Written the Shell Script file with content:
   '#!/bin/bash
    cat /etc/bandit_pass/bandit24 > /tmp/rand/password'

9. Given the necessary permissions to the Shell file.
   
10. Created a file using the command 'touch password'.

11. Given the permissions for the password file.

12. Executed the Shell file using the command 'cp bandit24_pass.sh /var/spool/bandit24/foo/bandit24_pass.sh'.

13. Displayed the content of the password file using the command 'cat password'.

14. The password 'VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar' was displayed.
    
## Level 24 -> 25

1. Logged in to the Bandit24 server using the command 'ssh bandit124@bandit.labs.overthewire.org -p 2220' using the password 'VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar' given in the previous level.

2. It was given that a daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

3. Made a tmp file and wrote a script file for getting all possible valuez (0000-9999)

4. The password along with the poassible values was stored in the pass.txt file.

5. By the command 'cat pass.txt | nc localhost 30006', the correct pincode was enterd.

6. The password 'p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d' was displayed.
   
## Level 25 -> 26

1. Logged in to the Bandit25 server using the command 'ssh bandit125@bandit.labs.overthewire.org -p 2220' using the password 'p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d' given in the previous level.

2. It was given that logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

3. Used the command 'ls' to find what files was there.

4. Tried to log in to Bandit26 using the command 'ssh -i bandit26.sshkey bandit26@localhost -p 2220'

5. But it was simulatneously logged out.
y using the comman
6. A hint was given in the /usr/bin/showtext about more ~/text.txt.

7. So entered the command 'ssh -i bandit26.sshkey bandit26@localhost -p 2220' and reduced the size of the terminal tab to activate the more program.

8. Entered 'V' to start up an editor in the current line.

9. Tried to execute the shell by using the command ':shell'

10. Nothing happened.So changed the shell to /bin/bash by using the command ':set shell=/bin/bash'.

11. Executed the shell again by the command ':shell'

12. Now it was logged in to the Bandit26 sever.

13. Used the command 'cat /etc/bandit_pass/bandit26' to get the password.
   
14. The password 'c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1' was displayed.
    
## Level 26 -> 27

1. Logged in to the Bandit26 server using the command 'ssh bandit126@bandit.labs.overthewire.org -p 2220' using the password 'c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1' given in the previous level.

2. It was given that 'Good job getting a shell! Now hurry and grab the password for bandit27!'

3. Used 'ls' command to find out what all files was there in the server.

4. Used the command './bandit27-do cat /etc/bandit\_pass/bandit27' to get the password.

5. The password 'YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS' was displayed.
   
## Level 27 -> 28

1. Logged in to the Bandit27 server using the command 'ssh bandit127@bandit.labs.overthewire.org -p 2220' using the password 'YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS' given in the previous level.

2. It was given that there is a git repository at ssh://bandit27-git@localhost/home/bandit27-git/repo via the port 2220. The password for the user bandit27-git is the same as for the user bandit27.Clone the repository and find the password for the next level.

3. Clonned the Git repo by the command 'git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo'.

4. Opened the repo directory by the command 'cd repo'.

5. Use 'ls' to find the  files in the repo directory.

6. Displayed the content of the README file by using the command 'cat README'

7. The password 'AVanL161y9rsbcJIsFHuw35rjaOM19nR' was displayed.
   

## Level 28 -> 29

1. Logged in to the Bandit28 server using the command 'ssh bandit128@bandit.labs.overthewire.org -p 2220' using the password 'AVanL161y9rsbcJIsFHuw35rjaOM19nR' given in the previous level.

2. It was given that There is a git repository at ssh://bandit28-git@localhost/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28.Clone the repository and find the password for the next level.

3. Clonned the Git repo by the command 'git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo'.

4. Opened the repo directory by the command 'cd repo'.

5. Use 'ls' to find the  files in the repo directory.

6. Displayed the content of the README file by using the command 'cat README'.

7. But the password was encrypted.

8. Used the command 'git log'.

9. Used the command 'git checkout c0a8c3cf093fba65f4ee0e1fe2a530b799508c78' to decrypt the README.md .

10. Displayed the content of the README file by using the command 'cat README'.

11. It was still encrypted.

12. Used the command 'git checkout abcff758fa6343a0d002a1c0add1ad8c71b88534' to decrypt the README.md .

13. Displayed the content of the README file by using the command 'cat README'.

14. The password 'tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S' was displayed.

## Level 29 -> 30

1. Logged in to the Bandit29 server using the command 'ssh bandit129@bandit.labs.overthewire.org -p 2220' using the password 'tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S' given in the previous level.

2. It was given that there is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29. Clone the repository and find the password for the next level.

3. Clonned the Git repo by the command 'git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo'.

4. Opened the repo directory by the command 'cd repo'.

5. Use 'ls' to find the  files in the repo directory.

6. Displayed the content of the README file by using the command 'cat README'.

7. But the password was encrypted.

8. Used the command 'git log'.

9. Used the command 'git checkout 1a57cf10158f133c4f40ff82251f605a7618631d' to decrypt the README.md .

10. Used the command 'git branch' th find the branch.

11. Used the command 'git branch -a' to find whart all branches are there.

12. Used the command 'git checkout dev' to change the branch to 'dev'.

13. Displayed the content of the README file by using the command 'cat README'.

14. The password 'xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS' was displayed.
