#db_is_really_good  
![fisrt](http://sori.gq/writeup/wargame/db_is_really_good/first.PNG)  
닉네임을 입력하라는 것 같다.  


![chat](http://sori.gq/writeup/wargame/db_is_really_good/chat.PNG)  
닉네임을 입력하니 실시간 채팅 창이 나온다.  
XSS과 injection을 해보니 아무것도 안된다.  

![dbexcept](http://sori.gq/writeup/wargame/db_is_really_good/dbexcept.PNG)  
로그인 창에서 각종 문자들을 입력하다가 '/'를 입력하면  
php상에서 Exception이 발생하게 된다.  
에러를 읽어보면 DB를 불러와서 채팅창이 운영되는 것 같다.  

따라서 admin의 db를 불러오면 될 것 같아서 경로와 이름을 맞추어 주면 db가 다운이 된다.  

http://wargame.kr:8080/db_is_really_good/db/wkrm_admin.db  
![down](http://sori.ml/writeup/wargame/db_is_really_good/down.PNG)  
db를 sqlite Browser로 열어보면 플래그가 나온다  
