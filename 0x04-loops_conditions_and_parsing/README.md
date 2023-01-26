✅ 0. Create a SSH RSA key pair
Read for this task:

Linux and Mac OS users
Windows users
man: ssh-keygen

You will soon have to manage your own servers hosted on remote data centers. We need to set them up with your RSA public key so that you can access them via SSH.

Create a RSA key pair.

Requirements:

Share your public key in your answer file 0-RSA_public_key.pub
Fill the SSH public key field of your intranet profile with the public key you just generated
If you decide to add a passphrase to your key, make sure to save this passphrase in a secure location, you will not be able to use your keys without the passphrase
SSH and RSA keys will be covered in depth in a later project.

File(s): 0-RSA_public_key.pub

✅ 1. For Best School loop
Write a Bash script that displays Best School 10 times.

Requirement:

You must use the for loop (while and until are forbidden)
File(s): 1-for_best_school

✅ 2. While Best School loop
Write a Bash script that displays Best School 10 times.

Requirements:

You must use the while loop (for and until are forbidden)
File(s): 2-while_best_school

✅ 3. Until Best School loop
Write a Bash script that displays Best School 10 times.

Requirements:

You must use the until loop (for and while are forbidden)
File(s): 3-until_best_school

✅ 4. If 9, say Hi!
Write a Bash script that displays Best School 10 times, but for the 9th iteration, displays Best School and then Hi on a new line.

Requirements:

You must use the while loop (for and until are forbidden)
You must use the if statement
File(s): 4-if_9_say_hi

✅ 5. 4 bad luck, 8 is your chance
Write a Bash script that loops from 1 to 10 and:

displays bad luck for the 4th loop iteration
displays good luck for the 8th loop iteration
displays Best School for the other iterations
Requirements:

You must use the while loop (for and until are forbidden)
You must use the if, elif and else` statements
File(s): 5-4_bad_luck_8_is_your_chance

✅ 6. Superstitious numbers
Write a Bash script that displays numbers from 1 to 20 and:

displays 4 and then bad luck from China for the 4th loop iteration
displays 9 and then bad luck from Japan for the 9th loop iteration
displays 17 and then bad luck from Italy for the 17th loop iteration
Requirements:

You must use the while loop (for and until are forbidden)
You must use the case statement
File(s): 6-superstitious_numbers

✅ 7. Clock
Write a Bash script that displays the time for 12 hours and 59 minutes:

display hours from 0 to 12
display minutes from 1 to 59
Requirements:

You must use the while loop (for and until are forbidden)
File(s): 7-clock

✅ 8. For ls
Write a Bash script that displays:

The content of the current directory
In a list format
Where only the part of the name after the first dash is displayed (refer to the example)
Requirements:

You must use the for loop (while and until are forbidden)
Do not display hidden files
File(s): 8-for_ls

✅ 9. To file, or not to file
Write a Bash script that gives you information about the school file.

Requirements:

You must use if and else (case is forbidden)
Your Bash script should check if the file exists and print:
if the file exists: school file exists
if the file does not exist: school file does not exist
If the file exists, print:
if the file is empty: school file is empty
if the file is not empty: school file is not empty
if the file is a regular file: school is a regular file
if the file is not a regular file: (nothing)
File(s): 9-to_file_or_not_to_file

✅ 10. FizzBuzz
Write a Bash script that displays numbers from 1 to 100.

Requirements:

Displays FizzBuzz when the number is a multiple of 3 and 5
Displays Fizz when the number is multiple of 3
Displays Buzz when the number is a multiple of 5
Otherwise, displays the number
In a list format
File(s): 10-fizzbuzz

Advanced Tasks
✅ 11. Read and cut
help: read

Write a Bash script that displays the content of the file /etc/passwd.

Your script should only display:

username
user id
Home directory path for the user
Requirements:

You must use the while loop (for and until are forbidden)
File(s): 100-read_and_cut

✅ 12. Tell the story of passwd
Read:

IFS (internal field separator)
Understanding /etc/passwd
Write a Bash script that displays the content of the file /etc/passwd, using the while loop + IFS.

Format: The user USERNAME is part of the GROUP_ID gang, lives in HOME_DIRECTORY and rides COMMAND/SHELL. USER ID's place is protected by the passcode PASSWORD, more info about the user here: USER ID INFO

Requirements:

You must use the while loop (for and until are forbidden)
File(s): 101-tell_the_story_of_passwd

⬜ 13. Let's parse Apache logs
Apache is among the most popular web servers in the world, serving 50% of all active websites, no doubt that you will have to interact with it within your career.

As a Full-Stack Software Engineer, you have to master the art of parsing log files. This task involves a simple parsing of Apache log access files.

Today the Customer Support department reported that a user reported that the site is being “buggy”. Not being a detailed description, you want to have a look at the Apache logs and gather data about the traffic.

Write a Bash script that displays the visitor IP along with the HTTP status code from the Apache log file.

Requirement:

Format: IP HTTP_CODE
in a list format
See example
You must use awk
You are not allowed to use while, for, until and cut
Download and commit the apache-access.log file along with your answers files
Example log lines:

81.65.217.135 - - [07/Feb/2016:07:22:16 -0800] "GET /wp-content/uploads/2015/02/1620528_10152406520622652_278602715_n-300x300.jpg HTTP/1.1" 200 37378 "http://hnwatcher.com/silicon-valley/" "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.97 Safari/537.36"
81.65.217.135 - - [07/Feb/2016:07:22:16 -0800] "GET /wp-content/uploads/2015/03/1-l57K-8uyN9ELuGbgcaItmw-1024x524.png HTTP/1.1" 200 190496 "http://hnwatcher.com/silicon-valley/" "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.97 Safari/537.36"
178.137.93.235 - - [07/Feb/2016:07:27:24 -0800] "GET /steeve-morin-de-google-a-lentreprenariat/ HTTP/1.1" 200 29286 "http://jm-aj.com/" "Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; TheFreeDictionary.com; .NET CLR 1.1.4322; .NET CLR 1.0.3705; .NET CLR 2.0.50727)"
178.137.93.235 - - [07/Feb/2016:07:28:33 -0800] "GET /steeve-morin-de-google-a-lentreprenariat/ HTTP/1.1" 200 29452 "http://alborzan.com/" "Mozilla/4.0 (compatible; MSIE 6.0; America Online Browser 1.1; rev1.2; Windows NT 5.1; SV1; .NET CLR 1.1.4322)"
File(s): 102-lets_parse_apache_logs


