# redirect()
정말 간단합니다. return redirect 
>구문
<pre>
@app.rout('/redirect', methods=['GET','POST'])
def hello();
    return redirect("https://google.com")
</pre>

괄호 안에 redirect 시킬 주소를 입력하면 끝입니다
서버를 실행 한 뒤에, 지정해둔 주소를 웹브라우저에 입력 하면,
바로 지정해둔 페이지로 이동하는 것을 확인 할 수 있습니다.