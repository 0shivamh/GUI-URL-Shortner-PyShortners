from pyshorteners import Shortener
from pyshorteners import *
import tkinter as tk
from tkinter import *

frame=tk.Tk()
frame.title('URL Shortner') 
frame.geometry('600x300')
frame.configure(bg="#74B9FF")

title=Label(frame,text="URL Shortner",bg="#74B9FF",font="Helvetica")
title.place(x=230,y=50,width=120,height=30)

l1=Label(frame,text="URL:",bg="#74B9FF")
l1.place(x=30,y=120,width=50,height=25)

st=StringVar()
e=Entry(frame,textvariable=st)
e.place(x=100,y=120,width=400,height=30)

var = StringVar()
sh=Entry(frame,textvariable=var)
sh.place(x=100,y=200,width=400,height=30)

def Short():
    shortener = Shortener()
    url=e.get()
    var.set(shortener.tinyurl.short(url))
    st.set("")

b=Button(frame,text="Short",command=Short,bg='#badc57')
b.place(x=250,y=160,width=60,height=30)


frame.mainloop()
