스택(stack) : 더미를 쌓아 놓는다.

스택의 구조 : 후입선출(LIFO)을 한다

스택의 중요한 연산
push() = 스택에 데이터를 추가한다.
pop() = 스택에서 데이터를 삭제한다.

스택이 공백상태라면 -1

![image](https://user-images.githubusercontent.com/103267689/163111797-e71bb9a6-4f8c-4b84-a3f5-d770e74f2ba6.png)

    
스택이 포화 상태라면 MAX_STACK_SIZE -1

![image](https://user-images.githubusercontent.com/103267689/163112003-083dc40d-6889-49d4-bbf5-8fad501a5e38.png)
    
동적 배열 스택은 프로그램을 실행할 때 메모리를 할당 받는다.
정적 배열 스택은 메모리를 프로그램 실행 전에 할당받는다.

수식의 계산에는 전위, 중위, 후위의 표현이 있다.

후위 표기식의 계산
수식을 왼쪽에서 오른쪽으로 스캔하며 피연산자이면 스택에 저장하고, 
연산자이면 필요한 수만큼의 피연산자를 스택에서 꺼내 연산을 실행하고 연산의 결과를 다시 스택에 저장한다. 
ex) 82/3-32*+   결과 값은 7이다.
