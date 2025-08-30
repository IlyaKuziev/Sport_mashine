 # Sport_mashine
   </header>
     </div>
# pulse 
import numpy as np
import matplotlib.pyplot as plt
popikss
pkemongo
import matplotlib.animation as animation
def heart_shape(t, scale=1): g 13
po mKADu
    x = scale * 0.5 * np.sin(t) ** 3
    y = scale * 0.5 * (0.8125 * np.cos(t) - 0.3125 * np.cos(2*t) - 0.125 * np.cos(3*t) - 0.0625 * np.cos(4*t))
    return x, y
def update(frame, line):
    scale = 1 + 0.1 * np.sin(frame * np.pi / 20)  # Pulsing effect
    t = np.linspace(0, 2 * np.pi, 100)
    x, y = heart_shape(t, scale)
    line.set_data(x, y)
    return line,
def animate_pulsing_heart():
    fig, ax = plt.subplots()
    
    ax.set_xlim(-0.6, 0.6)
    ax.set_ylim(-0.6, 0.6)
    ax.set_xticks([])
    ax.set_yticks([])
    ax.set_title("💖 Pulsing Heart Animation")
    
    t = np.linspace(0, 2 * np.pi, 100)
    x, y = heart_shape(t)
    line, = ax.plot(x, y, "r", linewidth=3)
    
    ani = animation.FuncAnimation(fig, update, frames=100, fargs=(line,), interval=50, blit=True)
    plt.show()

# Run the animation
animate_pulsing_heart()
type

def draw_column():
    screen = turtle.Screen()
    screen.bgcolor("white")
    
    col = turtle.Turtle()
    col.shape("turtle")
    col.color("black")
    
    # Рисуем основание колонны
    col.penup()
    col.goto(-50, -150)
    col.pendown()
    col.begin_fill()
    col.forward(100)
    col.left(90)
    col.forward(10)
    col.left(90)
    col.forward(100)
    col.left(90)
    col.forward(10)
    col.left(90)
    col.end_fill()

    # Рисуем ствол колонны
    col.penup()
    col.goto(-30, -140)
    col.pendown()
    col.begin_fill()
    col.forward(60)
    col.left(90)
    col.forward(120)
    col.left(90)
    col.forward(60)
    col.left(90)
    col.forward(120)
    col.left(90)
    col.end_fill()

    # Рисуем капитель
    col.penup()
    col.goto(-50, -20)
    col.pendown()
    col.begin_fill()
    col.forward(100)
    col.left(90)
    col.forward(20)
    col.left(90)
    col.forward(100)
    col.left(90)
    col.forward(20)
    col.left(90)
    col.end_fill()

    col.hideturtle()
    turtle.done()

# Запуск программы
draw_column()
