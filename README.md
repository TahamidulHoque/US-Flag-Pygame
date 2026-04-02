# US-Flag-Turtle Graphics
#programid: Us falg creation
#author: Tahamidul Hoque
#purpose: TO be able to draw the us flag using turtle drawing

from turtle import *
#initialize variable
hoist = 0


#defining function for the first star
def polystar(length):
  for index in range(5):
    forward(length * .023)
    right(-72)
    forward(length * .023)
    right(144)


speed('fastest')

hoist = int(input('Enter the hoist value: '))
# the base for the flag (the two rectangles)
for index in range(2):
  pd()
  forward(hoist * 1.9)
  right(90)
  forward(hoist)
  right(90)
#The stripes
for index in range(7):
  fillcolor("red")
  begin_fill()
  forward(hoist * 1.9)
  right(90)
  forward(hoist * .0769)
  right(90)
  pu()
  forward(hoist * 1.9)
  left(90)
  forward(hoist * .0769)
  left(90)
  end_fill()
  
#the blue union with the mini box
pu()
goto(0, 0)
fillcolor("blue")
begin_fill()
pd()
for index in range(2):
  forward(hoist * .76)
  right(90)
  forward(hoist * .5385)
  right(90)
end_fill()

x=0
#6 stars with 5 columns
for six__star in range(5):
  pu()
  fillcolor('white')
  begin_fill()
  x = x + hoist * .126
  y = -hoist * .063/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()

for six__star in range(5):
  fillcolor('white')
  begin_fill()
  pu()
  forward(hoist * .063)
  x = x + -hoist * .126
  y = -hoist * .063/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()

for six__star in range(5):
  pu()
  forward(hoist * .063)
  x = x + hoist * .126
  y = (-hoist *.063)*3/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

for six__star in range(5):
  fillcolor('white')
  begin_fill()
  pu()
  forward(hoist * .063)
  x = x + -hoist * .126
  y = (-hoist *.063)*3/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()



for six__star in range(5):
  pu()
  forward(hoist * .063)
  x = x + hoist * .126
  y = (-hoist *.063)*5/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()
  
for six__star in range(5):
  fillcolor('white')
  begin_fill()
  pu()
  forward(hoist * .063)
  x = x + -hoist * .126
  y = (-hoist *.063)*5/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()



for six__star in range(5):
  pu()
  forward(hoist * .063)
  x = x + hoist * .126
  y = (-hoist *.063)*7/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

  
for six__star in range(5):
  fillcolor('white')
  begin_fill()
  pu()
  forward(hoist * .063)
  x = x + -hoist * .126
  y = (-hoist *.063)*7/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()




for six__star in range(5):
  pu()
  forward(hoist * .063)
  x = x + hoist * .126
  y = (-hoist *.063)*9/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

for six__star in range(5):
  fillcolor('white')
  begin_fill()
  pu()
  forward(hoist * .063)
  x = x + -hoist * .126
  y = (-hoist *.063)*9/1.15
  goto(x, y)
  pd()
  polystar(hoist)
  end_fill()



#five star in between and 4 columns 
for five_star in range(1):
  pu()
  x = x + hoist *.063
  y = (-hoist * .063)*2/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

for five__star in range(4):
  pu()
  x = x + hoist *.063*2
  y = (-hoist * .063)*2/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()



for five__star in range(4):
  pu()
  setheading(0)
  x = x + -hoist *.126
  y = (-hoist * .063)*4/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()
  
for five__star in range(4):

  pu()
  x = x + hoist *.126
  y = (-hoist * .063)*4/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

for five__star in range(4):
  pu()
  setheading(0)
  x = x + -hoist *.126
  y = (-hoist * .063)*6/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

for five__star in range(4):
  pu()
  x = x + hoist *.126
  y = (-hoist * .063)*6/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()



for five__star in range(4):
  pu()
  setheading(0)
  x = x + -hoist *.126
  y = (-hoist * .063)*8/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()
  
for five__star in range(4):
  pu()
  x = x + hoist *.126
  y = (-hoist * .063)*8/1.15
  goto(x, y)
  fillcolor('white')
  begin_fill()
  pd()
  polystar(hoist)
  end_fill()

done()
