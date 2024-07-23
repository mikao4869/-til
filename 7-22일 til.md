# 7월 22일 til

## 2.0 강의

### JS 파일을 열려면 어떻게 해야할까?

    중간 접착제인 HTML이 필요하다
    js 파일을 열기 위해서는 html 파일에서 열어야한다

    nico: css 와 js는 파일을 연다고 실행되지 않고, html을통해서 열어야한다

## 2.1 강의

### 숫자

- interger

      2 + 2 = 4

여기서 2는 number이라고 하지 않고
`integer`라고한다. `정수`라는 뜻이다.

`아아`

- float

       1.5

여기서 1.5는 float이다.

- 예외

        44+ 2.5= 46.5

  _integer과 float을 같이 쓸수 있다._

### string

값을 정의하기 위해서는

      "xxxx"

이런 형태이어야한다.

# 2.2

### variavles

콘솔에게 메시지를 보내는거

    console.log(숫자, string 가능)

괄호안의 값을 출력한다.

## _string할때 "xxx" 말고 'xx'도 가능할까?_

### yes

: 대신 시작과 끝의 부호가 같아야한다.

- variables: 값을 지정하거나 유지하는 역할

* const: 상수
  _(바뀌지 않는 값)_

  ### Variable을 쓰기 위해서는 const를 사용해야한다

- variables는 공백(스페이스)가 있으면 안된다\_

- 자바스크립트에서는 카멜 표현법을 사용한다

         ex) MyName

# 2-3

variable을 만드는 방법은 두가지가 있다

- const
- let

## const와 let의 차이점은?

- const는 상수이기 때문에 값이 바뀔수 없다는 의미이다.

* let: 새로운것을 생성할때 사용하는것, let은 생성할때 사용하는거

const로 variable을 만들었다면 절대 값을 업데이트 할수 없다.

### const의 값은 변할수 없지만, let의 값은 변할수 있다

    - const는 변수 재선언, 변수 재할당 모두 불가능하다
    - let은 변수에 재할당이 가능

const를 기본적으로 사용하고
variavle의 값을 업데이트 하고 싶으면 let값을 쓰는것이다.

### var이란?

원한다면 어디서든 업데이트를 할수 있다

    코드에서의 의미를 바로 찾을수 없기 떄문에 var을 잘 사용하지 않는다.

# 2-4

## boolean

- true
- false

### NULL

아무것도 없음

false와는 다름

    false는 그 값이 존재
    null은 아예 값이 존재하지 않음

null은 variable 안에 어떤것이 없다는 것을 확실히 하기 위해서 사용한다.

### undefine

값을 주어주지 않는거

---

# 2-5

## array

array를 만들기 위해서는

    [array]

이 기호를 사용한다

array는 0부터 센다

- push: 항목 하나를 array안에 추가해주는 역할

### array의 목적

    하나의 variables안에 데이터의 list를 가지는것
