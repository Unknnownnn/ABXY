<h1 align="center">ABXY</h1>
<h3 align="center">Forensics/Batch CTF</h3>

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
1) Run the .bat file in an isolated folder.
2) This creates multiple folders at the file location
3) The .bat file self-destructs.
4) The file copies itself to \New Folder(6)\CR\22.
5) Running the file repeats this again to \New Folder(6)\CR.
6) Running the file again displays the message “Not here. Try Again.”
7) The .bat file self-destructs.
8) Within the users Documents folder, a file called dblank.txt is created.
9) The password is found within it.
10) Opening the .bat file with a text editor reveals a lot of commented
code making the more time consuming to find the password within.
