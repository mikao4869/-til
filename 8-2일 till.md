# 4.0

    querySelector('#logon-form');

대상이 id인지 명확히 확인해야함

하지만

    getElementById()

를 사용할 때는 그럴 필요가 없다

왜냐하면 js가 내가 id를 찾고 있다는 것을 이미 알고 있기 때문에

##### event를 하기 위해서는

1.  이름.addEventListener("click")

2.  함수를 만든다

            function onloginclick() {

    }

#### string의 길이를 제한 하고 싶을때는

ex) 15글자 이내의 이름을 적어라

`length`을 사용한다

`length`을 사용하면 string의 길이를 구할 수있다.

string의 길이를 알고 싶다면 콘솔에다가

    string.length을 치면 글자 수가 나온다



      if (username === '') {
        alert('please werite your name');
        --> username에다가 아무것도 없을때

      } else if (username.length > 15) {
        alert('your name is too long');
      }
      --> username이 15글자를 넘어갈때
