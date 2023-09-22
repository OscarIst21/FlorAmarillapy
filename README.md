from turtle import *

bgcolor("gray")
speed(100)
h = 0
penup()
goto(0, -100)
pendown()
color("green")
begin_fill()
right(90)
fd(400)
left(90)
fd(20)
left(90)
fd(400)
left(90)
fd(20)
end_fill()
penup()
goto(0, 0)
pendown()
for i in range(16):
    for j in range(18):
        color("yellow")
        h += 0.005
        right(90)
        circle(150 - i * 6, 90)
        left(90)
        circle(150 - i * 6, 90)
        right(180)
        circle(40, 24)

for l in range(65):
    penup()
    goto(-65 + l , -18 )
    pendown()
    if l % 2 == 0:  # Usar == para comparar
        color("brown")
    else:
        color("black")
    begin_fill()
    circle(65-l+1)  # Ajustar el radio del centro
    penup()
 

goto(250, -250)
color("black")
write("Para ti<3 ", align="right", font=("Script MT Bold", 22, "normal"))
end_fill()
done()
