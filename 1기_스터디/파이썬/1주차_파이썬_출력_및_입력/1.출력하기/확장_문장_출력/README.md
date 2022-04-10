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
* 8진수로 출력되며 숫자 156(8진수)에 아스키코드 값은 n 이다.
```
print('\156')//
>>>n
```
print 16진수 사용한다면?
* \x 통해서 16진수 값 6E을 출력하게 되면 6E는 아스키코드 값이 n 으로 n이 출력된다.
```
print("\x6E")
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

