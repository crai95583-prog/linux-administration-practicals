# Linux Practical - Day 3 User & Permission Management

##  Objective
To learn how to create users, manage groups, and handle file permissions in Linux.

---

##  Create a New User

sudo adduser devopsuser

## Set or Change Password
sudo passwd devopsuser

## Create a Group
sudo groupadd devopsgroup

## Add User to Group
sudo usermod -aG devopsgroup devopsuser

 # Check groups
groups devopsuser

## Switch to Another User
su - devopsuser


# Exit back:

exit

## File Permissions (chmod)
 1) View permissions:
ls -l

2) Give execute permission:
chmod +x script.sh

3) Numeric permission example:
chmod 755 script.sh


## Change File Ownership (chown)
sudo chown devopsuser:devopsgroup file.txt

