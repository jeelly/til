# scrollIntoView()
원하는 내용이 있는 위치로 이동시켜야 한다거나 그럴 때 사용합니다.

>▷ 구문
<pre>
    element.scrollIntoView();
    element.scrollIntoView(alignToTop); // Boolean parameter
    element.scrollIntoView(scrollIntoViewOptions); // Object parameter
</pre>
보는것처럼 3개의 문법이 존재하는데
첫번째로 아무 매개변수도 사용하지 않고 그냥 사용하는방법과
두번째로 Boolean parameter true/false를 매개변수로 사용하는 방법
세번째로 options 객체를 넣어서 사용하는 방법이 존재하는데

요즘같은 화면구성으로는 아마 세번째 방법인 옵션을 주는 방법을 주로 사용할것이다.

>▷ 두번째 문법 (alignToTop)
 - true : element 요소의 상단을 기준으로 스크롤을 이동한다.
 - false : element 요소의 하단을 기준으로 스크롤을 이동한다.

<pre>
    document.getElementById("mine").scrollIntoView(true);
    document.getElementById("mine").scrollIntoView(false); 
</pre>
>▷ 세번째 문법 (scrollIntoViewOptions)
 - behavior : 전환 에니메이션 정의 (auto || smooth)
 - block : 수직 정렬 (start || center || end || nearest)
 - inline : 수평 정렬 (start || center || end || nearest)

<pre>
    var element = document.getElementById("mine");
    element.scrollIntoView({behavior: "smooth", block: "end", inline: "nearest"});
</pre>
    
reference : https://mine-it-record.tistory.com/399