# Linux-users
To practice add users and delete users 

Add Users
-------------


    ~$ useradd -c “Jieun, Admin” -m -s /bin/bash -p 'mkpasswd 12345' jieun

-m : make home directory

-c : comment

-s : assign the shell

-p : make user's password


Delete Users
-----------------


    ~$ userdel -rf jieun
    
    

Add Groups
---------------

    ~$ groupadd tech
    


Delete Groups
---------------

    ~$ groupdel tech
    
    
Require user to change password 
----------------------------------
- expire user's password

   
    ~$chage -d 0 jieun
        
        
View user's password status 
----------------------------

        ~$chage -l jieun
        
        
    
    
