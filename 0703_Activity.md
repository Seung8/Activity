## 7월 3일 엑티비티

### 피보나치 수 

```
def fibonacci(num):
    a, b = 0, 1
    # 피보나치 수열에 더해질 기본 값 정의
    for i in range(num):
    # for문으로 문제에 주어진 num의 범위만큼 순회
        a, b = b, a+b
        # 피보나치 수는 앞의 두 수를 더한 수가 다음 수가 됨
        # 여기서는 0, 1 = 1, 0+1 ... 식으로 순회하게 됨
        # 그러므로 a, b = b, a+b
    return a

# 아래는 테스트로 출력해 보기 위한 코드입니다.
print(fibonacci(3))
```

