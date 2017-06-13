## 6월 13일 엑티비티 

### 문자열 다루기 기본

```
def alpha_string46(s):
    #함수를 완성하세요
    return s.isdigit() and len(s) in [4,6]
	# isdigit은 자릿수 판별 함수 (숫자면 True, 아니면 False)
    # and 연산은 조건(s.isdigit()) and 대상(len(s))가 참이면 연산, 아니면 종료
    # s(len(s))가 in[4,6](len(s)가 4거나 6이면) 
    #isdigit()(숫자)이면 True 리턴, 아니면 False리턴 

# 아래는 테스트로 출력해 보기 위한 코드입니다.
print( alpha_string46("a234") )
print( alpha_string46("1234") )
```

### 문자열 내  p와 y의 개수

```
def numPY(s):
    return s.lower().count('p') == s.lower().count('y')
	# lower()는 대문자를 소문자로 바꿔주는 내장함수
    # count()는 ()안의 값의 개수를 반환하는 함수
    # s의 p(lower로 대문자도 소문자로 바꿔줌)의 개수(count)가 
    # s의 y(lower로 대문자도 소문자로 바꿔줌)의 개수(count)와 같으면
    # return True 아니면 False



# 아래는 테스트로 출력해 보기 위한 코드입니다.
print( numPY("pPoooyY") )
print( numPY("Pyy") )
```

- 밑의 방식으로도 가능하나 대문자가 포함된 경우 값이 다르게 나옴

```
def numPY(s):
	return s.count('p') == s.count('y')
```


