As a security analyst, it’s key to know how to find the information you need. The ability to search for specific strings can help you locate what you need more efficiently

grep error server_logs.txt

This will filter server_logs.txt file, and return a list of the lines that match the text string error.

Note: The first argument passed to grep is the string you're searching for, and the second argument is the name of the file you're searching through.

ls | grep Q1

Using the pipe character (|), pipe the output of the ls command to the grep command to list only the files containing the string Q1 in their names.

Note: Piping sends the standard output of one command to the standard input of another command for further processing. In the example, the output of the grep command is piped to the ls command and the output displayed in the shell.

grep jhill Q2_deleted_users.txt

Searches the Q2_deleted_users.txt file for the username jhill

grep "Human Resources" Q4_added_users.txt

Search the Q4_added_users.txt file to list the users who were added to the Human Resources department.



