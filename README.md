<h1 align="center">ABXY</h1>
<h3 align="center">Forensics/Batch CTF</h3>

<p align="center">CTF Made for Code and Conquer '24</p>

<h3>$${\color{red}Overview:}$$</h3>
We are given a .bat file called “ABXY.bat”. We need get the answer in
hacker{XXXX}.


<h3>$${\color{red}Theory:}$$</h3>
.bat files work on language called batch, which is used for DOS application. It
can perform various functions such as copying, deleting, creating new files,
reading file data or writing to files. Rem command is used to comment out lines
in batch.

<h3>$${\color{red}Important:}$$</h3>
• The given .bat file is self-duplicating and self-destructing. Please use a
copy of the given file before continuing the challenge.
• The .bat file works only for windows/DOS based systems. Running .bat
files under Linux or Windows emulators such as WINE may not work as
intended.

<h3>$${\color{red}Solution:}$$</h3>

1. Run the .bat file in an isolated folder.
2. This creates multiple folders at the file location

![image](https://github.com/user-attachments/assets/99eb9116-8ee1-42e2-bb25-d4fb5046dbd4)

3. The .bat file self-destructs.
4. The file copies itself to \New Folder(6)\CR\22.

![image](https://github.com/user-attachments/assets/78d1afdd-5cab-4077-81af-5dc2fec15ed5)

5. Running the file repeats this again to \New Folder(6)\CR.

![image](https://github.com/user-attachments/assets/937bf3f5-eed8-406d-a883-aea1c2e02f21)

6. Running the file again displays the message “Not here. Try Again.”
7. The .bat file self-destructs.
8. Within the users Documents folder, a file called dblank.txt is created.

![image](https://github.com/user-attachments/assets/6873b96a-6e78-4b82-8f6a-63529848b92e)

9. The password is found within it.

![image](https://github.com/user-attachments/assets/3aed339b-e304-4602-ae40-c01fe597288a)

10. Opening the .bat file with a text editor reveals a lot of commented
code making the more time consuming to find the password within.
![image](https://github.com/user-attachments/assets/e7befdb9-d13c-41b9-85e1-07d24085407c)


<h3>$${\color{red}Flag:}$$</h3>
<h4>$${\color{lightgreen}hacker(21qw14aabfgh3refl4gbt3)}$$</h4>
