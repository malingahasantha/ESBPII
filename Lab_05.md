###IT12068838##
###W.V.H.Malinga##

----------


# Create Local YUM repository on CentOS 7 #
------------------------------------------

## 1.Create Source: ##
### 1.1 Mount the CD/DVD ROM on the any directory of your wish, for testing mount it on /cdrom. ###

* # mkdir /cdrom 
* # mount /dev/cdrom /cdrom

## 2.Configuration file: ##
### 2.1 Create the new repo file called cdrom.repo under /etc/repos.d directory. ##

* # vi /etc/yum.repos.d/local.repo

![1](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11796359_972786909433580_3787227264172542481_n.jpg?oh=e4da01ae5d3faa067a4a02b1197eda59&oe=564ADE4E)

### 2.2 Add the following details. ###

![2](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfa1/v/t1.0-9/11822308_972786919433579_7522304763833638445_n.jpg?oh=7d188a07a12b8c19116d3980237f133a&oe=5651DA61)

## 3.Installation: ##
### 3.1 Before installing clear the repository cache by issuing the following command. ###

![3](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11828783_972786949433576_3206604363380409048_n.jpg?oh=861d7dc3a949978cec114ce431f743ad&oe=565BE3FC)

### 3.2 Install the package using the yum command, let’s install the vsftpd package from the local repository. ###

![4](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfa1/v/t1.0-9/11813533_972786996100238_7157562868563993355_n.jpg?oh=05c4e1fb4a2b88ff1097c1f415e79124&oe=56383285)

![5](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xat1/v/t1.0-9/11143468_972787039433567_1322442666722115865_n.jpg?oh=2f113c806cde19bc5d95259cf34dd532&oe=56419034)

![6](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpa1/v/t1.0-9/11796271_972787202766884_7149415709095642346_n.jpg?oh=28a503520951daf20a4f4bfc521fb40a&oe=564F4395)

# Install OwnCloud 7 on CentOS 7 #
----------------------------------

## 1.Prerequisites: ##
### 1.1 it is based on PHP and database combination, database can be any of the above four. So install PHP, Apache web server and MySQL server on CentOS 7. ###

![a1](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xta1/v/t1.0-9/11144903_972787232766881_3793629089785570007_n.jpg?oh=be361608d54613b25f5d4599deac7bf4&oe=5655C19E)

![a2](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xaf1/v/t1.0-9/11813403_972787259433545_1490655195124097027_n.jpg?oh=a19abf6a18829bdc911dc1971fc07a36&oe=564E1D52)

### 1.2 Set SELinux to allow OwnCloud to write the data. ###

![a3](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xft1/v/t1.0-9/11800078_972787306100207_7250731718140946561_n.jpg?oh=efc8f56df2459f1fa56feb920d53ebb9&oe=5645FA60)

### 1.3 Allow apache in firewall. ###

![a4](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xft1/v/t1.0-9/11825881_972787319433539_5833916289851440137_n.jpg?oh=5acb0566c7302eefce7398733719f25a&oe=5650536B)

### 1.4 Start Apache and MariaDB. ###

![a5](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfa1/v/t1.0-9/11054280_972787332766871_4790966344752091218_n.jpg?oh=fe100919bb3083b1dcffbc80828ae8c9&oe=5653A3DB)

### 1.5 Auto start the service at system start-up. ###

![a6](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11836652_972787342766870_7391236364047913662_n.jpg?oh=49d7b849007c26b04f2767feb89a3a8e&oe=563BB772)

## 2.Download and Setup: ##
### 2.1 Download ownCloud from official website or enter the fallowing command on terminal. ###

* wget https://download.owncloud.org/community/owncloud-7.0.0.tar.bz2

### 2.2 Extract the archive. ###

![a7](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtp1/v/t1.0-9/11800508_972787396100198_1121634173984782988_n.jpg?oh=565bb3fe108aa2ea853ad739be112891&oe=563E6C3D)

![a8](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xft1/v/t1.0-9/11831748_972787439433527_6160962993680637829_n.jpg?oh=b05aece2aaa5b584032afd4abb55b2b6&oe=564E2C97)

### 2.3 Allow the web server to read and write the files on cloud directory. ###

![a9](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtp1/v/t1.0-9/11796439_972787446100193_7877211800433023807_n.jpg?oh=0a54c915b005f944ed1d9ab1a27a3165&oe=56561B22)

![a10](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xat1/v/t1.0-9/11265121_972787499433521_5496489501887613233_n.jpg?oh=b86d2e083d822ef25688982e9511ce29&oe=564614B8)

![a11](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpa1/v/t1.0-9/11800396_972787519433519_3259988085311233195_n.jpg?oh=088b7b9d5199a15ff1485672cf672ec9&oe=564A0426)

## 3.Create Database: ##
### 3.1 If you are setting up a MariaDB for the first time, here is the tutorial on Securing MariaDB.  MariaDB server must be started before creating the database, login to MySQL server. ###

![a12](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/11813295_972787542766850_2821491067885580741_n.jpg?oh=ef95c743d439e2f635fdcddf0e47b1eb&oe=565148FB)

### 3.2 Create database called “clouddb” ###
### 3.3 Allow “clouddbuser” to access the “clouddb” database on localhost with predefined password. ###

![a13](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xta1/v/t1.0-9/11800114_972787622766842_7737091638826257223_n.jpg?oh=ffb9bc95566f0549d894287ad7dbf560&oe=565B8C83)

## 4.Configure Apache server: ##
### 4.1 While configuring Apache web server, it is recommended that you to enable .htaccess to get a enhanced security features, by default .htaccess is disabled in Apache server. To enable it, open your virtual host file and make AllowOverride is set to All. ###

![a14](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/11800172_972787659433505_8375361115061643718_n.jpg?oh=528086b3fe088f2874700a09fbf6a782&oe=56573041)

* Add the following.

![a15](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfa1/v/t1.0-9/11822659_972787676100170_3659147236722103275_n.jpg?oh=49c9507fb4a5aaf8f1b0729a3c058936&oe=564F0012)

### 4.2 Remember to restart all services related to Apache server. ###

![a16](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xap1/v/t1.0-9/11825991_972787696100168_5465583993007228220_n.jpg?oh=9c3c862a6be96fa028973d7a12c879f3&oe=565C2CDD)

## 5.Configure ownCloud: ##

* Open up web browser, point a URL to http://your-ip-address/owncloud ( http://Your-custom-domain). Browser will automatically take you to ownCloud setup page where it must be configured before going to live. Enter admin user name, password, data folder location and database details. You can choose any one of the database from SQLite or MySQL. If you choose SQLite database, you do not require to enter database details. where as MySQL database requires database user, password and data base name.

![a17](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/11811428_972787722766832_2150495110391355710_n.jpg?oh=d0ec9d58592449a4df48bc7ec2401594&oe=564F3D43)

* Alternately you can download ownCloud client to upload the files.

![a18](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpa1/v/t1.0-9/11206959_972787759433495_7414465118415566222_n.jpg?oh=51d2f40803d0ba0b535292508676a395&oe=5658418C)