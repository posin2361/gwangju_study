선형큐 : 배열을 선형으로 사용하여 삽입을 계속하기 위해서는 주기적으로 요소들을 이동시켜야 한다. 하지만 문제점이 많아 사용되지 않음

원형큐 : 배열을 원형으로 사용하여 큐를 구현한다. 앞에서 삽입하고 뒤에서 삭제하는 방식이다.

front : 첫 번째 요소 하나 앞의 인덱스
rear : 마지막 요소의 인덱스

큐에서 주로 사용하는 연산
enqueue(q, e)  = 큐의 뒤에 요소를 추가한다.
dequeue(q) = 큐의 앞에 있는 요소를 반환한 다음 삭제한다.

![image](https://user-images.githubusercontent.com/103267689/163175095-b7eea8a1-8575-4e64-be41-68f747e07b60.png)


덱큐 : 앞과 뒤에서 삽입과 삭제가 가능하다.

덱큐에서 주로 사용하는 연산
add_front(dq, e) = 덱의 앞에 요소를 추가한다.
add_rear(dq, e) = 덱의 뒤에 요소를 추가한다.
delete_front(dq) = 덱의 앞에 있는 요소를 반환한 다음 삭제한다
delete_rear(dq) = 덱의 뒤에 있는 요소를 반환한 다음 삭제한다.

![image](https://user-images.githubusercontent.com/103267689/163175233-1e9a1a8f-3f1e-43b1-a767-acdc63a3a1f0.png)

![image](https://user-images.githubusercontent.com/103267689/163175397-5048cb73-f01a-47ed-9bf4-e77e0f7cceca.png)

![image](https://user-images.githubusercontent.com/103267689/163175433-665a48f1-a78a-4ab7-82a9-aba7329871e7.png)
