### {}와 % 출력

#### 개요
{} 하고 %을 출력하기

```
print('{0}씨는 상위 {1}%안에 있는 사람입니다.'.format('한사람',10))
>>>한사람씨는 상위 10%안에 있는 사람입니다.

print('{{0}}씨는 상위 {{1}}%안에 있는 사람입니다.'.format('한사람',10))
>>>{0}씨는 상위 {1}%안에 있는 사람입니다.

print('{{{0}}}씨는 상위 {{{1}}}%안에 있는 사람입니다.'.format('한사람',10))
>>>{한사람}씨는 상위 {10}%안에 있는 사람입니다.

print('%s씨는 상위 %d%%안에 있는 사람입니다.'%('한사람',10))
>>>한사람씨는 상위 10%안에 있는 사람입니다.
```
