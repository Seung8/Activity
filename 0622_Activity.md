## 6월 22일 엑티비티

### 딕셔너리 정렬

```
from operator import itemgetter
def sort_dictionary(dic):
    '''입력받은 dic의 각 키와 값을 튜플로 만든 다음, 키 값을 기준으로 정렬해서 리스트에 넣으세요. 그 리스트를 return하면 됩니다.'''
    return sorted(dic.items(), key=itemgetter(0))
	# sorted는 정렬해서 반환해주는 함수
    # items 함수는 key와 value 값을 튜플로 묶은 값을 반환
    # itemgetter는 operator에 정의되어있는 내장함수로
    # key=itemgetter()시에 ()안의 값이 0 이면 키(key)를 기준으로,
    # key=itemgetter()안의 값이 1이면 값(value)을 기준으로 정렬이 가능함
    # 정렬 후 반환한다(dic의 키,벨류(dic.items()로 dic의 키,값의 튜플로 묶음, 
    # 키를 기준(key=itemgetter(0))으로)
    

# 아래는 테스트로 출력해 보기 위한 코드입니다.
print( sort_dictionary( {"김철수":78, "이하나":97, "정진원":88} ))
```