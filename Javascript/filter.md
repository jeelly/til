# filter() 
메서드는 주어진 함수의 테스트를 통과하는 모든 요소를 모아 새로운 배열로 반환합니다.


> filter 정의
    Array.prototype.filter ( callbackfn [ , thisArg ] )

filter는 해석 그대로 걸러주는 역할을 하는 함수입니다. 주로 특정 조건을 만족하는 새로운 배열을 필요로 할 때 사용하는 편입니다.


<pre>
const numbers = [1, 2, 3, 4, 5]; 
const result = numbers.filter(number => number > 3); 
console.log(numbers); // [1, 2, 3, 4, 5]; 
console.log(result); // [4, 5]
</pre>
reference: https://7942yongdae.tistory.com/49 [프로그래머 YD]