### 확장 문장 출력

#### 개요
출력에 필요한 재공되는 확장 문장


따옴표 문자(작은 따옴표) - \'
```
print('나의 이름은 \'한사람\'입니다.')
>>>나의 이름은 '한사람'입니다.
```
쌍따옴표 문자(큰 따옴표) - \"
```
print("나의 이름은 \"한사람\"입니다.")
>>>나의 이름은 "한사람"입니다.
```
엔터 - \n
```
print("Hello \nWorld!!")
>>>Hello
World
```
```
print("Hello \012World")
>>>Hello
World
```
```
print("Hello \0AWorld")
>>>Hello
World
```
print \ 에 정체는?
```
print('\156')//8진수로 출력되며 숫자 156(8진수)에 아스키코드 값은 n 이다.
>>>n
```
tab - \t
```
print('Hello \tWorld!!')
>>>hello   World
```
바로 아래로 엔터 - \v
```
print("\nhello \vworld")
>>>
hello
      world
```

