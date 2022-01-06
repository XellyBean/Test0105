# Test0105 with python


#1.


import json


path = "./bread2.json"

data = {}
data['breadType'] = []
data['breadType'].append({
    "breadType" : "cream",
    "recipe" : "",

    "flour" : 100,
    "water" : 100,
    "cream" : 200

})

data['breadType'].append({
    "breadType" : "sugar",
    "recipe" : "",
    
    "flour" : 100,
    "water" : 50,
    "cream" : 200

})

data['breadType'].append({
    "breadType" : "butter",
    "recipe" : "",

    "flour" : 100,
    "water" : 100,
    "cream" : 50

})

print(data)

with open(path, 'w') as outfile:
    json.dump(data, outfile, indent=4)



#2.

class add(int):
   def __call__(self, n):
      return add(self + n)


class subtract(int): 
   def __call__(self, n):
      return subtract(self - n)


#print(add(2)(3))
#print(subtract(1)(3))



#3.


def factorial_for(n):
    ret = 1
    for i in range(1, n+1):
        ret *= i
    return ret

#사용예시
#print(factorial_for(4))
#결과값 24



#4.

#만약 한 함수에서 너무 큰 지역 변수를 선언하거나 함수를 재귀적으로 무한정 호출하게 되면 Stack Overflow가 발생할 수 있습니다.
#Stack Overflow가 발생하면 컴파일러 옵션에서 Stack 영역의 크기를 늘리거나 또는 함수에서 사용하는 지역 변수의 크기를 줄이거나 아니면 지역 변수를 전역 변수로 바꾸어 해결할 수 있습니다.







#5.
