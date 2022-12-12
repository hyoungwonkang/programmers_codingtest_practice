# 풀이

1. 유클리드 호제법으로 최소공배수를 구하는 함수를 만든다.
2. 배열의 순서대로 요소를 넣어 제일 큰 수를 제일 마지막에 넣어 마지막 최소공배수를 만든다.

# 코드

function solution(arr) {

    const gcd = (a, b) => {
      while (b > 0) {
        let temp = b;
        b = a % b;
        a = temp;
      }
      return a;
    };

    const lcm = (a, b) => {
      return (a * b) / gcd(a, b);
    };

    let answer = 1;
    arr = arr.sort((a,b)=> b-a)
    for (let i=0; i<arr.length; i++){
        answer = lcm(answer, arr[i])
    }
    return answer

}

```js

```
