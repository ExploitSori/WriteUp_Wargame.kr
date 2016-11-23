#strcmp  

![source](http://sori.ml/writeup/wargame/strcmp/source.png)  

소스가 제공이 된다.  

php에서 strcmp를 할 때 배열과 문자열을 비교하면 null일때 true를 반환한다.  
따라서 html소스에서 name부분에 []를 추가해주면 문제가 풀리게 된다.  
![first](http://sori.ml/writeup/wargame/strcmp/fir.png)  
이 html코드를  
![solve](http://sori.ml/writeup/wargame/strcmp/solve.png)  

이렇게 바꾸어주면 풀리게 된다.  
