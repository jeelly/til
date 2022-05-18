# replace의 새로운 사용방법 ! 

    .replace(' ','')          : 첫번째 공백 제거

	.replace(/\-/g,'')        : 특정문자 제거1 (-)

	.replace(/,/g,'')         : 특정문자 제거2 (,)

	.replace(/^\s+/,'')       : 앞의 공백 제거

	.replace(/\s+$/,'')       : 뒤의 공백 제거

	.replace(/^\s+|\s+$/g,'') : 앞뒤 공백 제거

	.replace(/\s/g,'')        : 문자열 내의 모든 공백 제거

	.replace(/\n/g,'')        : 개행 제거

	.replace(/\r/g,'')        : 엔터 제거 