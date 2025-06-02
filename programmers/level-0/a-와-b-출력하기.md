# 원하는 문자열 찾기

## 문제 설명
정수 **a** 와 **b** 가 주어집니다. 각 수를 입력받아 입출력 예와 같은 형식으로 출력하는 코드를 작성해 보세요.

## 제한사항
* -100,000 ≤ **a**, **b** ≤ 100,000

## 입출력 예
입력 #1

```bash
4 5
```

출력 #1

```bash
a = 4
b = 5
```

## 시작 코드
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
    console.log(Number(input[0]) + Number(input[1]));
});
```

## 작업 코드
```javascript
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

const printIntegerWithName = (name, value) => {
    console.log(`${name} = ${value}`);
};

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
}).on('close', function () {
    printIntegerWithName('a', Number(input[0]));
    printIntegerWithName('b', Number(input[1]));
});
```
## 문제 풀이 후기
