<!-- loop_main  readme.md-->

반복문
===


    반복문은 프로그램에서 똑같거나 일정 패턴의 행동을 반복하여 수행하도록 하기위해
    제어하는 명령문입니다. python 에서는 For와 While 그리고 Do while 을 통해
    반복문을 사용할 수 있다. 어떤 프로그래밍을 작성하는지에따라 적절하게 사용 하도록 하자!

## 1. 

> 


## 2. Pass, Continue, Break

    반복문에서 공통적으로 사용되는 반복문을 제어하기 위해 사용하는 구문 

### 2.1 Pass

```python 
    # Pass 1
    for value in value_list :
        pass

```
> Pass 는 반복문 뿐만아니라 class 등에서도 사용되며 
>
> 반복문에서는 조건문에 딱히 넣어줄게 없을경우 넣습니다. 실제로는 어떤동작도하지않지만
> 프로그램 사용시 '빈칸을 채우기 위해 명시해 둔다' 이정도로 이해 하면 좋을거 같습니다.
    

### 2.2 Continue

```python
    # Continue 1
    for value in range(10):
        if value % 2 == 0:
             continue
             print(value) # 실행되지 않음 x(
        print(value)
    print("finish")    
```
<details>
  <summary>Answer</summary>

  ```python
  >>> 1
  >>> 3
  >>> 5
  >>> 7
  >>> 9
  >>> finish
  ```
</details>

> Continue 문은 반복문에서 특정 조건에서 해당 루프를 건너뛸때 사용한다. 
> 
> 위의 예제 에서는 0~9 의 값중 /2 의 몫이 0 일경우 continue를 하는 반복문이다.
>  
> 결과적으로는 홀수만 출력되고 루프문이 종료된다.
>
> 반복문에서 continue 를 만날경우 해당 번째 루프를 건너뛰고 다음 루프를 진행 하는것으로 이해하면 좋을거 같습니다.


### 2.3 Break

```python
    # Break 1
    for value in raange(10):
         if value % 2 == 0:
             break
             print(value) # 실행되지 않음 x(
        print(value)
    print("finish")
```


<details>
    <summary>Answer</summary>

    ```python
        
        >>> finish

    ```
</details>


> Break 문은 반복문에서 특정 조건에서 루프를 인위적으로 종료시키기위해 사용합니다.
>
> 위의 예제는 0~9 값중 나머지가 0이면 break문이 실행되면서 for문에서 실제로 출력되는값은 
>없습니다.
> break 문을 만날경우 해당 루프를 종료 한다고 이해 하시면 될거 같습니다.