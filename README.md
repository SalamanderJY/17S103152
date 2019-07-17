# Peer2Peer_File_Deliver_System

Software System Design and Development Practice Repository.

1) Launch the Terminal and Navigate into the P2P_File_Sharing_System folder from the above zip.
2) Open Multiple-tabs and navigate into CentralIndxServer folder on the First tab, into the Peer_1 folder on the second tab, into the Peer_2 folder on the third tab and into the Peer_3 folder on the fourth tab.
3) Navigate into the First tab, where CentralIndxServer files are present.
4) On the Command prompt Run the build-script using the ant command.
$ ant
5) The Build-script is executed and it cleans and compiles the files of the CentralIndxServer present in the CentralIndxServer directory. After successful build, a message is displayed on the terminal:
Build Successful
Total Time: 1 second
6) Run the CentralIndxServer by the command:
$ java CentralIndxServer
A message is displayed saying the “<Central Index Server is Up and Running>”
This runs the CentralIndxServer and it starts listening to other Peers on the Port
7) Now, Navigate into the Second tab, where Peer_1 files are present.
8) Edit the file “indxip.txt” present inside Peer_1 folder using “vim” or “gedit”. Edit and Enter the IP Address of the Machine which is running the CentralIndxServer into this file. The IP Address of the Machine running CentralIndxServer can be obtained by running the “ifconfig” command on the CentralIndxServer Machine.
Example: If the IP Address of the CentralIndxServer Machine is: 10.0.0.16 or 127.0.0.1(for Localhost)
$vim indxip.txt
Inside the file-> Remove the existing IP Address and Enter:
10.0.0.16
Save the file and exit.
9) On the Command prompt Run the build-script using the ant command.
$ ant
10) The Build-script is executed and it cleans and compiles the files of the Peer_1 present in the Peer_1 directory. After successful build, a message is displayed on the terminal:
Build Successful
Total Time: 1 second
11) Run Peer_1 using the command:
$ java PeerServer
The Peer is run and a MENU is displayed on the screen with the following options for the Peer to select:
Enter The Option:
==================
1. Registering the File
2. Searching On CentralIndxServer
3. Downloading From Peer Server
4. Exit
