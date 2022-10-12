# GUI_ATM_project



from tkinter import*

class Atm:
    def __init__(self,root):
        self.f=Frame(root,width=500,height=200,bg='teal')
        self.f.propagate(0)
        self.f.pack()

        self.b=Button(self.f,text='Submit')
        self.b.place(x=200,y=100)

        self.l=Label(self.f,text='Enter 4 digit pin')
        self.l.place(x=120,y=70)

        self.e=Entry(self.f,show='*')
        self.e.place(x=230,y=70)

        self.b2=Button(self.f,text='Open new window')
        self.b2.place(x=200,y=300)
        # self.e.bind("<Return>",self.reset)

    # def reset(self):
    #     l=Label(s)



root=Tk()
l=Atm(root)
root.mainloop()
