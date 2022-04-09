루프문 사용시 자주 사용되는 함수
===

    이 문서는 루프문에서 자주 사용되는 함수 

> 1.[range](#range) #range 범위
>  
> 2.[len](#len) #length 길이
>
>3.[reversed](#reversed) #reversed 역순 

### range() 

    파이썬 에서 range 함수는 자주 사용되는 함수중 하나다. 연속된 숫자(정수)를 
    반환 하는 range 함수에대해 간략하게 설명한다.

    기본 :
    
    range(stop)
    range(n) = 0~ n-1 만큼의 '정수'  range 클래스를 반환(실제사용은 list형처럼 사용)
    
```python
#range() #1
test = list(range(5)) # 기본형 

print(test)

>>> [0,1,2,3,4]
```
    
    인자를 두개 받는 경우 :
    
    range(start,stop)
    range(n, m) = n~m-1 만큼의 '정수' range 클래스를 반환 

```python
#range() #2
test = list(range(2,5)) # 인자를 두개 받는경우 
print(test)
>>>[2, 3, 4]

```

    인자를 세개 받는 경우:
 
    range(start, stop , step):
    range(n,m,x): n ~ x 까지 정수 를 n 부터 x 만큼 이동하면서 m까지출력

```python
    #range() #3
    test= list(range(1,5,2))
    print(test)
    >>>[1,3]
    #[1,2x,3,4x] => 2와 4는 출력되지않음.
```

    감소식으로 표현 : 
    range(start, stop, step):
    range(n,m,x): n ~ x 까지 정수 를 n 부터 x 만큼 이동하면서 m까지출력
    * range 값 설정시 n > m 으로 준 이후 x에 음수를 넣어 사용한다.

```python
    #range() #4
    test = list(range(10,1,-1)) # m >n > x
    print(test)
    >>>[10, 9, 8, 7, 6, 5, 4, 3, 2]
```


### len()
    
    파이썬의 len 함수는 타 언어에서의 length와 같다고 생각하면 이해하기 편하다.
    len(집합, 배열등 변수) => 함수인자의 크기를 반환한다.

```python
    #len() #1
    test = [1,2,3,4]
    print(len(test))
    >>>4 #test 리스트형의 크기인 4를 반환 

```
    
     String 형에서도 사용 가능하다. 이 경우 단어의 길이(크기)를 반환한다.

```python
    
    #len() #2
    test = "test"
    print(len(test))
   
    >>> 4 #test 문자열 길이인 4를 반환

```

### reversed()

    파이썬의 reversed(list) 함수는 인자로 들어온 list 형을 뒤집어서 반환한다.

```python
    #reversed()
     
    test = [1,2,3,4]
    test = reversed(test)
    for i in test :
        print(i , end=" ")
 
    >>> 4 3 2 1  
```
