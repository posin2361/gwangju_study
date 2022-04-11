선형큐 : 배열을 선형으로 사용하여 삽입을 계속하기 위해서는 주기적으로 요소들을 이동시켜야 한다. 하지만 문제점이 많아 사용되지 않음

원형큐 : 배열을 원형으로 사용하여 큐를 구현한다. 앞에서 삽입하고 뒤에서 삭제하는 방식이다.

front : 첫 번째 요소 하나 앞의 인덱스
rear : 마지막 요소의 인덱스

큐에서 주로 사용하는 연산
enqueue(q, e)  = 큐의 뒤에 요소를 추가한다.
dequeue(q) = 큐의 앞에 있는 요소를 반환한 다음 삭제한다.

/* 삽입 함수 */
void enqueue(QueueType *q, element item) {
    if(is_full(q))
    error("큐가 포화상태입니다");
    rear = (rear+1) % MAX_QUEUE_SIZE;
    queue[rear] = item;
}

/* 삭제 함수 */
element dequeue(QueueType *q) {
    if(is_empty(q))
    error("큐가 공백상태입니다.");
    front = (front+1) % MAX_QUEUE_SIZE;
    return queue[front];
}



덱큐 : 앞과 뒤에서 삽입과 삭제가 가능하다.

덱큐에서 주로 사용하는 연산
add_front(dq, e) = 덱의 앞에 요소를 추가한다.
add_rear(dq, e) = 덱의 뒤에 요소를 추가한다.
delete_front(dq) = 덱의 앞에 있는 요소를 반환한 다음 삭제한다
delete_rear(dq) = 덱의 뒤에 있는 요소를 반환한 다음 삭제한다.

/* 첫 번째의 삽입 함수 */
void add_front(DequeType *q, element val) {
    if)is_full(q))
    error("큐가 포화상태입니다.");
    data[front] = val;
    front = (front - 1 + MAX_QUEUE_SIZE) % MAX_QUEUE_SIZE;
}

/* 마지막의 추가 함수 */
void add_rear(DequeType *q, element item) {
    if (is_full(q))
    error("큐가 포화상태입니다");
    rear = (rear + 1) % MAX_QUEUE_SIZE;
    data[rear] = item;
}

/* 첫 번째의 삭제 함수 */
element delete_front(DequeType *q) {
    if (is_empty(q))
    error("큐가 공백상태입니다");
    front = (front + 1) % MAX_QUEUE_SIZE;
    return data[front];
}

/* 마지막의 삭제 함수 */
element delete_rear(DequeType *q) {
    int prev = rear;
    if (is_empty(q))
    error("큐가 공백상태입니다");
    rear = (rear - 1 + MAX_QUEUE_SIZE) % MAX_QUEUE_SIZE;
    return qdata[prev];
}
