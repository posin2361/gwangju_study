<!-- readme. md  
    귀찮다. 😒
-->


서문 
======================
## ⚠️ 주의!
 
> 1. 이 글은 이번주차에 대한 서문으로 굳이 읽지 않아도 공부에는 전혀 문제 될 것이 없는 글입니다.
> 2. 이 글은 글재주도 말재주도 없는 글쓴이로 인해 불쾌감 및 졸음이 유발될 수 있는 글임을 알립니다.
> 3. 이 글은  전적으로 글쓴이의 생각을 기반하여 주관적으로 작성된글이며 스터디그룹의 의견과 다를 수 있음을 알립니다. 
  

![그림파일!]( https://i.pinimg.com/736x/1d/4e/81/1d4e8172c673e187d3e5a291c9a2c5b7.jpg "그림파일")

## 1. 사실 반복문 없이 프로그램 구현하는것은 문제없다. 🙃

엥 이게 무슨소리인가? 놀랍게도 맞는말이다 가령 위의 이미지처럼 칠판에 글씨를 적는 프로그램을 작성해본다고 가정해보자.

```python
write = "I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT" 
# 나는 내 벌을 대신 수행한 동생에게 아무보상도 안해줄거다. ~ 🤣  
print(write)
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
```

잠깐만요 이러면 해당지문 이 한번만 출력되는거 아닌가요 ? 

생각해보니 그런거같다.

다시 고쳐써보자. 

```python
write = "I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT"
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
print(write)
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
>>> I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT
# .. 칠판크기만큼 추가 !
```

짜잔! 이러면 wrtie 와 print만 사용한 프로그램을 만들 수 있다.

## 2. 그럼 왜 써야하는데 ? 🤔

> 왜 써야할까 라는 질문에 대해서는 진지하게 생각해 본 적이 없다.<br>
> 확실하게 말할수 있는건 변수나 input , output처럼  컴퓨터가 인간이 원하는 동작을하게끔 만드는데 완전한 필수조건은 아니다. 하지만 반복문을 사용하지 않을때 생기는 다음과 같은 문제들이 있다.<br>

 

    


### 2.1 일의 효율 문제 
 
    위 1번에서 나온 문제를 해결하는데 반복문을 이용하면 10줄 20줄 쓸 코드를 확 줄일 수 있다.

```python 
write = "I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT"
#위 1번의 칠판에 글을 쓰는코드를 반복문을 사용하면 3줄로 확 줄일수있다. 
for size in whiteboard :
    print(write)
```

    
    어짜피 복사 붙여넣기 하면 그만인데 ctrl + c,v 몇번 더누르면 되는거 아닌가 라고 반문한다면 
    칠판 크기가 변하고 print 뿐만아니라 다른 함수도 같이 동작하는 다른 프로그램이라면 어떨까 ? 
    추가해야할 행동이 두개 세개를 넘어 더 복잡한 행동을 해야하는 프로그램이나 장치를 만들어야한다면 
    복사 붙여넣기하는 것도 큰 일일 것이다. 컴퓨터는 인간의 효율을 위해서 발명된 도구이지 
    효율을 위해서 만든 도구로 비효율적인 일을 한다는건 정말 슬픈 일이지않을까 🤔


### 2.2 유지 보수의 문제 
    
    만약 위의 1번의 반복문을 쓰다 오탈자가 생겨 출력문이 이상하게 된다거나 
    괄호를 빠트려 프로그램 실행 자체에 문제가 생기는 경우 원인을 찾기위해 
    소스코드를 하나씩 찾아 봐야할 것 이다. 위의 경우는 print 문의 12번 실행이지만
    작성 코드줄수가 100만 , 200만 이아니라 50줄 100줄만 되도 오탈자 찾기란
    사막에서 떨어트린 유리구슬 찾는것 만큼이나 눈알 빠지는 일이 될것이다.
    
### 2.3 용량의 최적 문제 
    
    
    위의 1번과 같은경우는 크기가 크지않고 한행동의 반복이라 코드를 읽기에는 (매우) 불편할지라도 프로그램 실행에는 문제없다. 
    그럼 굳이 반복문을 사용하지 않아도 되는게 아닐까 ? 라는 의문이 생길수있다. 

    위의 칠판에 쓴 글을 출력하는 프로그램의 글자수는 총 798자(공백포함)으로
    용량으로 따지면 798byte 를 차지한다.
    
    위의 칠판 프로그램을 반복문을 작성하면 
    
```python 
write = "I WILL NOT PAY MY SISTER TO DO MY PUNISHMENT"

for size in whiteboard :
    print(write)
```
    이런식으로 반복문을 사용해서 코드를 만들면 총97자(공백포함)으로 용량은 97byte 
    단순히 위의코드와 비교해 7~8배정도 효율적인 코드를 작성 할 수 있을뿐더러 훨씬 보기좋다. 😊

##  3. 그럼 안써도 되는거야 ? 🙄

![funcool](https://upload3.inven.co.kr/upload/2020/05/19/bbs/i013308301945.gif)

    
    단언컨대 ! 아니다.

    프로그램 은 대부분 혼자 작성하는 일이 없으며 당장 지금은 혼자서 코드를 짜더라도 언젠가 
    옆자리의 동기 , 선배 혹은 취직후 동료들과 같이 코딩을 같이해야하는 상황이 올수있다.  
    그 떄가 왔을때 이 글이 생각나서 
    " 누가 저번에 반복문 안 써도된데요 ~ " 하면서 나만의 길을 개척하는 힙스터는 없기를 바란다. 

    적절한 반복문으로 fun 하고 cool 하고 sexy 한 코딩을 하는 멋진 사람이 되도록 하자. 😘
    
