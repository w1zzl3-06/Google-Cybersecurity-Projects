As a security analyst, it’s key that you know how to navigate, manage, and analyze files remotely via a Linux shell without a graphical user interface.

pwd

Displays current directory.

ls

Displays the names of the files and directories in the current working directory.

cd reports

Navigates to the reports directory i.e /home/analyst/reports

Note: The cd command accepts absolute and relative paths. An absolute path includes all the directories from the root of the file system and starts with a /. An alternative is a relative path, which is expressed starting from the current directory and starts without the initial /. The above command uses a relative path.

cd /home/analyst/reports

The command to complete this step using an absolute path

cat Q1_added_users.txt

Display the contents of the Q1_added_users.txt file

Note: The cat command prints the contents of a file to the shell. You can specify the file to display using absolute or relative paths.

head server_logs.txt

Displays the first 10 lines of the server_logs.txt file

Note: The head command displays just the beginning of a file, by default ten lines. You can specify how many lines to display using the -n argument, which specifies the number of lines to display.

tail

Displays the last 10 lines of a file


