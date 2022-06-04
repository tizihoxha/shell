# Shell, loops, conditions and parsing
## Recources
1. [Loops sample](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_01.html)
2. [Variable assignment and arithmetic](https://tldp.org/LDP/abs/html/ops.html)
3. [Comparison operators](https://tldp.org/LDP/abs/html/comparison-ops.html)
4. [File test operators](https://tldp.org/LDP/abs/html/fto.html)
5. [Make your scripts portable](https://www.cyberciti.biz/tips/finding-bash-perl-python-portably-using-env.html)

### Useful commands
#### Use man or help 
- env
- cut
- for
- while
- until
- if


| Scripts | Functions |
| --- | --- |
|[0-RSA_public_key.pub](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/0-RSA_public_key.pub) |  Public key|
|[1-for_best_school](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/1-for_best_school) | Displaying "Best School" 10 times|
|[2-while_best_school](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/2-while_best_school) | Displaying "Best School" 10 times|
|[3-until_best_school](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/3-until_best_school) | Displaying "Best School" 10 times|
|[4-if_9_say_hi](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/4-if_9_say_hi) | Displaying "Best School" 10 times, but for the 9th iteration, displays Best School and then Hi on a new line|
|[5-4_bad_luck_8_is_your_chance](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/5-4_bad_luck_8_is_your_chance) | Displaying "bad luck" for the 4th loop, "good luck" for the 8th loop and "Best School" for any other loop|
|[6-superstitious_numbers](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/6-superstitious_numbers) | Displays "bad luck from china" in the 4th loop, "bad luck from japan" in the 9th loop, "bad luck from italy" in the 17th loop, and numbers for any other loop until the number 20|
|[7-clock](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/7-clock) | Displays hours from 0 to 12 and minutes from 1 to 59|
|[8-for_ls](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/8-for_ls) | Displays the content of the current directory in a list format where only the names after the dash are displayed|
|[9-to_file_or_not_to_file](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/9-to_file_or_not_to_file) | Script that gives you information about the school file, and if it exists which type of file it is| 
|[10-fizzbuzz](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/10-fizzbuzz) | Displays numbers 1-100. Replaces any number with FizzBuzz for which are a multiple of both 3 and 5, Fizz for multiples of 3 and Buzz for multiples of 5. Any other numbers displayed as is|
|[11-read_and_cut](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/11-read_and_cut) | Displays the content of the file /etc/passwd but only the username, user id and home directory path for the user|
|[12-tell_the_story_of_passwd](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/12-tell_the_story_of_passwd) | Displays each line of the /etc/passwd file as a message, with some words being variable strings taken from the 1-7th fields of each line from the mentioned file|
|[13-lets_parse_apache_logs](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/13-lets_parse_apache_logs) | Displays the parsed Apache logs to show only the IP and HTTP_code using the mawk command|
|[14-dig_the-data](https://github.com/tizihoxha/shell/blob/main/loops_conditions_and_parsing/14-dig_the-data) | Displays the parsed Apache logs to show IP and HTTP_code using the mawk command in the desending order sorted by occurence|

