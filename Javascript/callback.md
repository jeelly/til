### CallBack 콜백함수란

CallBack 함수란 이름 그대로 나중에 호출되는 함수를 말한다.
콜백함수라고 해서 그 자체로 특별한 선언이나 문법적 특징을 가지고 있지는 않다.
콜백함수도 일반적인 자바스크립트 함수일 뿐이다.
콜백 함수는 코드를 통해 명시적으로 호출하는 함수가 아니라, 개발자는 단지 함수를 동록하기만 하고, 어떤 이벤트가 발생했거나 특정 시점에 도달했을 때 시스템에서 호출하는 함수를 말한다.
즉 콜백함수는 콜백함수라는 <b>`유니크한 문법적 특징을 가지고 있는 것이 아니라, 호출방식에 의한 구분이다.`</b>

> 대표적인 콜백 함수의 사용 예로는 자바스크립트에서 이벤트 핸들러 처리이다.
<pre>
<button id="button1" onclick="button1_click();">버튼1</button>
<script>
function button1_click() {
	alert("버튼1을 누르셨습니다.");
}
</script>
</pre>

>Html에 onclick에 button1_click함수는 브라우저의 javascript API에서 DOM 이벤트 핸들러에 전달(등록)되고, 해당 버튼에 클릭이벤트가 발생했을 이벤트 핸들러가 콜백함수를 호출한다.
<pre>
$( "#target" ).click(function() {
  alert( "Handler for .click() called." );
});</pre>

reference : https://www.hanumoka.net/2018/10/24/javascript-20181024-javascript-callback/