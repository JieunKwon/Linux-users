
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

Mkpasswd 
--------------
        
    ~$ sudo apt install whois

         need to install whois to use mkpasswd

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
    
    
Change User Setting
-------------------------
    ~$usermod Option UserAccount
    
    ~$usermod -e 2018-10-15 jieun
    // -e expire date : jieun account will be expired by 2018-10-15
   
     

Add group
--------------	    
    ~$ groupadd Groupname


Delete group
------------------------
    ~$groupdel Groupname

View User Account
------------------------
    ~$tail -n10 /etc/passwd
    ~$less /etc/passwd
     
View User Password
----------------------
    ~$sudo tail /etc/shadow
       
Switch user
---------------------
     ~$su - jieun
    
View Group
-------------------
    ~$tail /etc/group
