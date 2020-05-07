##### Anchor-cms-0.12.7 https://anchorcms.com/
There is an XSS vulnerability in /install/routes.php. No security filtering for sitename.   
  
![avatar](/pictures/router.png)   
  
When I install the anchor-blog,and edit the sitename, I use "<script>alert(/xss/)</script>" as the sitename.  
  
![avatar](/pictures/install.png)    
  
after finishing the process, when I visit the home page:  
  
![avatar](/pictures/site.png)   
