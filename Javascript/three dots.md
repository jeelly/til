# three dots, rest parameter, spread operator


"..." , three dots, rest parameter, spread operator


"..." 점 3개가 연달아 붙어있는 이 표시는 Spread Opertor(스프레드 오퍼레이터, 스프레드 연산자, 전개 구문, 펼침 연산자...)를 나타내는 것으로, 배열, 함수, 객체 등을 다루는 데 있어서 매우 편리하고 새로운 기능을 제공합니다.


> Spread Operator 기본 문법
<pre>
// Array
var arr1 = [1, 2, 3, 4, 5]; 
var arr2 = [...arr1, 6, 7, 8, 9]; 

console.log(arr2); // [ 1, 2, 3, 4, 5, 6, 7, 8, 9 ]

// String
var str1 = 'paper block'; 
var str2 = [...str1]; 
console.log(str2); // [ "p", "a", "p", "e", "r", " ", "b", "l", "o", "c", "k" ]
</pre>

>배열에서의 Spread Operator
<pre>
// 기존 방식
var arr1 = [1,2,3]; 
var arr2 = [4,5,6]; 

var arr = arr1.concat(arr2); 
console.log(arr); // [ 1, 2, 3, 4, 5, 6 ] 

// ES6 spread operator
var arr1 = [1,2,3]; 
var arr2 = [4,5,6]; 

var arr = [...arr1, ...arr2]; 
console.log(arr); // [ 1, 2, 3, 4, 5, 6 ] 
</pre>
<b>Spread 연산자를 이용하면 다양한 형태의 배열 병합을 비교적 간단하게 수행할 수 있습니다.</b>
<pre>
var arr1 = [1,2,3]; 
var arr2 = [4,5,6]; 
arr1.push(...arr2) 

console.log(arr1); // [1,2,3,4,5,6]


var arr1 = [1,2];
var arr2 = [0, ...arr1, 3, 4];

console.log(arr2); // [0, 1, 2, 3, 4]
</pre>