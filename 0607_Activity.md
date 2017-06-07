## 6월 7일 엑티비티

### 수박수박수박수박수?

```
def water_melon(n):
    # 함수를 완성하세요.
    s = "수박" * n
    # 수박 문자열이 n만큼 더해짐(수박수박수박수박...)
    return s[:n]
	# 리턴할 때 n만큼 늘어난 수박 문자열을 n만큼 슬라이싱해서 리턴함


# 실행을 위한 테스트코드입니다.
print("n이 3인 경우: " + water_melon(3));
print("n이 4인 경우: " + water_melon(4));

```




### 서울에서 김서방 찾기

```
def findKim(seoul):
    # 함수를 완성하세요

    return "김서방은 {}에 있다".format(seoul.index("Kim"))
    # format 함수에서 바로 조건이 "Kim"인 인덱스 번호 리턴


# 실행을 위한 테스트코드입니다.
print(findKim(["Queen", "Tod", "Kim"]))
```



