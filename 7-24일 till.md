# 2-10

console은 사실 object라는 것을 알수 있다.

## object에서 item을 업데이트 하는 법

    name:"nico"
    --> player.name="nocolas"

## object의 item을 가져오는 방법

    player.name

# function을 실행시키기 위해서는 !!!!

    ()가 필요하다

function은 body안에서만 사용이 가능하다

# 2-11

console.log는 console에 무언가를 log 하는거

        const calculator = {
         add: function (a, b) {
           console.log(a + b);
        },
        minus: function (a, b) {
          console.log(a - b);
        },
        divide: function (a, b) {
          console.log(a / b);
        },
        xx: function (a, b) {
          console.log(a ** b);
        },
        };

            calculator.add(1, 1);
            calculator.minus(1, 1);
            calculator.divide(1, 1);
            calculator.xx(1, 1);

함수가 그냥 어떤 기능을 수행하는것이라고 생각하기보단

`함수`는

    어떤 일을 수행하고 그 결과를 알려주는 거라고 생각해라

# return

## funtion 안에서 console.log을 하지 않는경우 어떻게 될까?

이 말은 우리는 항상

    const calculator = {
    add: function (a, b) {
    console.log(a + b);
    },

    calculator.add(2, 3);

이런 식으로 function 안에서 console.log를 불러왔는데 그러지 않고,
function밖에서 console.log를 부르면 어떻게 될까?

### : retur을 쓰면 된다

무언가를 return 하면
계산을 담당하는 function의 코드는
그 function이 return 하는 값과 같아질거야.

    const age = 96;
    function calculatekrage(ageofforeigner) {
    *return* ageofforeigner + 2;       //ageofforeigner +2 의 값이
    }

    const krage = calculatekrage(age);    ==98       //여기에  값과 같아진다.

    console.log(krage);

function이 function 밖과 소통하는 방법: return

### return

        어느 작업을 하고 그 작업의 결과를 알려주는 function

return 하는 것은 console.log를 하는것이 아니라 결과값을 보여준다

<<<<<<< HEAD
함수를 호출할때는

    const calculator ={

    plaus:function (a,b){
    return a+b; //값을 반환
    },
    };

    const plusresult=calculator.plus(2,3); //함수 호출
     console.log(plusresult);

## 이런 짓을 하는이유(function안애서 console.log를 쓰지 않은 이유)

:console에서 값을 가져올수 없었는데 코드에서 결과값을 알수 있기 떄문에
=======
아아아
>>>>>>> a78d92cecf59f23cb2712074482532756b107b68
