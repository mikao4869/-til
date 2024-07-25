# 2-11

    const calulator ={
    plus: function(a,b)
    return a + b;  == 5
    }

    const plusresult=calulator.plus(2,3);

여기서 plusresult는 5가 된다

이게 가능한 이유는 return을 했기 떄문에 가능한 일이다.

## 한번 return 을하면 function은 끝난다.

한번 return 을 하면

function을 하면 그 코드는 작동하지 않는다는 의믿이기 떄문이다.

_return 밑에있는것은 실행되지 않는다_

## console.log를 하고 싶지 않는 이유

그 이유는 function 외부에서 values를 제공받기 위해서

# 2.13

# 조건문(condigional)

: true인지 false인지 알려줌

- promtpr:

        사용자에게 창을 띄울수 있도록 함
        두개의 arguments가 들어간다.

        `message`, `default`이다.

        여기서 message는 "string" 이다

_한번 사용하면 코드는 멈춘다_

- typeof: value의 type를 볼때 사용한다.

variable의 type를 보내는 법

      console.log(typeof age);

type를 변경하는 법

    string --> number

: parseInt라는 function을 사용한다.

### parseInt: string -> number

    ex)console.log(typeof '15', typeof parseInt('15'));

실행한후 숫자가 아닌 수를 누르면
`NaN`이 나온다

## 정리

    const age = parseInt(prompt('how old are you?'));

이 코드는 두가지의 function이 있는것인데,

첫번째 function(prompt)에서는 나이를 묻는 function이고,

두번쨰 function(const age)는 string을 number로 바꿔주는 function이다.

#2-14

## NaN인지 판별하는 방법

    const age = parseInt(prompt('how old are you?'));
    console.log(isNaN(age));

isNaN은 Boolean을 반환한다.

- `true` 가 나온경우:

        age가 NaN 이기떄문에

- `false` 가 나온경우:

         age가 number 이기 떄문에

true가 나오면 값이 NaN,
false가 나오면 값이 number를 뜻한다.

### conditional(조건):

     if (condition)
     {
        condition== true
    }
    else{
        condition== false
        }

_condition은 boolean이 들어가야한다._

condition을 사용하는 방법 ex)

    if (isNaN(age))
    {
    console.log('please write a number');
    }

- js는 `==` 대신 `===` 를 사용한다.

---

# 화살표 함수( arrow function)

`=>`를 사용하여 함수를 만들어내는거

### 쓰면 좋은 이유

- 입출력 기능이 직관적

- 소괄호 생략 가능, 중괄호 생략
  그러나 함수의 본문에 return문만 있는 경우이다.

## 화살표 함수 표현법,

        =>

예를 들자면

    const add = (a, b) => a + b;

---

## 함수 표현식과 화살표 함수의 차이점?

1.  우선 함수는 `function`을 사용해야한다.
    함수 표현식은 변수에 할당될수 있다.

            const add = function(a, b) {
            return a + b;
            };

    이 코드를

        const add = (a, b) => a + b;

이렇게 바꿀수 있다.

---

2. this 바인딩

일반 함수를 호출했을 때 `this`가 지정되지 않다. 하지만

### 화살표 함수는 this 가 필요 없다!
