### map()
모든 배열의 아이템에 function을 실행하는 Method
그리고 나서 그 함수의 결과 값으로 새로운 배열을 만듬

> ex)
<pre>
function solution(s) {
    //s "try hello world"
    return s.split(' ').map(word => {
        //s를 [try,hello,world] 배열로 만들고 배열을 map()안에 새롭게 만듬 wrod(새로만든배열) => {} 안에 새로운 내용을 추가 
        let result = ''; // result 선언
        for(let i = 0; i < word.length; i++) { //word배열만큼 반복
            if(i%2==1) { // i%2 했을때 나머지가 1이면 
                result += word[i].toLowerCase(); //소문자를 더해주고
            } else { // 나머지가 0이면 
                result += word[i].toUpperCase(); // 대문자를 더해준다
            }
        }
        return result; // 결과를 리턴
    }).join(' '); //split 했던 s값을 다시 하나로 합친다.    
}
</pre>

reference: https://programmers.co.kr/learn/courses/30/lessons/12930