# tic-tac
from tkinter import *
win=Tk()
global valt
valt='0'
win.title('Tic Tac')
frame1=Frame(win)
frame2=Frame(win)
frame3=Frame(win)
frame4=Frame(win)
frame5=Frame(win)
frame6=Frame(win)
frame7=Frame(win)
frame8=Frame(win)
frame9=Frame(win)
frame1.grid()
frame2.grid()
frame3.grid()
frame4.grid()
frame5.grid()
frame6.grid()
frame7.grid()
frame8.grid()
frame9.grid()


def click(a):
    global valt
    if valt=='x':
        valt='0'
    else:
        valt='x'
    if a==1:
        button1['text']=valt
    elif a==2:
        button2['text']=valt
    elif a==3:
        button3['text']=valt
    elif a==4:
        button4['text']=valt
    elif a==5:
        button5['text']=valt
    elif a==6:
        button6['text']=valt
    elif a==7:
        button7['text']=valt
    elif a==8:
        button8['text']=valt
    elif a==9:
        
        button9['text']=valt
    
    vivek()
def reset():
    top=Toplevel(padx=50, pady=50)
    top.grid()
    message=Label(top,text='reset complete')
    button=Button(top,text='OK',command=top.destroy)

    message.grid(row=0,padx=5,pady=5)
    button.grid(row=1,ipadx=10,ipady=10,padx=5,pady=5)
    button1['text']=''
    button2['text']=''
    button3['text']=''
    button4['text']=''
    button5['text']=''
    button6['text']=''
    button7['text']=''
    button8['text']=''
    button9['text']=''
    
    message=Button()
    
    
button1=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(1))
button1.grid(row=0,column=0)
#button1.pack()
button2=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(2))
button2.grid(row=0,column=1)
#button2.pack()
button3=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(3))
button3.grid(row=0,column=2)
#button3.pack()
button4=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(4))
button4.grid(row=1,column=0)
#button4.pack()
button5=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(5))
button5.grid(row=1,column=1)
#button5.pack()
button6=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(6))
button6.grid(row=1,column=2)
#button6.pack()
button7=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(7))
button7.grid(row=2,column=0)
#button7.pack()
button8=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(8))
button8.grid(row=2,column=1)
#button8.pack()
button9=Button(frame1,bg='black',fg='white',width=8,height=3,font=('arial',12,'bold'),command=lambda :click(9))
button9.grid(row=2,column=2)
#button9.pack()
resetButton = Button (frame1, text = "Reset", font = ("Arial", 8, "bold"), relief = RAISED, bd=5, justify = CENTER, overrelief = GROOVE, activebackground = "green", activeforeground="blue", command = reset)
resetButton.grid(row = 5, column = 1,ipady = 8, ipadx = 12, pady = 5, sticky = NW)

def vivek():
    if button1['text']==button2['text']==button3['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button1['text']==button2['text']==button3['text']=='0':
            print('0 is winner')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
            
    elif button4['text']==button5['text']==button6['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button4['text']==button5['text']==button6['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
  
    elif button7['text']==button8['text']==button9['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button7['text']==button8['text']==button9['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''


    elif button1['text']==button4['text']==button7['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button1['text']==button4['text']==button7['text']=='0':
            print('0 is winner')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
            
    elif button2['text']==button5['text']==button8['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button2['text']==button5['text']==button8['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
  
    elif button3['text']==button6['text']==button9['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button3['text']==button6['text']==button9['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''






    elif button1['text']==button5['text']==button9['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button1['text']==button5['text']==button9['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
  
    elif button3['text']==button5['text']==button7['text']=='x':
            print('X winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
    elif button3['text']==button5['text']==button7['text']=='0':
            print('0 winner ')
            button1['text']=''
            button2['text']=''
            button3['text']=''
            button4['text']=''
            button5['text']=''
            button6['text']=''
            button7['text']=''
            button8['text']=''
            button9['text']=''
     
win.mainloop()


