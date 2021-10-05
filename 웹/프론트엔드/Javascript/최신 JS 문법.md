![image](https://user-images.githubusercontent.com/77263282/136032326-706c84b5-edc6-4ca0-9c43-37566b00d235.png)

## ECMA 인터내셔널

ECMA 인터내셔널은 정보 통신에 대한 표준을 제정하는 비영리 표준화 기구이다. 여기서 스크립트 언어에 대한 표준을 제정하는데 그렇게 정의되는 하나의 언어가 ECMAscript이다.

더 자세하게 말하면 ECMAscript는 ECMA-262기술규격에 의해서 정의된 범용 스크립트 언어이다. 그리고 javascript언어는 ECMAscript규칙을 준수하는 범용 스크립트 언어이다.

예를들어서 ES6는 ECMA-262표준의 제 6판이다.


<br></br>
## 1. var 쓰지말고 const 와 let을 써라.

var를 특정 함수 안에서 선언했다 하더라도 밖에서 참조하는것이 가능하다. 즉, 스코프의 구분이 명확하지 않다.

그러므로 const와 let으로 쓰는것이 문제가 없다.

또한, 변경되지 말아야 할 변수를 const로 선언함으로써 디버깅 혹은 코드 수정 시 문제가 없도록 해주기 위해서이기도 하다.


<br></br>
## 2. forEach, map, filter

forEach는 배열의 각 요소에 대해서 특정 작업을 수행한다.
```
const arr = [1,2,3]
arr.forEach((element)=>{console.log(element)}

const arr = [1,2,3]
arr.forEach(function(element){console.log(element)}
```

map은 배열의 각 요소에 대해서 특정 작업을 수행한 결과요소들을 가지는 새로운 배열을 return한다.
```
const arr = [1,2,3]
const result = arr.map((element)=>{element * 2})

const arr = [1,2,3]
const result = arr.map(function(element){return element * 2}
```

filter는 배열의 각 요소에 대해서 특정조건에 대해 true가 return되는 요소들만 가지는 새로운 배열을 만들어서 return한다.
```
const arr = [1,2,3]
const result = arr.filter((element)=>{element > 2})

const arr = [1,2,3]
const result = arr.filter(function(element){return element > 2})
```

<br></br>
## 참고 문서
1. https://wormwlrm.github.io/2018/10/03/What-is-the-difference-between-javascript-and-ecmascript.html
