<!-- conditional document -->
조건문
===
> 이 문서는 조건문 과 사용법에 대해서 간단하게 작성한 문서입니다.

## 조건문 ?

> 조건문은 특정 조건을 만족 할 때 행동을 제어하기위해 사용합니다. 대표적으로 Switch case , If 문이 있으며 python은 switch case문을 지원하지 않아, if문을 사용합니다.
>
> 

## If 기본 구조 
> if 문에서 조건은 참과 거짓을 판단 합니다.
>
> 파이썬은 코드블럭 기준을 들여쓰기로 하기에. 유의하셔야 합니다.
---
```python

    if (조건) :
        task()

```
---
    (조건)을 만족할 경우 if 내용을 실행한다. 즉 특정 조건을 충족 / 불충족할떄 실행 을 제어 할 수 있다.

## else 와 else if 

>else , else if 조건을 추가함으로써 다양한 조건에대해 실행 할 코드를 작성 할 수 있다.

### else
```python
    if (조건):
        task()
    else :
        else_task()

```

    (조건)을 만족할 경우 if 내용을 실행한다. 다만 만족하지않을 경우 else구문을 실행한다.

```python
    if (조건):
        task()

    elif (조건2) :
        task_elif2()

    elif (조건3):
        task_elif3()

    else :
        else_task()
```
    if문을 순서로 elif 의 조건을 만족한다면 해당구문을 실행한다. 
    elif 를 추가하는것으로 더많은 조건에 대해서 식을 작성 할 수 있다.
    elif 를 사용하는것으로 python에서  swich case 처럼 사용할수있다.

## if문의 다양한 조건들

- bool형 (참, 거짓) 
    - True, False : 조건의 참 ,거짓 두가지 경우사용 
    - 추가적으로 and , or , not 을 사용함으로서 여러게를 비교 할수있다.
- 비교형 ( < , = 등 .)
    - 입력값의 비교 , 수치의 값의 비교등 , 비교 조건에서 사용
- 리스트 , 튜플등 원소의 유무 확인 
    - x in (집합) 으로 작성하는것으로 사용  

```python
# 다양한 조건들

# bool형
if True:
    True_task()

# 비교형
if x < y :
    task2()

#원소의 유무
if 1 in [1,2,3,4] :
    task3()


```


## Example


```python

    for num in range(10):
        if num%2 == 0:
            print("even")
        else
            print("odd")
    
    # 홀수일경우 odd, 짝수일경우 even 을 출력한다.

```
---


```python
n , m = map(int,input().split())

if n < m and 0 < n :
    print(f"{n} 과 {m} 은 양의 정수입니다.")
    
    # 띄어쓰기로 구분된 두입력값을 받고 입력값이 숫자이 고 양의정수일경우 if문이 실행됨

```
