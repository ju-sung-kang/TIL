## search 함수에 대해서

mdn에 검색하면 마치 정규 표현식으로만 써야하는것으로 나오지만 그렇지 않음
```javascript
let test = "hello world"

test.search("h") // => 0을 리턴
test.search("z") // => -1을 리턴
```

참고 문서
1. [자바스크립트의 search함수](https://redcow77.tistory.com/595)
