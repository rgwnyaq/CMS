
I found a sql Injection in bluecms. It's exact location is in line 149 of /uploads/admin/ad_phone.There is no filtering of "id",attacker can attck by using sql injection by control the id that upload by GET.   

As shown in the picture:  

![avatar](/pictures/ad_phone.png)   

We can use query such as:" DELETE FROM blue_ad_phone WHERE id=1 and updatexml(1,concat(0x7e,(SELECT @@version),0x7e),1);" to get some imformation of database.  
The attack result is as follows:  

![avatar](/pictures/result.png) 
