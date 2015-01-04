Function
=====

함수 작성하기
----
두 가지 숫자를 받아서 더한 값을 되돌려주는 함수
```js
var sum = function(a,b){
  return a+b;
}
```
```js
console.log( sum(1,2) ); // 3
```

여러 개의 값 입력 받기
----
여러 개의 값을 입력받고 싶을 때는 배열을 argument로 넘겨주면 됩니다.
```js
var sum = function(ary){
  var s = 0;
  for(i=0;i<ary.length;i++)
    s += ary[i];
  return s;
}
```
```js
console.log( sum( [1,2,3,4,5] ) ); // 1+2+3+4+5
```


여러 개의 값 리턴하기
----
마찬가지로 배열을 return 하면 여러 개의 값을 돌려줄 수 있습니다.
```js
var foo = function(){
  return [1,2,3,4];
}
```
```js
console.log( foo() ); // [1,2,3,4]
```

문제
----
* 숫자를 넘겨주면 __홀수__인지 __짝수__인지 판별하는 함수를 작성하세요
  * 함수의 이름은 evenOrOdd로 작성하세요
  ```js
  console.log( evenOrOdd(5) ); // '홀수'
  console.log( evenOrOdd(2) ); // '짝수'
  ```
* 숫자를 넘겨주면 해당 숫자가 소수(prime number)인지 아닌지 판별하는 함수를 작성하세요
  * 함수의 이름은 isPrimeNumber로 작성하세요
  ```js
  console.log( isPrimeNumber(3) ); // true
  console.log( isPrimeNumber(4) ); // false
  ```
  * [참고링크](http://blog.naver.com/vest2004/220046281712)
  * [참고링크2](http://blog.naver.com/jordanhuh/70134571159)
