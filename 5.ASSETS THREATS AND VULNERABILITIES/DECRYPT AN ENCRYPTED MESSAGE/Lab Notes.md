Read the contents of a file:

ls /home/analyst

Lists the files in the current working directory, Two files, Q1.encrypted and README.txt, and a subdirectory, caesar are found.

cat README.txt

cat command to list the contents of the README.txt file

This will display the following output:

Hello,
All of your data has been encrypted. To recover your data, you will need to solve a cipher. To get started look for a hidden file in the caesar subdirectory.

Find a hidden file:
cd caesar
The cd command is used to change to the caesar subdirectory of the home directory.

ls -a

List all files, including hidden files, in your home directory.

cat .leftShift3

Lists the contents of the .leftShift3 file

cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z"

Decrypts the Caesar cipher in the .leftshift3 file

This will display the following output:

In order to recover your files you will need to enter the following command:

openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute

openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute

Decrypts the Q1.encrypted file

cat Q1.recovered

Lists the contents of the Q1.recovered file

This will display the following output:

If you are able to read this, then you have successfully decrypted the classic cipher text. You recovered the encryption key that was used to encrypt this file. Great work!

