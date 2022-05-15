# Project_5
Client/Server Architecture Using A MySQL Relational Database Management System
## Create and configure two Linux-based virtual servers (EC2 instances in AWS).
![Screen Shot 2022-05-14 at 9 18 49 PM](https://user-images.githubusercontent.com/101080172/168453400-fd8a219a-720a-42bb-80a5-d2aa4efc4518.png)
## On mysql server Linux Server install MySQL Server software.
- First we connect to our server using ssh key-gen provided by aws 
  - then we change our hostname using `sudo hostnamectl set-hostname mysql-server`
  - then we updated and upgraded the ubuntu package manager
******
![Screen Shot 2022-05-13 at 1 54 25 PM](https://user-images.githubusercontent.com/101080172/168453461-7a011271-52c0-4981-b30a-d6107d36b73e.png)
![Screen Shot 2022-05-13 at 1 54 41 PM](https://user-images.githubusercontent.com/101080172/168453478-9ced3fc2-faed-4905-8cfe-bd99a97f9c4d.png)
![Screen Shot 2022-05-13 at 1 54 54 PM](https://user-images.githubusercontent.com/101080172/168453480-fb8a8a3c-d200-4db9-9835-944f995581bd.png)
![Screen Shot 2022-05-13 at 1 55 12 PM](https://user-images.githubusercontent.com/101080172/168453516-71767bb0-9bf0-4fc9-a715-6e3956696cc3.png)
******
- We installed mysql-server, enabled it and the secured the installation
*****
![Screen Shot 2022-05-13 at 1 55 30 PM](https://user-images.githubusercontent.com/101080172/168453642-5371d3ab-f87a-4196-8cb7-bdcdc3b9cdbd.png)

![Screen Shot 2022-05-13 at 1 56 04 PM](https://user-images.githubusercontent.com/101080172/168453655-a7b5d18b-4da0-44c0-8276-129fe985feef.png)

![Screen Shot 2022-05-13 at 1 57 14 PM](https://user-images.githubusercontent.com/101080172/168453679-481301b6-54fd-4fdf-8abf-5ec6d828c77b.png)

![Screen Shot 2022-05-13 at 1 57 30 PM](https://user-images.githubusercontent.com/101080172/168453691-6234025b-6d31-4e86-a168-72a0a285cc85.png)
*****
- We went on to create a simple database 
****
![Screen Shot 2022-05-13 at 1 58 07 PM](https://user-images.githubusercontent.com/101080172/168453962-3cba4e7c-38d0-4cf9-a603-0a4bdbbb07aa.png)
![Screen Shot 2022-05-13 at 1 58 19 PM](https://user-images.githubusercontent.com/101080172/168454005-75cb51ef-ffeb-47b3-b0cb-b1e4df4c93f1.png)
![Screen Shot 2022-05-13 at 1 58 40 PM](https://user-images.githubusercontent.com/101080172/168454007-98d3c680-6761-4465-a09e-efba6c8ff292.png)

## On mysql client Linux Server install MySQL Client software

- We followed the same steps to install mysql-client software on the second ubumtu server

![Screen Shot 2022-05-13 at 1 59 09 PM](https://user-images.githubusercontent.com/101080172/168454065-e23b7828-7031-4b0b-b6bc-04c347a46d35.png)
![Screen Shot 2022-05-13 at 1 59 21 PM](https://user-images.githubusercontent.com/101080172/168454131-b086b1e7-42c0-402d-bcbb-caf4cdb1f84b.png)
![Screen Shot 2022-05-13 at 1 59 35 PM](https://user-images.githubusercontent.com/101080172/168454238-e6164b54-ee46-459e-afb5-e6ea70dc1618.png)
![Screen Shot 2022-05-13 at 1 59 51 PM](https://user-images.githubusercontent.com/101080172/168454207-f0bb884d-5b80-4a1f-bc08-2ecab65bf6c3.png)
![Screen Shot 2022-05-13 at 2 00 17 PM](https://user-images.githubusercontent.com/101080172/168454193-98e4c827-0097-47e4-816d-d91e8d4c6a49.png)
 ****
 - We  configured MySQL server to allow connections from remote hosts by changing the bind-address from‘127.0.0.1’ to ‘0.0.0.0’
  -`sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf`
 ****
 ![Screen Shot 2022-05-14 at 10 24 23 PM](https://user-images.githubusercontent.com/101080172/168455005-a9a90bee-8e8f-417a-abab-9b4b50923ce1.png)
****
 - we connected to the mysqel server through our client and show the detabases that we have created
****
![Screen Shot 2022-05-13 at 2 01 04 PM](https://user-images.githubusercontent.com/101080172/168454247-83131cdd-6661-4114-96c9-d137211cedde.png)


