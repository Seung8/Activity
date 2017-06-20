## 6월 20일 엑티비티

### 문자열 내 마음대로 정렬하기

```
from operator import itemgetter
def strange_sort(strings, n):
    '''strings의 문자열들을 n번째 글자를 기준으로 정렬해서 return하세요'''
    return sorted(strings, key=itemgetter(n))
    # sorted는 입력값을 정렬한 후 출력하는 함수
    # 리스트는 key를 쓸 수 없어서 튜플을 사용(key 순으로 sorted)
    # itemgetter함수로 키 값의 n번째 값을 뽑아서 키에게 넘겨줌
    
    # sorted() - ()값을 정렬 후 반환
    # 리스트 key값 정렬(튜플 이용) - key(itemgetter값을 전달 후)로 sorted
    # itemgetter(n) - n번째 아이템 반환
    
# 아래는 테스트로 출력해 보기 위한 코드입니다.
print( strange_sort(["sun", "bed", "car"], 1) )
```





