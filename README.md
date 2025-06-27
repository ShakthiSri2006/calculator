# calculator
# function of calculator
from tkinter import*
window=Tk()
def add():
    a=float(entry1.get())
    b=float(entry2.get())
    label.config(text=f"Result:{a+b}")
def sub():
    a=float(entry1.get())
    b=float(entry2.get())
    label.config(text=f"Result:{a-b}")
def mul():
    a=float(entry1.get())
    b=float(entry2.get())
    label.config(text=f"Result:{a*b}")
def div():
    a=float(entry1.get())
    b=float(entry2.get())
    label.config(text=f"Result:{a/b}")
window.title("Area")
label1=Label(window,text="number_1").pack()
entry1=Entry(window,font=20)
entry1.pack()
label2=Label(window,text="number_2").pack()
entry2=Entry(window,font=20)
entry2.pack()
button1=Button(window,text="add",command=add,font=50).pack()
button2=Button(window,text="sub",command=sub,font=50).pack()
button3=Button(window,text="mul",command=mul,font=50).pack()
button4=Button(window,text="div",command=div,font=50).pack()
label=Label(window,text="Result",font=("poppins",50))
label.pack()
window.mainloop()

