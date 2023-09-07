# WpOnUbuWithAnsible
Ansible script that install locally wordpress on ubuntu.

## About
I made this for improving my ansible's skills and to understand how WordPress works, for production it's better to use other (ex. hosting service).

## Guide
Change username and password for the db in wp.yml on that line with a better password and username, if you aren't lazy:
```
shell: sudo mysql -u root -e "CREATE USER username@localhost identified by 'changeme';"
```
Run those commands for installing the service:
```
sudo apt update && sudo apt install ansible -y
ansible-playbook wp.yml
```
After that follow the instruction on your browser using the ip of your pc or localhost.
