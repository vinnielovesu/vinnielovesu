import math
from turtle import*
def hearta(k):
return 15 * math.sin(k) ** 3
def heartb(k):
return 12 * math.cos(k) - 5 * math.cos(2 * k) -
2 * math.cos(3 * k) - math.cos(4 * k)
speed(1200)
bgcolor("black")
color("yellow")
begin_fill()
for i in range(600):
x=hearta(i * 2 * math.pi / 600) * 10
y=heartb(i * 2 * math.pi / 600) * 10
goto(x,y)
end_fill()
done()
