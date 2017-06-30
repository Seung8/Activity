## 6월 30일 엑티비티

### 행렬의 덧셈

```
def sumMatrix(A,B):
    answer = [[] for j in range(len(A))]  
    # 빈 값의 2차원 배열을 생성해서 answer에 지정
    for i in range(len(A)):
    # A의 길이만큼 순회하면서 
        for x in range(len(A[i])):
        # A의[i]의 길이만큼 한 번 더 순회한다
            answer[i].append(A[i][x] + B[i][x])
            # A, B의 각각 [i],[x]를 더해서
            # 미리 정의해둔 2차원 배열 answer에 append 한다
    return answer

	# 한 줄로 표현하면?
    # answer = [[c + d for c, d in zip(a, b)] for a, b in zip(A,B)]
    # zip을 이용하면 원하는 값을 다차원 배열로 만들어서 할당할 수 있음
    # 리스트의 길이만큼 반볼할 때는 for j in range(len(A))를 사용함
    # 빈 2차원 리스트에 값을 넣으려면 a[0].append(1)를 사용
    
    # return answer


# 아래는 테스트로 출력해 보기 위한 코드입니다.
print(sumMatrix([[1,2], [2,3]], [[3,4],[5,6]]))
```

