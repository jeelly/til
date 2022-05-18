
# 정규 표현식(RegEx) 


> 문자클래스, []

[]는 문자클래스를 선언하는데 사용 합니다. 이는 그 내부에 해당하는 문자열 중 하나를 고르겠다는 이야기 입니다.

>[(문자의 나열)]

[ab]: a, b중 하나를 선택한다는 이야기 입니다.
[abd]: a, b, d중 하나를 선택한다는 이야기 입니다.
[abd] 예시

JustKode, who named Min Jae Park is super babo. He not good at english. So, He studied english hard. From reading to writing, everyday he struggled. Sadly, he is still weak at english words. Yes, The above story is my story. So, If you are good at english, Call me!, justkode@kakao.com

> [(문자)-(문자)]

[a-z]: ASCII 코드상 a와 z사이 모든 문자를 선택 합니다.
[A-Za-z]: ASCII 코드상 A와 Z사이, a와 z사이 모든 문자를 선택 합니다.
[A-Za-z] 예시

JustKode, who named Min Jae Park is super babo. He not good at english. So, He studied english hard. From reading to writing, everyday he struggled. Sadly, he is still weak at english words. Yes, The above story is my story. So, If you are good at english, Call me!, justkode@kakao.com

> [^(클래스 조합)]


[^A-Za-z]: ASCII 코드상 A와 Z사이, a와 z사이를 제외한 모든 문자를 선택 합니다.
[^A-Za-z] 예시

JustKode, who named Min Jae Park is super babo. He not good at english. So, He studied english hard. From reading to writing, everyday he struggled. Sadly, he is still weak at english words. Yes, The above story is my story. So, If you are good at english, Call me!, justkode@kakao.com

 > 특수 문자 \

\는 다양한 용도로 사용 됩니다. [0-9] 같은 문구를 쓰지 않고 \d처럼 간단하게 원하는 문자열을 찾을 수 있게 해 줍니다. 밑에 예시를 들어 드리겠습니다.

- \^: 특수문자 "\"를 입력 할 수 있게 해 줍니다.
- \b: 단어의 처음 혹은 끝에 있는 문자 혹은 문자 클래스를 검출 합니다.

   - 만약 s\b 라면

        she sells seashells

    - 만약 \bs 라면

        she sells seashells

- \B: 단어의 처음 혹은 끝에 있지 않은 문자 혹은 문자 클래스를 검출 합니다.

    - 만약 s\B 라면

        she sells seashells

    - 만약 \Bs 라면

        she sells seashells

    - \d: 숫자를 찾습니다.

        My Number is 010-1010-1010

    - \D: 숫자가 아닌 것을 찾습니다.

        My Number is 010-1010-1010

    - \s: 공백문자를 찾습니다.

        Hello, World!

    - \S: 공백문자가 아닌 것을 찾습니다.

        Hello, World!

    - \t: Tab 문자를 찾습니다.

        Hello, World!

    - \w: 알파벳 + 숫자 + _를 찾습니다.

        justkode@kakao.com

    - \W: 알파벳 + 숫자 + _가 아닌 것을 찾습니다.

        justkode@kakao.com

> ## Meta 문자
- ^x: 문자열이 x로 시작합니다.

    - ^x

        xy and xz

  - ^\w

    Simple is best

  - ^\w+

    Simple is best

- x$: 문자열이 x로 끝납니다.

    - x$

        xy yx

    - \w$

        Simple is best


  - \w+$

  - Simple is best

- .: 임의의 한 문자를 나타냅니다.
 
    - .
    <br>Simple is best

    - .s
    <br>Simple is best

- x+: x가 1번이상 반복합니다.

    - i+
    <br>real illness

    - \w+

        justkode@kakao.com

- x?: x가 있거나 없는 것을 나타 냅니다.

    - colou?r

        color colour coloor

- x*: x가 0번 이상 반복 된다는 것을 나타 냅니다.

    - co*

        cl col cool coool cooool

- x|y: x 또는 y를 나타냅니다.

    - b(a|e)d

        bad bed bid

- (xy): () 안의 내용을 그룹화 합니다.

    - (lol)|(ha)

        ha haha hahaha! lol lolol lololol

- x{n}: x를 n번 반복한 문자를 찾습니다.

    - (ha){3}

        haha hahaha hahahaha

- x{n,}: x를 n번 이상 반복한 문자를 찾습니다.

    - (ha){3,}

        haha hahaha hahahaha

- x{n,m}: x를 n번 이상, m번 이하 반복한 문자를 찾습니다.

    - (ha){2,3}

        haha hahaha hahahaha

reference : https://justkode.kr/data-science/regex-1
