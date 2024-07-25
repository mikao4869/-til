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

NaN인지 판별하는 방법
