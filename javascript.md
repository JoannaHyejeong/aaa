#Javascript

##Javascript(ECMASscript) 버전

- 2009 : ES5
- 2015 : ES6

## ES6 버전 특징

- 변수 scope 개념 확장
- class 개념 도입
- 함수 선언 형식/개념 추가
- 프론트엔드 프레임워크/라이브러리에 사용

## 프로그래밍 언어 공부

- 프로그래밍 언어 문법
- 프로그래밍 언어 활용
  - 알고리즘
  - 로직(계산 후 화면에 어떻게 표시할거냐? 논리적 흐름)
  - API 이미 만들어져있는 것을 가져다 쓰는 추세(ex.위치기반서비스 기존에 있는 지도를 이요함 그 과정에서 사용하는 것 중의 하나가 API (날씨등))물론 이게 답은 아님 기본적인것

## Javascript 문법

- 변수(데이터 타입)

- 명령문(구문)

- 함수

- 배열, 객체, class

## Javascript 활용

- 이벤트

- HTML, CSS와의 관계

## Javascript 변수 : var

https://www.w3schools.com/js/js_variables.asp

- 변수를 정의/선언할때 사용하는 키워드(예약어)
- ES5 버전에서 사용
- 값을 초기화한 후 자유롭게 변경 가능

```
var a;
var b;

var a, b;
```

## Javascript 변수 : let

https://www.w3schools.com/js/js_let.asp

- 변수를 정의/선언할때 사용하는 키워드(예약어)
- 기능상으로는 var과 같은 성질, 그러나 특징은 다름

## Javascript 변수 :const(상수 변수)

- constant : 상수(항상 같은숫자)
- 한번 값을 초기화하면 변경할 수 없음

> ES5 버전에서는 일반 변수 var 만 존재했었는데 ES6 에서는 일반변수 let, 상수변수 const가 추가

### 데이터 타임

- 숫자

  - 정수
  - 실수

- 문자

  - 문자(character)
  - 문자열(string)

- 논리
  - 참(true)
  - 거짓(false)

> 자바스크립트는 숫자, 문자, 논리 구분외에 데이터 타입을 구분하지 않음
> 자바스크립트는 숫자, 문자, 논리 데이터를 구분하는 변수 선언 키워드가 없음
> 데이터 타입을 구분해주는 자바스크립트 : 타입 스크립트

## Javascript 연산자

https://www.w3schools.com/js/js_operators.asp

### 산술 연산자

- +, -, \*, /, %(나머지)

### 대입(할당) 연산자

- =
- +=

```
b = a + 1;

a = a + 2; //여러번 실행시 2씩 증가하는 식

a += 2;
>>>>>>>>>>>>>>>>>>>>>>>>>
a = a + 1;

a += 1;

a++;
>>>>>>>>>>>>>>>>>
a = a - 1;

a -= 1;

a--
>>>>>>>>>>>>>
```

> ++, -- 증강 연산자

### 연결 연산자

```
"a" + "b" => ab

"a" + 1 => a1

"1" + 1 => 11

console.log("총합계 : " + sum);
```

### 따음표 사용방법

'''
element. innerHTML = "<imga src=\"picture.jpg\">"

element. innerHTML = '<imag src="picture.jpg">'
'''

### 비교 연산자

- ==, === : 데이터 타입을 동시에 비교 여부

- 비교 연산의 결과는 논리 데이터가 출력 : true / false

### 논리 연산자

- 여러개의 비교식을 연결해서 연산할 때 사용
- 논리 데이터를 연산할 때 사용

> &&(and) : &&로 연결되는 비교식 또는 논리데이터가 모두 참일 때 전체가 참

```
true && true => true
true && false => false
3<5 && 10<12 => true
```

| : pipe line

> ||(or) : ||로 연결되는 비교식 또는 논리데이터가 하나라도 참이면 전체가 참

```
true || true => true
true || false => true
3<5 || 10>12 => true
```

## 명령문/구문 Syntax

- 프로그램 실행 흐름을 제어 역할

### 조건문/분기문

> if 구문
> https://www.w3schools.com/js/js_if_else.asp

```
if(conditions){
  // 코드블럭
}

if(conditions){
  // 코드블럭 1
} else {
  // 코드블럭 2
}

if(conditions){
  // 코드블럭 1
} else if(conditions 2){
  // 코드블럭 2
} else {
  // 코드블럭 3
}
```

> conditions 식의 결과가 true이면 코드 블럭을 실행 false 이면 실행하지 않음
>
> conditions : 결과가 true/false가 나오는 식
>
> 숫자를 논리 데이터로 인식
> 0 :false
> 그 외의 정수 : true

> if 사용법
>
> - else if(){} : 필요한 개수만큼 사용 가능
> - else : 맨마지막 부분에 사용

> switch 구문
> https://www.w3schools.com/js/js_switch.asp
> expressions 식의 결과에 따라 여러 갈래로 분기
>
> expressions : 결과는 숫자, 문자의 형태 (true, false 와는 아무관계가 없음)

```
switch(expressions){
  case '결과값1'
    코드블럭1;
    break;

    case '결과값2'
    코드블럭1;
    break;

    case '결과값3'
    코드블럭1;
    break;

    default:
    코드블럭 4;
}
```

### 반복문

> for loop
> https://www.w3schools.com/js/js_loop_for.asp
>
> - 특정 횟수만큼 반복 실행

for/in 과 for/of 는 중요하지만 어려워서 이번엔 다루지 않고 for 와 while 만 다룰예정

###

https://www.w3schools.com/js/js_break.asp

## 함수(funtion)

https://www.w3schools.com/js/js_functions.asp

- 특정한 기능을 실행(독립적으로 실행)할 수 있는 여러 코드를 묶어놓은 블럭
- 함수는 선언과 호출로 구성
- 선언(declaration) : 함수 정의(definition)
- 호출(call) : 함수 실행
- 함수는 재사용이 가능하다

## 배열, 객체, class

- 데이터, 함수의 집합

### 배열(array)

배열은 한 번에 둘 이상의 값을 보유할 수 있는 특수 변수입니다.
https://www.w3schools.com/js/js_arrays.asp

> 배열 데이터가 메모리에 생성되는 구조
>
> - 일반 변수는 선언이 되었을 때 메모리에 값이 직접 할당되는 형태이고, 배열 변수는 메모리에 배열 데이터가 저장된 곳의 주소값이 할당되는 형태
> - 배열 변수가 const로 선언되었을 때 각 원소들의 변경에는 영향을 미치지 않고, 배열 자체가 변경될 때는 영향을 미치기 때문에 변경할 수 없음

### 객체(object)

> 프로그래밍 상의 데이터를 객체라는 개념으로 대상화시키는 것
>
> 객체
>
> - Property
>
>   - 객체가 가지고 있는 속성, 특성
>
> - Method
>
>   - 객체의 기능, 동작
>     객체 데이터는 name:value 한 쌍으로 구성됨.
>   - name:value 형태는 key:value 형태로도 이야기 함
>
> - 객체 method에서 this 키워드를 사용하면 method를 소유하고 있는 (포함하는) 객체를 가리킨다.

> 내장객체
>
> - js에서 기본으로 가지고 있는 객체
> - Array, Date, Math 객체가 있다

### Class

https://www.w3schools.com/js/js_classes.asp

> 객체 데이터를 여러개 생성할 수 있도록 하는 설계도
>
> new 키워드를 사용하여 객체 데이터를 생성
