# Shell, I/O Redirections and filters

### I/O Redirections
This feature of the command line enables you to redirect the input and/or output of commands from and/or to files, or join multiple commands together using pipes to form what is known as a “command pipeline”


[**1. Standard Output**](http://linuxcommand.org/lc3_lts0070.php)

[**2. Standard Input**](http://linuxcommand.org/lc3_lts0070.php)

[**3. Pipelines**](https://www.geeksforgeeks.org/piping-in-unix-or-linux/)

[**4. Filters**](https://www.geeksforgeeks.org/filters-in-linux/)


## [Special characters](http://mywiki.wooledge.org/BashGuide/SpecialCharacters)
### Table of commands applied:

**Questions** | **Commands used**
--------- | -----------------------
[0-hello_world](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/0-hello_world)| `echo "Hello, World"` used to display text string
[1-confused_smiley](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/1-confused_smiley)| `echo "\"(Ôo)'"` command used to display confused smiley
 [2-hellofile](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/2-hellofile)| `cat /etc/passwd` used to display the content of /etc/passwd
[3-twofiles](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/3-twofiles)|`cat /etc/passwd /etc/hosts` used to display the contents of /etc/passwd & /etc/hosts
[4-lastlines](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/4-lastlines)|`tail -10 /etc/passwd` used to display 10 last lines of the file
[5-firstlines](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/5-firstlines)|`head -10  /etc/passwd` used to display 10 first lines of a file
[6-third_line](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/6-third_line)|`head -n 3 iacta | tail -n 1` script displays the third line of file iacta
[7-file](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/7-file)|`echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)` write a shell script that creates given file containing the text Best School starting with a new line
[8-cwd_state](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/8-cwd_state)|`ls -la > ls_cwd_content` used standard output 
[9-duplicate_last_line](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/9-duplicate_last_line)|`tail -n 1 iacta >> iacta` duplicates the last line
[10-no_more_js](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/10-no_more_js)|`find . -type f -name "*.js" -delete` used to delete the files .js
[11-directories](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/11-directories)|`find . -type d -not -name '.' | wc -l` commands used to count the nr of dir and subdir 
[12-newest_files](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/12-newest_files)|`ls -t | head` used to display 10 newest files
[13-unique](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/13-unique)|`sort | uniq -u` commands used to display a script that takes a list of words as input and prints only words that appear exactly once.
[14-findthatword](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/14-findthatword)|`grep -i "root" /etc/passwd` used to display lines containing the pattern “root” from the file /etc/passwd
[15-countthatword]
(https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/15-countthatword)|`grep -c -i "bin" /etc/passwd` used to display the number of lines that contain the pattern “bin” in the file /etc/passwd
[16-whatsnext](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/16-whatsnext)|`grep -i "root" -A 3 /etc/passwd` commands used to display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd
[17-hidethisword](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/17-hidethisword)|`grep -i -v "bin" /etc/passwd` used to display all the lines in the file /etc/passwd that do not contain the pattern "bin"
[18-letteronly](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/18-letteronly)|`grep -i "^[a-z]" /etc/ssh/sshd_config`display all lines of the file /etc/ssh/sshd_config starting with a letter.include capital letters as well
[19-AZ](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/19-AZ)|`tr "A" "Z" | tr "c" "e"`replace all characters A and c from input to Z and e respectively.
[20-hiago](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/20-hiago)|`tr -d "cC"`create a script that removes all letters c and C from input
[21-reverse](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/21-reverse)|`rev` script that reverse its input
[22-users_and_homes](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/22-users_and_homes)|`cut -d ':' -f 1,6 /etc/passwd | sort` displays all users and their home directories, sorted by users
[23-empty_casks](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/23-empty_casks)|`find . -empty | rev | cut -d '/' -f 1 | rev` Write a command that finds all empty files and directories in the current directory and all sub-directories
[24-gifs](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/24-gifs)|`find . -type f -name "*.gif" | rev | cut -d'/' -f1 | cut -d'.' -f2,3 | rev | sort -Vf` script that lists all the files with a .gif extension in the current directory and all its sub-directories
[25-acrostic](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/25-acrostic)|`cut -c 1 | paste -s -d ''`script that decodes acrostics that use the first letter of each line
[26-the_biggest_fan](https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/26-the_biggest_fan)|`tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev` script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
