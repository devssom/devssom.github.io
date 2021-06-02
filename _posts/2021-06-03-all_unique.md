# All Unique 문제
## 리스트의 모든 값이 다 중복없이 고유한 값인가요?

- 문제 : 리스트의 값이 고유한 값이면, True를 반환하고, 그렇지 않으면 False를 반환하세요.
- 참고 : 리스트에 set() 함수를 사용하면, 중복되는 값을 제거할 수 있어요.
         그리고 len() 함수로 리스트 각각의 길이를 재서 비교합니다.


```python
def all_unique(lst):
    return len(lst) == len(set(lst))
```


```python
x = [1, 2, 3, 4, 5, 6]
y = [1, 2, 2, 3, 4, 5]
all_unique(x)
```




    True



리스트 x의 경우, 중복되는 값들이 없기 때문에 len(x)도 6개, len(set(x))도 6개로 갯수가 동일. 그래서 True가 출력됨.


```python
all_unique(y)
```




    False



리스트 y는 2가 중복되기 때문에, set()함수로 중복된 2가 제거되서 len(set(y))는 5개. 그래서 False가 출력됨.
