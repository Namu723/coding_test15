#약수의 개수와 덧셈

def solution(left, right):
    result = 0
    div_list = []
    for i in range(left, right+1):
        for j in range(1,i+1):
            if i % j == 0:
                div_list.append(j)
        if len(div_list) % 2 == 0:
            result += i
        else:
            result -= i
        div_list = []
    return result

#print(solution(13	,17))
#ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ


def solution(left, right):
    answer = 0
    for i in range(left,right+1):
        print(int(i**0.5),i**0.5)
        if int(i**0.5)==i**0.5:
            answer -= i
        else:
            answer += i
    return answer


