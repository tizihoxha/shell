# [Shell, processes and signals](https://www.bogotobogo.com/Linux/linux_process_and_signals.php)

***Information***

- [Linux PID](http://www.linfo.org/pid.html)
- [Linux process](https://www.thegeekstuff.com/2012/03/linux-processes-environment/)
- [Linux signal](https://www.thegeekstuff.com/2012/03/linux-signals-fundamentals/)

***Important commands***
- ps
- pgrep
- pkill
- kill
- exit
- trap


| Scripts | |
| --- | --- |
|[0-what-is-my-pid](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/0-what-is-my-pid) | Displays its own PID.|
|[1-list_your_processes](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/1-list_your_processes) | Displays a list of all currently running processes, including those which may not have TTY, in a hierarchy order.|
|[2-show_your_bash_pid](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/2-show_your_bash_pid) | Adds to the previous and displays lines containing the bash word.|
|[3-show_your_bash_pid_made_easy](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/3-show_your_bash_pid_made_easy) | Displays only the PID of the processes containing 'bash'|
|[4-to_infinity_and_beyond](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/4-to_infinity_and_beyond) | Print a message indefinitely every 2 seconds.|
|[5-dont_stop_me_now](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/5-dont_stop_me_now) | Script that kills previous process.|
|[6-stop_me_if_you_can](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/6-stop_me_if_you_can) | Script that stops process using pkill command.|
|[7-highlander](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/7-highlander) | Script that prints 'To infinity and beyond' indefinitely with a sleep 2 and prints 'I am invincible!!!' when it terminates.|
|[8-beheaded_process](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/8-beheaded_process) | Script that deletes highlander.|
|[10-process_and_pid_file](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/10-process_and_pid_file) | Creates the file /var/run/myscript.pid containing its PID, displays a message indefinitely, and does several other thing based on the signal.|
|[11-manage_my_process](https://github.com/tizihoxha/shell/blob/main/processes_and_signals/11-manage_my_process) | Script that manages bg process manage_my_process. Either starting, stopping or restarting the other process and creating a file storing its PID.|
