# JavaScript의 ES란?, ES5/ES6 문법 차이
ECMA스크립트(ECMAScript, 또는 ES)란, Ecma International이 ECMA-262 기술 규격에 따라 정의하고 있는 표준화된 스크립트 프로그래밍 언어를 말한다. 자바스크립트를 표준화하기 위해 만들어졌다. 액션스크립트와 J스크립트 등 다른 구현체도 포함하고 있다.[2] ECMA스크립트는 웹의 클라이언트 사이드 스크립트로 많이 사용되며 Node.js를 사용한 서버 응용 프로그램 및 서비스에도 점차 많이 쓰이고 있다.  

ES는 규격, 표준 즉 스펙을 뜻합니다.

js는 10일이라는 정말 짧은 기간에 만들어진 언어입니다. 그런만큼 설계상의 미스가 있을 수 밖에 없고, 그렇기에 지속적으로 버전이 업그레이드 되고, 기능이 늘어 1999년 ES3, 2009년 ES5, 2015년 ES6가 생겨 나게 되었습니다.

출처:https://ko.wikipedia.org/wiki/ECMA%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8 

> ES3

es5, es6의 문법 차이를 설명하기전에 es3부터 설명하자면 우리가 흔히 아는 js이다. 함수 단위의 스코프, 호이스팅, 모듈화 미지원, 프로토타입, 클로저 등등 자바스크립트의 기본적인 특징들이 들어있습니다.

> ES5

배열과 관련해서 새로운 메소드들이 생겼는데 대표적으로 forEach, map, filter, reduce, some, every와 같은 메소드가 생겼습니다. 이 메소드들은 개발자가 반복 횟수나 조건을 잘못 입력하는 등의 실수를 줄여주는 효과가 있습니다.

object에 대한 getter/setter 지원

자바스크립트 strict 모드 지원(더욱 세심하게 문법 검사를 합니다.)

JSON 지원(과거에는 XML을 사용하다가, json이 뜨면서 지원하게 되었습니다.)

bind() 메소드가 생겼습니다. (this를 강제로 bind 시켜주는 메소드입니다.)
> ES6 (2015 IE9부터 지원)

let, const 키워드 추가

arrow 문법 지원

iterator/generator 추가

module import / export 추가

Promise 도입