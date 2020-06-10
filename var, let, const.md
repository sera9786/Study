# var, let, const

javascript에선 변수를 생성하는 방법은 3가지가 있다. 

```
var test;
let test;
const test;
```

굳이 3가지나 되는이유는 이들마다 차이가있기때문이다.

* `var`는 `function-scoped`이고, `let`, `const`는 `block-scoped`입니다. (scope에 대해선 따로 주제를 갖고 설명하겠습니다.)

* `var`는 재선언이 가능함 but `let`과 `const`는 재선언 불가능 

* `let`과 `const`의 차이점은 `immutable`(불변)의 여부이다, `let`은 재할당은 가능하지만 `const`는 모두 불가능하다.

아래의 코드들을 보면 `var`, `let`, `const`들의 차이를 볼수있다. 우선 var의 경우 재선언, 재할당이 가능하기 때문에 에서 if문에서 재선언, 재할당된 test변수들을 볼수있다.

```javascript
var test1 = 1;
var test2 = 1;
console.log(test1, test2)

test1 = 2; // 재할당
var test2 = 2; // 재선언

console.log(test1, test2); //2 2
```
`let`같은 경우를 보면 재할당은 됐지만 재선언은 오류가 난다.

```javascript
let test1 = 1;
let test2 = 1;
console.log(test1, test2);//1 1	

test1 = 2;
let test2 = 2; //오류발생

console.log(test1, test2);//2 1
```

`const`는 재선언, 재할당이 모두 불가하기 때문에 오류가 난다.

```javascript
const test1 = 1;
const test2 = 1;
console.log(test1, test2);

test1 = 2;
const test2 = 2;

console.log(test1, test2);
```

const로 변수를 선언하면 값을 바꿀수없습니다. 다른값으로 할당한다면 에러가 발생합니다.
