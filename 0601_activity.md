## 6월 1일 오전 액티비티

### 최소값을 제거한 리스트 구하기

```
def rm_small(mylist):	
# mylist의 최소값을 제거한 값을 리턴하는 함수

    mylist.remove(min(mylist))	
    # mylist에서 remove한다 min(mylist)을
    
    return mylist	
    # 제거한 값을 리턴

my_list = [4, 3, 2, 1]
print("결과 {} ".format(rm_small(my_list)))
```

