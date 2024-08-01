# 3.7

### css에서 적용한것을 js로 불러올려면 어케 할까

    .active {
    color: tomato;
    }

css를 한다

js로 옮기고 싶어한다.

    function handletitleclick() {
     h1.className = 'active';
    }

이렇게 한다.

_함수 안에 이름을 적고 그 파일을 불러온다._

`====`는 같다는 뜻이고

`=`이면 해당값을 이 값으로 변경하라는 뜻이다.

#### 만약에 변수 이름을 잘못 써서 계속 오류가 나타나서 어떡하지?

그럴때에는

    const clickedClass = 'clicked';

이걸써서 만약에 css가 변경되어도 `''`안에것만 변경하면 되니깐 오류를 줄일 수 있다.

전체 코드

    function handletitleclick() {
    const clickedClass = 'clicked';
    if (h1.className === clickedClass) {
      h1.className = '';
    } else {
      h1.className = 'clicked';
    }

이걸하면 코드를 더욱이 깔끔하게 쓸수 있다.

# 3.8

classname을 바꾸는 다른 방법

#### classlist

두 가지 옵션이 있는데

- clasname
- classlist

#### classlist는?

    class들의 목록으로 작업할 수 있게 허용해 준다.

#### classname은?

    이전에 것들을 상관하지 않고 모든것을 변경해 버린다.

classlist에서 함수들

- contains

       우리가 명시한 class가 html element의 class에 포함되어 있는지 말해주는거

* toggle function

      classname이 존재하는지 확인을 함

if classname이 존재하면

    class name을 제거

else classsname이 존재하지 않으면

    class name을 추가

이걸 사용하면 좋은점은

    function handletitleclick() {
    const clickedClass = 'clicked';
    if (h1.classList.contains(clickedClass)) {
      h1.classList.remove(clickedClass);
    } else {
      h1.classList.add(clickedClass);
    }

}
이 긴 코드를 전부 대처할수 있기 때문에

    function handletitleclick() {
      h1.classList.toggle('clicked');
      --> string을 반복하는 순간 그때가 constant가 생성할 순간이다.
    }

아까 길었던 그 코드가

    function handletitleclick() {
      h1.classList.toggle('clicked');
    }

이걸로 대처 된것이다.

#### toggle

h1의 classlist에 clicked class가 이미 있는지 확인해서

- 만약 있다면 `toggle`이 clicked를 `제거` 해주고

- toggle은 `clicked`를 classlist에 `추가`해 줄것이다.

toggle의 정의:

    토큰이 존재한다면 토큰을 제거하고 존재하지 않는다면
    토큰을 추가한다.
