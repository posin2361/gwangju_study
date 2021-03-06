### 포인터이란?

#### 개요
데이터가 저장된 메모리의 시작 주소

#### 주소연산자
'&' 이라는 주소 연산자는 변수의 주소값을 반환하며 '&'기호는 앰퍼샌드라고 잀으며, 번지 연산자라고도 불린다.

#### 참조연산자
'*' 이라는 참조 연산자는 포인터에 가리키는 주소에 저장된 값을 반환한다.

```
int num01 = 1234;
double num02 = 3.14;
int* ptr_num01 = &num01;
double* ptr_num02 = &num02;

printf("포인터의 크기는 %d입니다.\n", sizeof(ptr_num01));
>>>포인터의 크기는 8입니다.

printf("포인터 ptr_num01이 가리키고 있는 주소값은 %#x입니다.\n", ptr_num01);
>>>포인터 ptr_num01이 가리키고 있는 주소값은 0x7c255e4입니다.

printf("포인터 ptr_num02가 가리키고 있는 주소값은 %#x입니다.\n", ptr_num02);
>>>포인터 ptr_num02가 가리키고 있는 주소값은 0x7c255e8입니다.

printf("포인터 ptr_num01이 가리키고 있는 주소에 저장된 값은 %d입니다.\n", *ptr_num01);
>>>포인터 ptr_num01이 가리키고 있는 주소에 저장된 값은 1234입니다.

printf("포인터 ptr_num02가 가리키고 있는 주소에 저장된 값은 %f입니다.\n", *ptr_num02);
>>>포인터 ptr_num02가 가리키고 있는 주소에 저장된 값은 3.140000입니다.
```
