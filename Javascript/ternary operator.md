### 삼항 조건 연산자 (ternary operator)
조건부 삼항 연산자는 JavaScript에서 세 개의 피연산자를 취할 수 있는 유일한 연산자입니다.
보통 if 명령문의 단축 형태로 쓰입니다.

조건 ? '조건이 참일때' : '아닐때'
condition ? exprIfTrue : exprIfFalse 


## 매개변수
<pre>
condition (조건문)
조건문으로 들어갈 표현식
exprIfTrue (참일 때 실행할 식)
condition이 Truthy일 때 실행되는 표현식입니다. (true일 때 치환될 값입니다).
exprIfFalse (거짓일 때 실행할 식)
condition이 falsy일 때 실행되는 표현식입니다. (false일 때 치환될 값입니다).
</pre>

reference: https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Conditional_Operator