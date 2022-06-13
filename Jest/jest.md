# jest 테스트방법
### 파일명.test.js 를 만든다

<pre>
import add from ",/파일명";

describe("testtest", () => {  // <= 테스트 묶는방법
//it테스트방법
it("함수명 test", () => {
export(add(1,2)).toBe(3);
});

//테스트 2번 방법
text("add test2", () => {
export(add(1,2)).toBe(4);
}
}
</pre>