<!-- while readme.md -->
While
===
> 이 문서는 While 반복문에 대해 설명하는 문서입니다.

## While 반복문

    while 반복문은 조건의 충족/불충족 에 대해 제한할 때 사용합니다.

## 기본적인 while 🤔

```python

    # while 기본형
    while 조건 : 
        행동()

```
>while 의 조건이 만족한다면 행동을 한다.! 라고 이해하면 좋다.
>
>다른 언어에서 while 을 접해 봤다면 이해하기 쉬울것이다. python도 문법의 차이가 있을 뿐
>사용법은 같다.

```python

    # while 예문 1
    x= 0
    while x < 5 :
        print(x , end=" ")
        x= x+1
    
```



##  + Do While  😅

> python 에서는 do while 문을 지원하지않는다.! 하지만 반드시 한번은 실행 되어야 하는 반복문이라면 반복조건을 뒤에서 확인하도록 작성하면 된다.

```python
    # Do while 처럼 사용하기 1    
    while 조건 :
        task()
        if condition :
            break

```

> 조건을 만족할 경우 종료 . 😎

```python
    
    #Do while 처럼 사용하기 2
    while :
        task()
        if not condition :
            continue
        break

```

> continue를 통해 조건을 만족하지 않는경우 반복하게도 작성 가능하다. 😮

## 무한 루프문

```python
    
    #while 무한 루프문
    while True:
        task()

```

> while 반복문은 조건에 대한 반복문이다. 조건이 항상 참인경우 루프문이 계속 반복하게된다. 보통 while True(python 에서 True 첫글자는 대문자로 작성함으로써 값의 참을 명시한다.)로 나타내며 True가 아니라 조건이 참이라면 위의 예문과 같이 무한 루프문으로 동작한다. 

### Example

```python
    # while example 1
    num = 5
    start = 1
    while start < 10: 
        print(f"{num} * {start} = {num*start}")
        start +=1

```
<details>
  <summary>Answer</summary>
    구구단 5단을 출력한다.
</details>

```python
    # while example 2 
    
    while True:
        print("종료 하시려면 \"종료\"를 입력해주세요")
        if input()=="종료":
            break

```

<details>
  <summary>Answer</summary>

    사용자가 "종료" 를 입력하기 전까지 반복한다.
</details>

