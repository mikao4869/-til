# TO DO LIST

    <form id="todo-form">
      <input type="text" placeholder="write a to do and press enter" required />
    </form>
    <ul id="todo-list"></ul>

## 여기에서의 form과 ul을 HTML에서 js로 가져오는 방법은?

    const todoInput = todoForm.querySelector('input');

요거랑

const todoInput = document.querySelector(' #todo-form input');

는 같다!

    const newTodo = toDoInput.value; //값 저장 하는거
      toDoInput.value = ''; //그 다음 값 비움
      console.log(toDoInput.value); //
      console.log(newTodo, toDoInput.value);
      //newTodo에 값은 아직 있음

여기에서

    console.log(newTodo, toDoInput.value);

이거에 결과는

newTodo 하나인데 그 이유는
