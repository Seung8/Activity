## 6월 2일 엑티비티

```
def sum_digit(number):
    '''number의 각 자릿수를 더해서 return하세요'''
    num = str(number)	
    # 매개변수 number를 문자열로 열거 후 num에 할당
    sum = 0
    # 각 자리수를 더할 임의의 변수 sum을 정의
    for i in range(len(num)):
        # num(number 문자열)의 길이만큼 순회
        sum += int(num[i])
        # num문자열 하나하나(i)를 int형으로 형변환하여 연산 후 sum에 할당
    return sum
	# 연산된 결과값 sum 리턴
print("결과 : {}".format(sum_digit(123)));
```

