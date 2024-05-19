from tkinter import *

window = Tk()
window.geometry('600x400')
window.title('Simple Calculator')
window.maxsize(400, 400)
window.minsize(400, 400)

# LABEL:
label = Label(text="Plaese Input Your Numbers Below", fg='white', bg='black')
answer = Label(text="", font=("Arial", 20))
label.place(x=100, y=50)
answer.place(x=175, y=340)

# X & Y:
x_label = Label(text="First Number:", fg='white', bg='black', font=("Arial", 8))
y_label = Label(text="Second Number:", fg='white', bg='black', font=("Arial", 8))
x_label.place(x=50, y=100)
y_label.place(x=35, y=150)


# PLUS:


def add():
    x = int(input.get())
    y = int(input2.get())
    c = x + y
    answer.config(text=str(c))


j = Button(text='ADD', fg='white', bg='black', command=add, height=1, width=8)
j.place(x=210, y=200)

# MINUS:
def minus():
    x = int(input.get())
    y = int(input2.get())
    c = y - x
    answer.config(text=str(c))


m = Button(text='MINUS', fg='white', bg='black', command=minus, height=1, width=8)
m.place(x=130, y=200)


# MULTIPLY:
def multiply():
    x = int(input.get())
    y = int(input2.get())
    c = x * y
    answer.config(text=str(c))


z = Button(text='MULTIPLE', fg='white', bg='black', command=multiply, height=1, width=8)
z.place(x=50, y=200)

# DEVIDE:
def devide():
    x = int(input.get())
    y = int(input2.get())
    c = y / x
    answer.config(text=str(c))


t = Button(text='DIVISION', fg='white', bg='black', command=devide, height=1, width=8)
t.place(x=290, y=200)


# POWER:
def power():
    x = int(input.get())
    y = int(input2.get())
    c = x ** y
    answer.config(text=str(c))


j = Button(text='Power', fg='white', bg='black', command=power, height=1, width=8)
j.place(x=50, y=235)


# ONE DEVIDED BY X:
def odx():
    x = int(input2.get())
    c = 1 / x
    answer.config(text=str(c))


j = Button(text='1/X', fg='white', bg='black', command=odx, height=1, width=8)
j.place(x=130, y=235)


# PERCENTAGE:
def percentage():
    x = int(input.get())
    y = int(input2.get())
    c = y * 100 / x
    answer.config(text=str(c))


j = Button(text='PERCENT', fg='white', bg='black', command=percentage, height=1, width=8)
j.place(x=210, y=235)

# POWER OF 10:
def pot():
    y = int(input2.get())
    c = 10 ** y
    answer.config(text=str(c))


j = Button(text='P O 10', fg='white', bg='black', command=pot, height=1, width=8)
j.place(x=290, y=235)


# INPUT:
input = Entry(window)
input2 = Entry(window)
input2.place(x=125, y=100)
input.place(x=125, y=150)

window.mainloop()
