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