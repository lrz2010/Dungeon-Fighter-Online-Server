Instructions for use:

Use CentOS 5 - 7  64-bit system

1G1H server recommended 5  or 7 
Download flie

installEN

Put the server root directory

putty run command:
cd /;chmod -R 0777 /installEN;bash installEN

The default database account is: game

The default password is:uu5!^%jg


php directory: /opt/lampp/htdocs  

Port:1234

Database directory: /opt/lampp/var/mysql

Download grade patch. 
Renamed df_game_r_60or70or80or90 to df_game_r
Download link:http://lrz2011.f3322.net:8181/gradepatch.7z

Upload Script.pvf, publickey.pem, grade patch.

Upload to folder: root/home/neople/game

Run the command after the upload is complete:
cd /root
./run


Routine maintenance orders:
cd /root;./stop;./stop

./run

Rerun the command:
cd /root;./stop;./stop;./run

-------------------------------------------------------

Database Backup

Packaging command:
tar -zcvf /root/backup.tar.gz /opt/lampp/var/mysql
Packaged files are in the root folder


After setting up the server
Upload the packaged file to the <root> root directory

Restore command:
cd /;rm -rf /opt/lampp/var/mysql;tar -zxvf backup.tar.gz.tar.gz -C /;reboot
After entering the command, the server will restart
