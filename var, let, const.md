# var, let, const

javascript에선 변수를 생성하는 방법은 3가지가 있다. 

```
var test;
let test;
const test;
```

굳이 3가지나 되는이유는 이들마다 차이가있기때문이다.

var는 let보다 엄격하지 않아 var를 사용해 똑같은 변수를 선언할수있습니다. 하지만 let으로 똑같은 변수를 선언한다면 에러가 발생합니다. var는 let과 범위가 다릅니다 그래서 var로 변수를 생성해면  scope를 벗어나도 상관없이 값이 유지됩니다.

```javascript
var test = "test1";
console.log(test); // test1
if(1){
var test = "test2";
console.log(test); // test2
}

console.log(test); //test2
```

let으로 생성한다면 마지막 출력이 test1인점이 var와 다른점이죠. if문안에서 test와 밖에서 test는 다른 test가 됩니다.

```javascript
let test = "test1"
console.log(test); //test1

if(1){
    let test = "test2"
    console.log(test) //test2
}
console.log(test); //test1
```

const로 변수를 선언하면 값을 바꿀수없습니다. 다른값으로 할당한다면 에러가 발생합니다.

```javascript
const test = "test1"
console.log(test); //test1
test = "test2"
```

