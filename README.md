# 3-1
input_string = input("정수들을 입력하세요 (띄어쓰기로 구분, 엔터를 입력하면 종료): ")
input_list = input_string.split()

sum = 0
count = 0

for num in input_list:
    try:
        sum += int(num)
        count += 1
    except:
        break

if count > 0:
    average = sum / count
    print("입력한 정수들의 평균은", average, "입니다.")
else:
    print("입력된 정수가 없습니다.")
