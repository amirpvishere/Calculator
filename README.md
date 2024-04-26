from tkinter import *

window = Tk()
window.geometry('400x300')
window.title('Simple Calculator')
window.maxsize(400, 300)
window.minsize(400, 300)

# LABEL:
label = Label(text="Plaese Enter Your Numbers Below", fg='white', bg='black')
javab = Label(text="")
label.place(x=100, y=50)
javab.place(x=175, y=250)

# Plus:


def add():
    x = int(input.get())
    y = int(input2.get())
    c = x + y
    javab.config(text=str(c))


j = Button(text='+', fg='white', bg='black', command=add, height=1, width=1)
j.place(x=200, y=200)

# Minus:


def minus():
    x = int(input.get())
    y = int(input2.get())
    c = y - x
    javab.config(text=str(c))


m = Button(text='-', fg='white', bg='black', command=minus, height=1, width=1)
m.place(x=150, y=200)

# Multiply:


def times():
    x = int(input.get())
    y = int(input2.get())
    c = x * y
    javab.config(text=str(c))


z = Button(text='X', fg='white', bg='black', command=times, height=1, width=1)
z.place(x=100, y=200)

# Devide:


def devide():
    x = int(input.get())
    y = int(input2.get())
    c = y / x
    javab.config(text=str(c))


t = Button(text='÷', fg='white', bg='black', command=devide, height=1, width=1)
t.place(x=250, y=200)


# INPUT:
input = Entry(window)
input2 = Entry(window)
input2.place(x=125, y=100)
input.place(x=125, y=150)

window.mainloop()
