There is an xss vulnerability in your latest version of the v5.6  
No security check in page admin/infolimg_add.php and /admin/infolimg_update.php 
When I add/update a  picture, I use "<script>alert(/xss/)</script>" as the title or the description   
  
![avatar](/pictures/pic.png)  

then when you visit case.php, you'll find xss   
  
![avatar](/pictures/case.png)   
  
Especially, case.php also has no security check   
  
![avatar](/pictures/case_php.png) 

