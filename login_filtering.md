#login_filtering  
![first](http://sori.ml/writeup/wargame/login_filtering/first.PNG)  
제공되는 소스를 봅시다!  
![phps](http://sori.ml/writeup/wargame/login_filtering/phpsource.PNG)  
쿼리를 날려 나오는 값이 blueh4g이거나 guest이면 플래그를 출력해줍니다  
![html](http://sori.ml/writeup/wargame/login_filtering/htmlsource.PNG)  
html소스를 보면 아이디와 패스워드가 적혀있습니다.  

blueh4g라는 계정으로 로그인 하려면 id : blueh4g pw : blueh4g1234ps이어야 합니다.  
하지만 php에서 blueh4g라는 문자열을 필터링하고 있습니다.    
mysql에서는 대소문자를 비교하지 않는 성질을 이용하여  
id blueh4G를 입력하고 pw는 blueh4g1234ps를 입력하면 클리어 됩니다.  
