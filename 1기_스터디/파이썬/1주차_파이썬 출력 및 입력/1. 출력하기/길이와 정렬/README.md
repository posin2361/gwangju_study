###길이와 정렬

####개요
원하는 길이 만큼 원하는 정렬 통한 출력

{:길이}는 문자열(왼쪽 정렬), 숫자(오른쪽 정렬)
```
print('Python is [{:15}]'.format('good'))
>>>Python is [good           ]

print('Python is [{:<15}]'.format('good'))
>>>Python is [good           ]

print('Python is [{:>15}]'.format('good'))
>>>Python is [           good]

print('Python is [{:^15}]'.format('good'))
>>>Python is [     good      ]

print('Python is [{:15}]세'.format(22))
>>>Python is [           good]
```
