### input함수

#### 개요
파이썬에 표준 입력 input 함수 사용에 대해 설명한다.

#### input()
```
a = input()
print(a) # 123 입력했다면
>>>123
```

두개 이상 입력 받기
```
a, b = input().split() # 입력 받은 값 공백으로 분리
print(a)
print(b)
```
숫자 2개 입력 받기
```
a, b = map(int, input().split())
print(a+b)
```
,으로 구분하기
```
a, b = map(int, input().split(','))
print(a+b)
```
