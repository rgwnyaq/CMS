#### hello
------------------------  
I found a XSS in PhpMyWind CMS, which located in the vote_add.php.  
  
![avatar](/pictures/vote.png)  

But the XSS vulnerability is triggered when you write something similar to the following when filling in the title or content:  
<script>alert(4)</script>   
when users choose to vote something and click a link like:http://127.0.0.1/PHPMyWind_5.6/PHPMyWind-master/vote.php?id=2 , This vulnerability will be triggered.   

![avatar](/pictures/xss.png)  
