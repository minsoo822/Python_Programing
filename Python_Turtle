import random
import turtle as t

#화면 초기화
t.clearscreen()
t.setup(1200, 1200)
count = 1

#속도 설정
t.speed(30)

#사각형, 오각형, 육각형 만드는 함수
def pentagon(d):
    num = random.randint(3, 6)
    if num == 3 :
        angle = 360 / num
        for _ in range(num):
            t.forward(d)
            t.right(angle)    
    elif num == 4 :
        angle = 360 / num
        for _ in range(num):
            t.forward(d)
            t.right(angle)    
    elif num == 5:
        angle = 360 / num
        for _ in range(num):
            t.forward(d)
            t.right(angle)
    else :
        angle = 360 / num
        for _ in range(num):
            t.forward(d)
            t.right(angle)

def draw():
    global count

    # 색상 (파스텔 톤)
    r = random.randint(200, 255) / 255  # 빨강 색상값
    g = random.randint(200, 255) / 255  # 초록 색상값
    b = random.randint(200, 255) / 255  # 파랑 색상값

    #펜 굵기
    a = random.randint(1, 10)
    #d : 다각형의 한 변의 길이(랜덤)
    d = random.randint(20, 100)

    #터틀의 좌표(랜덤)
    x = random.randint(-200, 200)
    y = random.randint(-200, 200)

    t.penup()
    t.goto(x, y)
    t.pendown()
    t.pensize(a)
    t.color(r, g, b)

    if count%2==0:
        pentagon(d)
        count += 1
    else :
        t.begin_fill()
        pentagon(d)
        t.end_fill()
        count += 1

for i in range(1, 40):
    draw()
