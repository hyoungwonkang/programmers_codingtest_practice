# 풀이

1. slice를 써서 배열을 만든다
2. commands의 세번째 원소로 값을 return 한다.

# 코드

function solution(array, commands) {
var answer = [];
let arr = [];

    // slice를 써서 배열을 만든다
    // commands의 세번째 원소로 값을 return 한다.

    for( let i =0; i < commands.length; i++){
    arr[i] = array.slice(commands[i][0]-1, commands[i][0+1]).sort((a,b)=>a-b)[commands[i][0+2]-1]
    }
    return answer = arr

}

```js

```
