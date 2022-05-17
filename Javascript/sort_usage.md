# 잘못 알았던 사실

> 오류가 자꾸 나서 이유를 찾아보았는데 <br>
> <b>숫자에서만 통하는 정렬방법이였다. </b>
<pre>
numbers.sort((a, b) => a - b);  // 오름차순 정렬
numbers.sort((a, b) => b - a); // 내림차순 정렬
</pre>


>문자 오름, 내림차순 정렬
<pre>
.sort(function(a,b) {return a < b ? -1 : a > b ? 1 : 0;})  
.sort(function(a,b) {return a < b ? -1 : a > b ? 1 : 0;}) 
</pre>