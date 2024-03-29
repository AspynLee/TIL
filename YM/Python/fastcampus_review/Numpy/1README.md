# 패스트 캠퍼스 강의 복습 및 클론코딩 
## Numpy
## 개념 정리 및 클론코딩

## Numpy 모듈
수학적 연산, 수치적연산에 최적화된 모듈
이 자체만으로도 많이 쓰이지만, 
여러가지 머신러닝 라이브러리에 깔고 가는 모드이다.

성능: 파이썬 리스트보다 빠름
메모리 사이즈: 파이썬 리스트보다 적은 메모리 사용
더 많은 데이터를 한꺼번에 로딩이 가능하다.
빌트인 함수: 선형대수, 통계관련 여러 함수 내장
(파이썬의 리스트는 범용적인 container이기 때문에, 단순히  아이템 추가하고 제거하고 가져오는 것에 치중했다면,
넘파이는 수치적 최적화된 연산 라이브러리 이기때문에, 
그 데이터의 어떤 선형대수적인 연산이나, 통계적인 연산을 적용하는 과정임
아주 풍부한 빌트인 함수들이 내정되어 있어서 쉽게 연산을 적용할 수 있음.)


## ndarray
numpy에서 사용되는 다차원 리스트를 표현할 때 사용되는 데이터 타입임.

기본 타입이 있다. 
N dimension array 
다차원 배열 표현
파이썬 내에도 리스트롤 통해서 표현할 수 있지만, 성능적으로 훨씬 빠르기 때문에 사용 한다.

왜 빠를까?
C언어로 구현되어 있음. 
생성 당시에, 생성되는 모든 원소들이 연속적인 메모리(물리적)에 잡히게 됨. 
이 어레이를 순회하거나, 연산을 반복적으로 적용할 때 훨씬 빠르게  적용할 수 있다.

ndarray
연속된 메모리
Vectorization 사용 함.

python list
연속되지 않은 메모리, 명시적인 loop 사용 함.


```python
print("파이썬코드입니다")
```

### 01. numpy 모듈과 ndarray 이해하기

```
import numpy as np
import matplotlib.pyplot as plt
```
```
x = np.array([1, 2, 3])
y = np.array([2, 4, 6])

print(x)
print(y)

plt.plot(x, y)

```

함수 이해와 이용 및 활용하기

### 02. ndarray data 생성_numpy 모듈 함수
### 03. ndarray 데이터 생성하기(random 서브 모듈 함수 이용)
### 04. ndarray indexing _ slicing 
### 05. ndarray 데이터 형태 바꾸기 (reshaping, flatten 등 함수 이용)
### 06. ndarray 기본 함수 사용하기
### 07. axis(축) 이해 및 axis를 파라미터로 갖는 함수 활용하기
### 08. broadcasting 이해 및 활용하기
### 09. Boolean indexing으로 조건에 맞는 데이터 선택하기
### 10. linalg 서브모듈 사용하여 선형대수 연산하기
### 11. ndarray 데이터를 이용하여 다양한 그래프 표현하기
### 12. numpy 연습문제 풀이
