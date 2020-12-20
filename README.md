# new_bie.py
import turtle


turtle.bgcolor('skyblue')
x = 0
def move(distance):
	turtle.penup()
	turtle.goto(-distance/2,distance/2)
	turtle.pendown()
	turtle.hideturtle()

def ran_turtle(distance):
	turtle.forward(distance)
	turtle.right(90)


turtle.speed(10000)
move(300)
while True:
	x+=2
	ran_turtle(300-x)
	if (300-x)<0:
		break


turtle.mainloop()
