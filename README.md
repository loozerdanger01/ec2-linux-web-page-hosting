# ec2-linux-web-page-hosting
after cretating EC2 linux server
=============================================
login the server in putty.
 -->host name --> public ip
 -->change the apperance and other colour setting as you wish.
 -->connections --> go to SSH --> auth --> credentials --> browse the .ppk key file
 -->then login as : ec2-user (user name)
==============================================
To copy the webpage templates
==============================================
-->WinSCP login
===================
   --> download WinSCP (download link : https://winscp.net/download/WinSCP-6.1.2-Setup.exe )
   --> install the WinSCP and launch
   --> select protocol --> SFTD
   --> host name --> public ip
   --> user name --> ec2-user
   --> password --> advanced --> SSH --> authentication --> browse the .ppk key file
   --> then login
===============================
-->WinSCP copy file
===================
   --> on left  :linux system --> go to the root directory path in linux (/var/www/html/)
   --> on right : your system --> go to the path you have the webpage template file 
   --> if you copy the file there will be a erro --> erro code : 3
   --> go to putty linux machine 
        -->to give permission read,write,remove file
        --> chmode 777 < directory name >   --> example : chmode 777 /var/www/html/
        --> now its ready to copy file
   --> now copy the file to the path
   --> serch the public ip in your browser 
   --> hosting complete***
