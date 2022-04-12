# Chapter3.Greedy

n = int(input())

# 큰 단위의 화폐부터 차례대로 확인
coin_types = [500, 100, 50, 10]
count = 0

for i in range(4):
  # 해당 화폐로 거슬러 줄 수 있는 동전의 개수 세기
  count += (n // coin_types[i])
  n = n % coin_types[i]

print(count)
