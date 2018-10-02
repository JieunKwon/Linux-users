# Linux-users
To practice add users and delete users 

Adding Users
-------------


    ~$ useradd -c “Jieun, Admin” -m -s /bin/bash -p 'mkpasswd 12345' jieun

-m : make home directory
-c : comment
-s : assign the shell
-p : make user's password
