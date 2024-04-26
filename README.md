from tkinter import *

window = Tk()
window.geometry('400x300')
window.title('Simple Calculator')
window.maxsize(400, 300)
window.minsize(400, 300)

# LABEL:
label = Label(text="plaese Input Your Numbers Below", fg='white', bg='black')
answer = Label(text="")
label.place(x=100, y=50)
answer.place(x=175, y=250)

# PLUS:


def add():
    x = int(input.get())
    y = int(input2.get())
    c = x + y
    answer.config(text=str(c))


j = Button(text='+', fg='white', bg='black', command=add, height=1, width=1)
j.place(x=200, y=200)

# MINUS:


def minus():
    x = int(input.get())
    y = int(input2.get())
    c = y - x
    answer.config(text=str(c))


m = Button(text='-', fg='white', bg='black', command=minus, height=1, width=1)
m.place(x=150, y=200)

# MULTIPLY:


def multiply():
    x = int(input.get())
    y = int(input2.get())
    c = x * y
    answer.config(text=str(c))


z = Button(text='X', fg='white', bg='black', command=multiply, height=1, width=1)
z.place(x=100, y=200)

# DEVIDE:


def devide():
    x = int(input.get())
    y = int(input2.get())
    c = y / x
    answer.config(text=str(c))


t = Button(text='÷', fg='white', bg='black', command=devide, height=1, width=1)
t.place(x=250, y=200)


# INPUT:
input = Entry(window)
input2 = Entry(window)
input2.place(x=125, y=100)
input.place(x=125, y=150)

window.mainloop()
