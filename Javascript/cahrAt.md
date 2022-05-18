# cahrAt()
   charAt 은 문자열에서 지정된 위치에 존재하는 문자를 찾아서 반환하는 함수입니다.

> 구문


str.charAt(index)
매개변수
0과 문자열의 길이 - 1 사이의 정수값. 
인자를 생략하면 기본값으로 0를 설정되고 첫 문자를 반환한다. 
index
반환 값
지정된 인덱스에 해당하는 유니코드 단일문자를 반환한다.
만약 인덱스가 문자열 길이보다 큰 경우 빈 문자열 (예) " " 을 반환한다.  

> 설명

문자열 내의 문자는 왼쪽에서 오른쪽으로 순번(인덱스)이 매겨집니다. 첫 번째 문자의 순번은 0, 그리고 stringName 이라는 이름을 가진 문자열의 마지막 문자 순번은 stringName.length - 1 입니다. index가 문자열 길이를 벗어나면 빈 문자열을 반환하게 됩니다.

index를 제공하지 않으면 기본값은 0입니다.

reference : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/charAt