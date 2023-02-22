# Turtle
import turtle

s = turtle.Screen ( )
t = turtle.Turtle ( ) 

s.bgcolor('#262626')
t.pencolor('#540d6e')
t.speed(100)
col = ('#DDA0DD', '#BA55D3', '#DB7093', '#C71585')

for n in range(10):
    for x in range(16):
        t.speed(x+200)
        for i in range(2):
            t.pensize(2)
            t.circle(80+n*20,90)
            t.lt(90)
        t.lt(45)
        t.pencolor(col[n%4])
s.exitonclick( )
