# Code Snippet in Python

파이썬을 사용할 때 자주 사용하는 구문 정리



## 1. 입출력

### 1.1. 입력

#### `sys.stdin.readline()` 의 활용

- 한 개의 정수를 입력받을 때

```python
import sys
a = int(sys.stdin.readline())
```

- 정해진 개수의 정수를 한 줄에 입력받을 때

```python
import sys
a,b,c = map(int,sys.stdin.readline().split())
```

​	`map()` 은 반복 가능한 객체(리스트 등)에 대해 각각의 요소들을 지정된 함수로 처리해주는 함수.

- 임의의 개수의 정수를 한 줄에 입력받아 리스트에 저장할 때

```python
import sys
data = list(map(int,sys.stdin.readline().split()))
```

​	`list()`는 자료형을 리스트형으로 변환해주는 함수. `map()`은 맵 객체를 만드므로, 리스트형으로 바꿔주기 위해서 `list()`로 처리

- 임의의 개수의 정수를 n줄 입력받아 2차원 리스트에 저장할 때

```python
import sys
data = []
n = int(sys.stdin.readline())
for i in range(n):
    data.append(list(map(int,sys.stdin.readline().split())))
```

이렇게 한다면 각 요소의 길이가 동일한 2차원 리스트도 만들 수 있고, 각각 길이가 다른 2차원 리스트도 입력 받을 수 있다.

- 문자열 n줄을 입력받아 리스트에 저장할 때

```python
import sys
n = int(sys.stdin.readline())
data = [sys.stdin.readline().strip() for i in range(n)]
```



### 1.2. 출력

#### 리스트에 있는 문자열을 하나의 문자열로 변환 :  `'구분자'.join(리스트)`

```python
li = ['a', 'b', 'c']
print("".join(li))		# 'abc' 출력
print("_".join(li))		# 'a_b_c' 출력
```



### 


