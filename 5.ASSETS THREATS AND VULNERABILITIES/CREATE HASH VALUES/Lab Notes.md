cat file1.txt
Displays the contents of the file1.txt file

cat file2.txt

Displays the contents of the file2.txt file

Output of the two files:

X5O!P%@AP[4\PZX54(P^)7CC)7}$EICAR-STANDARD-ANTIVIRUS-TEST-FILE!$H+H*

X5O!P%@AP[4\PZX54(P^)7CC)7}$EICAR-STANDARD-ANTIVIRUS-TEST-FILE!$H+H*

sha256sum file1.txt 

Generates a SHA-256 hash of the file1.txt file

sha256sum file2.txt

Generates a SHA-256 hash of the file2.txt file

Output:

131f95c51cc819465fa1797f6ccacf9d494aaaff46fa3eac73ae63ffbdfd8267

2558ba9a4cad1e69804ce03aa2a029526179a91a5e38cb723320e83af9ca017b 

Compare hashes
sha256sum file1.txt >> file1hash

Generates the hash of the file1.txt file, and sends the output to a new file called file1hash.

sha256sum file2.txt >> file2hash

Generates the hash of the file2.txt file, and sends the output to a new file called file2hash

cmp file1hash file2hash

Highlights the differences in the file1hash and file2hash files


