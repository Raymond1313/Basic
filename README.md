# Basic

#Integer

a = 1000 #양의 정수
print(a)

a = -7 #음의 정수
print(a)

a = 0 #0
print(a)


#Real Number

#양의 실수
a = 157.93
print(a)

#음의 실수
a = -1837.2
print(a)

#소수부가 0일 때 0을 생략
a = 5.  
print(a)

#정수부가 0일 때 0을 생략
a = -.7
print(a)

#10억의 지수 표현 방식
a = 1e9
print(a)

#725.5
a = 75.25e1
print(a)

#3.954
a = 3954e-3
print(a)

#2진수에서는 0.9를 정확히 표현할 수 없다!!!
a = 0.3 + 0.6
print(a)

if a == 0.9:
  print(True)
else:
  print(False)


#실수형 데이터를 비교할 때 소수점 다섯번째자리에서 반올림한 결과가 같으면 정답으로 인정!!
a = 0.3 + 0.6
print(round(a,4))

if round(a,4) == 0.9:
  print(True)
else:
  print(False)

#수 자료형의 연산

a = 7
b = 3

#나누기
print(a/b)

#나머지
print(a % b)

#몫
print(a//b)

#거듭제곱
a = 5
b = 3

print(a ** b)


#리스트 자료형

a = [1,2,3,4,5,6,7,8,9]
print(a)

#인덱스 4, 즉 다섯번째 원소에 접근
print(a[4])

#빈 리스트 선언 방법 1)
a = list()
print(a)

#빈 리스트 선언 방법 2)
a = []
print(a)

#크기가 N이고, 모든 값이 0인 1차원 리스트 초기화
n = 10
a = [0] * n
print(a)

#리스트의 인덱싱

a = [1,2,3,4,5,6,7,8,9]
#뒤에서 첫 번째 원소 출력
print(a[-1])

#뒤에서 세 번째 원소 출력
print(a[-3])

#네 번째 원소 값 변경
a[3] = 7
print(a)

# 리스트의 슬라이싱

a = [1,2,3,4,5,6,7,8,9]

#두 번째 원소부터 네 번째 원소까지
print(a[1:4])

#리스트 컴프리핸션 comprehension??

#0부터 19까지의 수 중에서 홀수만 포함하는 리스트
array = [i for i in range(20) if i % 2 == 1]

print(array)

#1부터 9까지의 수의 제곱 값을 포함하는 리스트
array = [i * i for i in range(1, 10)]
print(array)

# N x M 크기의 2차원 리스트 초기화
n = 3
m = 4
array = [[0] * m for _ in range(n)]
print(array)

summary = 0
for i in range(1,10):
  summary += i
print(summary)

for _ in range(5):
  print("Hello World")

  
#리스트 관련 기타 매서드

a = [1,4,3]
print("기본 리스트:",a)

#리스트에 원소 삽입
a.append(2)
print("삽입:",a)

#오름차순 정렬
a.sort()
print("오름차순 정렬:",a)

#내림차순 정렬
a.sort(reverse = True)
print("내림차순 정렬:",a)

#리스트 원소 뒤집기
a.reverse()
print("원소 뒤집기:",a)

#특정 인덱스에 데이터 추가
a.insert(2,3)
print("인덱스 2에 3 추가:",a)

#특정 값이 데이터 개수 세기
print("값이 3인 데이터 개수:",a.count(3))

#특정 값 데이터 삭제
a.remove(1)
print("값이 1인 데이터 삭제:",a)

a = [1,2,3,4,5,5,5]
remove_set = {3,5}

#remove_set에 포함되지 않은 값만을 저장
result = [i for i in a if i not in remove_set]
print(result)
