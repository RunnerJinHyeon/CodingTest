### 1. 두 정수 a, b와 boolean 변수 flag가 매개변수로 주어질 때, flag가 true면 a + b를 false면 a - b를 return 하는 solution 함수를 작성해 주세요.

```javascript
function solution(a, b, flag) {
    var answer = 0;
    if(flag === true){
        answer = a + b;
    } else if (flag === false){
        answer = a - b;
    }
    
    return answer;
}

```

### 2. 실수 flo가 매개 변수로 주어질 때, flo의 정수 부분을 return하도록 solution 함수를 완성해주세요.

```javascript
function solution(flo) {
    var answer = Math.floor(flo);
    
    return answer;
}
```

### 3. 문자열 my_string과 정수 k가 주어질 때, my_string을 k번 반복한 문자열을 return 하는 solution 함수를 작성해 주세요.

```javascript
function solution(my_string, k) {
    var answer = '';
    for(let i = 1 ; i<=k ; i++){
        answer = my_string + answer;
    }
    return answer;
}
```

### 4. 숫자로만 이루어진 문자열 n_str이 주어질 때, n_str을 정수로 변환하여 return하도록 solution 함수를 완성해주세요.

```javascript
function solution(n_str) {
    var answer = Number(n_str);
    
    return answer;
}
```

### 5. 정수 a와 b가 주어집니다. 각 수를 입력받아 입출력 예와 같은 형식으로 출력하는 코드를 작성해 보세요.
- 입출력 예시:
1. 입력: 4 5
2. 출력:<br> a=4 <br> b=5

```javascript
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
}).on('close', function () {
    console.log("a = "+String(input[0]));
    console.log( "b = "+ String(input[1]))
});
```

### 6. 문자열 str과 정수 n이 주어집니다. str이 n번 반복된 문자열을 만들어 출력하는 코드를 작성해 보세요.

```js
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
}).on('close', function () {
    str = input[0];
    n = Number(input[1]);
    for(let i = 1 ; i<n ; i++){
        str = str+input[0]
    }
    console.log(str)
});
```

### 7. 영어 알파벳으로 이루어진 문자열 str이 주어집니다. 각 알파벳을 대문자는 소문자로 소문자는 대문자로 변환해서 출력하는 코드를 작성해 보세요.

```js
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = [line];
}).on('close',function(){
    str = input[0];
    let convertedStr = '';
    for(let i = 0; i<str.length ; i++){
         const char = str[i];
        if (char >= 'a' && char <= 'z') {
            convertedStr += char.toUpperCase();
        } else if (char >= 'A' && char <= 'Z') {
            convertedStr += char.toLowerCase();
        } else {
            convertedStr += char;
        }
    }
    
    console.log(convertedStr)
});
```

### 8. 다음과 같이 출력하도록 코드를 작성해 주세요.
- !@#$%^&*(\'"<>?:;

```js
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

rl.on('close', function () {
    console.log('!@#\$%\^&*\(\\\'\"<>?:;');
});
```