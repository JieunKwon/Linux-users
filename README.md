
# Linux 1
# management users
To add and delete user account
To edit user account status

Add Users
-------------


    ~$ useradd -c “Jieun, Admin” -m -s /bin/bash -p `mkpasswd 12345` jieun

 
    	-m: make home directory
    	-s: assign the default shell
    	-G: add groups
    	-p: set user’s password with `mkpasswd xxxxx`
    	-c: set comment 


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
 expire user's password

    
       ~$chage -d 0 jieun
       ~$passwd -e jieun       
        
View user's password status 
----------------------------

        ~$chage -l jieun
        ~$passwd -S jieun
        
        
View user's password status 
----------------------------

        ~$chage -l jieun
        ~$passwd -S jieun
    
    
