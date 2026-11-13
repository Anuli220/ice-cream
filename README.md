# ice-cream

import turtle

screen = turtle.Screen()
screen.bgcolor('lightblue')

pen = turtle.Turtle()
pen.speed(0)
pen.hideturtle()

def draw_circle(colour, x, y, radius):
  pen.penup()
  pen.goto(x, y)
  pen.pendown()
  pen.color(colour)
  pen.begin_fill()
  pen.circle(radius)
  pen.end_fill()
  
def draw_triangle(colour, x1, y1, x2, y2, x3, y3):
  pen.penup()
  pen.goto(x1, y1)
  pen.pendown()
  pen.color(colour)
  pen.begin_fill()
  pen.goto(x2, y2)
  pen.goto(x3, y3)
  pen.goto(x1, y1)
  pen.end_fill()
  
draw_triangle('brown', -80, 40, 0, -150, 80, 40)
draw_circle('pink', -40, -10, 60)
draw_circle('yellow', 0, 40, 60)
draw_circle('lightgreen', 40, -10, 60)
draw_circle('red', 0, 150, 12)
