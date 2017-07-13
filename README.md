# xsdjkbhvg-fchjgtrfnhjvc
import turtle
turtle.bgcolor("blue")
turtle.pencolor("black")
polygons={"triangle":3,"quadrilateral":4,"pentagon":5,"hexagon":6,"septagon":7,"octagon":8,"nonagon":9,"decagon":10}
def polygon(sides,length):
    i = 1
    polygon=sides
    polygons={"triangle": 3, "quadrilateral": 4, "pentagon": 5, "hexagon": 6, "septagon": 7, "octagon": 8,"nonagon": 9, "decagon": 10}
    indx=polygons[polygon]
    while i<indx or i==indx:
        turtle.fd(length)
        turtle.right(360/indx)
        i=i+1
def draw_rectangle(length,width,x,y):
    turtle.up()
    turtle.goto(x-(length/2),y+(width/2))
    turtle.down()
    turtle.goto(x+(length/2),y+(width/2))
    turtle.goto(x+(length/2),y-(width/2))
    turtle.goto(x-(length/2),y-(width/2))
    turtle.goto(x-(length/2),y+(width/2))
"""triangle=polygons["triangle"]
quadrilateral=polygons["quadrilateral"]
pentagon=polygons["pentagon"]
hexagon=polygons["hexagon"]
septagon=polygons["septagon"]
octagon=polygons["octagon"]
nonagon=polygons["nonagon"]
decagon=polygons["decagon"]"""
"""draw_rectangle(500,430,0,15)"""
inputshape=raw_input("type in a shape that is either a triangle, a quadrilateral, a pentagon, a hexagon, a septagon, a octagon, a nonagon, a decagon")
inputshape=print()
polygon(inputshape,100)
turtle.exitonclick()

