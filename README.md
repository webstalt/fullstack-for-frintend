# fullstack-for-frontend

## Why?
To become a better engineer
To be able to solve much more number of issues, to be able to create the apps from start to the end,
To understand what's going on at the different stages of the development

The Internet works through the series of tubes. Internet is a system of globally interconnected devices.
If you use VPN, you're in the intranet - a private internet, inaccessible from outside.

man [command] - to get the info about the command

### VIM (means Vi improved)

| mode      | how to enter |
| :---        |    :----:   |
| insert mode (type text)      | i       |
| command   | esc        | 
| last line   | :        | 

how to quit vim: **:q!**

cheatsheet: https://linuxmoz.com/vi-commands-cheat-sheet/

cd ~ - go to the user directory
cat ... - show file content

### Server 

What does it do? It serves content
Everything thats gets requests and responds to it can be a server

### OS

I. unix:
1 BSD (freeBSD is used on macOS)
2 Linux: ubuntu, debian, red hat etc.
3 Solaris
II. windows

LTS version - long term support. Choose this version for huge projects to have a support from the manufacturer.
SSH - secure socket shell - for security. Idea of ssh: i have a private key on my computer, and the server sends me encrypted data. Only I can read it because i have my private key. I share it with the server once to get it know how to encrypt the message.
We can create several keys with different names. .pub can be shared, sent by email. Private shouldn't be shown to anybody.
cd ~/.ssh
ls | grep <filename to be searched>
cat <filename> - to show the file content

ssh -i <private-key-filename> root@<ipv4-from-digitalocean>
-v command is useful for debugging - shows whats going on
exit - to go to my normal computer = exit the server

### HOW TO CONNECT
ssh servername@ip
apt update - always keep your server up-to-date
apt upgrade
  
sudo = super user do
sudo !! = run last command with sudo

sudo tail -f  <server> = the most powerful tool for debugging, follows the new lines in the files. 

USER PERMISSIONS
ls -a  = shows hidden files in a directory

### NGINX
reserve proxy, web server, proxy server
it is a popular web server, another one is Apache (goes well with php)

NODEJS - is a js engine that runs on top of V8, which is developed by google chrome, it's usually a few versions behind (chrome has more new features). node js is a single threaded js engine that executes js and can handle requests.

&& - use it to chain commands. ex., git pull && yarn install
installed express js, run a server 
/var/www/app$ node app.js - to start a node application


fail2ban - or smth similar must be used on a production server. can try it on this project, but here it's not so important. bans attepmts to login failed 5 times and prevents running dangerous scripts. 
express

### HOW the internet works:
domain -> IP -> server -> web server (nginx for ex) -> application server (express.js)

HTTP
res.set() - to set a header
res.status() - to set a status

containers,
docker
orchestration with kubernetes (k8s)
load balancing (can do it with nginx - easily but take care about logging in the servers)
deployment with ansible / puppet - to deploy several servers at once
  
  
https://frontendmasters.com/courses/fullstack-v2
