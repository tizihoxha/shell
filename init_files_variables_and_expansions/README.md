# Shell, init files, variables and expansions

### Expansion
Each time we type a command line and press the enter key, bash performs several processes upon the text before it carries out our command.

### *Different types of expansions*

[**1. brace expansion**](https://www.gnu.org/software/bash/manual/html_node/Brace-Expansion.html)

[**2. tilde expansion**](https://www.gnu.org/software/bash/manual/html_node/Tilde-Expansion.html)

[**3. parameter and variable expansion**](https://www.gnu.org/software/bash/manual/html_node/Shell-Parameter-Expansion.html)

[**4. command substitution**](https://www.gnu.org/software/bash/manual/html_node/Command-Substitution.html)

[**5. arithmetic expansion**](https://www.gnu.org/software/bash/manual/html_node/Arithmetic-Expansion.html)

[**6. word splitting**](https://www.gnu.org/software/bash/manual/html_node/Word-Splitting.html)

[**7. filename expansion**](https://www.gnu.org/software/bash/manual/html_node/Filename-Expansion.html)

### Shell initialization files

A shell initialization file is a shell script that runs automatically each time the shell executes.

Shell init files are classified as below:

**System-wide configuration files**

1. /etc/profile
2. /etc/bashrc

**Individual user configuration files**
1. ~/.bash_profile
2. ~/.bash_login
3. ~/.profile
4. ~/.bashrc
5. ~/.bash_logout

### Variables
#### Types of variables

1. Global variables
2. Local variables

### Table of commands applied:

**Questions** | **Commands used**
--------- | -----------------------
[0-alias](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/0-alias)| `alias ls="rm *"` using an alias to attrribute `ls` `rm*` funcions
[1-hello_you](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/1-hello_you)| `echo "hello $USER"` command used to display script
 [2-path](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/2-path)| `PATH=$PATH:/action` Adding action to the path
[3-paths](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/3-paths)|`echo $PATH | tr ':' '\n' | wc -l ` the command is used to count the number of dir in the path
[4-global_variables](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/4-global_variables)|`printenv` command used to display environment variables
[5-local_variables](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/5-local_variables)|`set` command used to display local variables
[6-create_local_variable](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/6-create_local_variable)|`BEST='School'` script used to create a local variable
[7-create_global_variable](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/7-create_global_variable)|`export BEST="School"` command used to create global variable
[8-true_knowledge](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/8-true_knowledge)|`echo $((128 + $TRUEKNOWLEDGE))` the commands are used to display arithmetic expansion 
[9-divide_and_rule](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/9-divide_and_rule)|`echo $((POWER/DIVIDE))` commands used to display arithmetic expansions
[10-love_exponent_breath](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/10-love_exponent_breath)|`echo $((BREATH**LOVE))` arithmetic expnsions
[11-binary_to_decimal](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/11-binary_to_decimal)|`echo $((2#$BINARY))` arithmetic expansion used to convert numbers from binary to decimal
[12-combinations](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/12-combinations)|`echo {a..z}{a..z} |tr ' ' '\n' | grep -v "oo"` command group used to Create a script that prints all possible combinations of two letters, except oo
[13-print_float](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/13-print_float)|`printf '%.2f\n' $NUM` script that prints a number with two decimal places, followed by a new line
[14-decimal_to_hexadecimal](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/14-decimal_to_hexadecimal)|`printf '%x\n' $DECIMAL` commands used to convert a script from decimal to hexadecimal
[15-rot13](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/15-rot13)|`tr 'n-za-mN-ZA-M' 'a-zA-Z'` commands used to decode from rot13
[16-odd](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/16-odd)|`paste - - | cut -f1` command used to print every other line from the input, starting with the first line
[17-water_and_stir](https://github.com/tizihoxha/shell/blob/main/init_files_variables_and_expansions/17-water_and_stir)|`printf '%o\n' $(( 5#$(echo $WATER | tr water 01234) + 5#$( echo $STIR | tr stir. 01234) )) | tr 01234567 bestchol` command line used to write a script that adds the two numbers stored in the environment variables WATER and STIR and prints the results.
