## my work in python
```python
from tkinter import *
import random
from math import*
from chemlib import*


def RandomEmojiAscii(count):
    d=0
    a=""
    while d<count:
        d+=1
        j=["♦","☆","△","✉︎","✿","♥","♫","☢"]
        g=random.randint(0,len(j)-1)
        a+=j[g]+" "
    return a
print ("    ____________________________________________")
print (f"   |  {RandomEmojiAscii(1)}  |Вас приветствует калькулятор 0.2|      \\")
print(f"   |  {RandomEmojiAscii(1)}  |выберите вид калькулятора:|            /\n"
      f"   |  {RandomEmojiAscii(1)}  |1 - системы счисления     ( () )      /\n"
      f"   |  {RandomEmojiAscii(1)}  |2 - обычный                          /\n"
      f"   |  {RandomEmojiAscii(1)}  |3 - химический    |____________|____/")
userVariant=input(f"   |      |    {RandomEmojiAscii(1)}   выбор: ")
def RandomEmoji(count):
    d=0
    a=""
    while d<count:
        d+=1
        j=["🤜 ","😀 ","😏 ","😧 ","🤖 ","👾 ","☠️ ","🧠 ","👨‍⚕️ ","👩 ","👨‍🍳 ","👩‍✈️ ","👨‍🚒 ","👨‍🎨 ","👻 ","😄","😁",'🫣','🥹','👀'
           ,'👩‍🦲','🦷','👍','🧑‍🦱','👩‍🦳','🤷','🤌','🙆‍♂️','👲','❣️','🤷‍♂️','👩‍❤️‍💋‍👨','🛌','🤎','🕺','🧑‍🦳','👱‍♂️','🧑','😱','🥸'
           ,'😡','👨‍🦲','🙆‍♀️','👲','🤟','🙉','🥺','👋','🦴','🧑‍🦳','🧏‍♂️','🛌','🙍','🙆','👲','🦗','🐞','🪲','🪿'
           ,'🦋','🦪','🍲','🫛','🍋‍🟩','🫗','🍿','🥨','🥔','🥩','🍜','🍫','🍦','👨‍🎓','🎳','🥊','🏏','🎇','🎱','🧑‍💻','🧟‍♂️','🏄‍♀️']
        g=random.randint(0,len(j)-1)
        a+=j[g]+" "
    return a
def UV(userVariant):
    if  userVariant=="1":
        print("   \\  выберите функцию:                /\n"
        "    \\ 1 - перевод в двоичную          /\n"
        "     \\2 - перевод в восьмиричную     /\n"
        "     /3 - перевод в шестнадцатеричную\\")
        userVariantInCode=(input("функция: "))
        if userVariantInCode=="1" or userVariantInCode=="2" or userVariantInCode=="3":
                print ("|примечание! Вы можете ввести несколько чисел в одну строку ")
                userInput=[int(x) for x in input("|введите чис -ло -ла: ").split()]
                for i in range(len(userInput)):
                    if userVariantInCode=="1":
                        userInput[i]=bin(userInput[i])[2:]
                        print (f"|Число в 2-ичной системе счисления {userInput[i]}{RandomEmoji(1)}")
                    elif userVariantInCode=="2":
                        userInput[i]=oct(userInput[i])[2:]
                        print (f"|Число в 8-ричной системе счисления {userInput[i]}{RandomEmoji(1)}")
                    elif userVariantInCode=="3":
                        userInput[i]=hex(userInput[i])[2:]
                        print (f"|Число в 16-тиричной системе счисления {userInput[i]}{RandomEmoji(1)}")
        elif userVariantInCode!="1" or userVariantInCode!="2" or userVariantInCode!="3":
                print ("ERROR (неверная операция Bip-Bop)\n"
                "     \\_/\n"
                "     (* *)\n"
                "    __)#(__\n"
            "   ( )...( )(_)\n"
            "   || |_| ||//\n"
            ">==() | | ()/\n"
                "    _(___)_\n"
            "   [-]   [-]")  
    elif userVariant=="2":
        print ("   |примечание! Вы можете ввести только одно число в одну строку!")
        userVariantCalculateOne=int(input("   |введите 1 число: "))
        userVariantCalculateTwo=int(input("   |введите 2 число: "))
        userVariantCalculate=input("   |введите действие: ")
        if userVariantCalculate=="/" or userVariantCalculate=="//" or userVariantCalculate=="*" or userVariantCalculate=="**" or userVariantCalculate=="-" or userVariantCalculate=="+":
            def calculate(userVariantCalculate):
                    if userVariantCalculate=="/" or userVariantCalculate=="//":
                        if userVariantCalculateOne==0 or userVariantCalculateTwo==0:
                            return "   |на 0 делить нельзя"
                        elif userVariantCalculateOne!=0 or userVariantCalculateTwo!=0:
                            userVariantCalculate=userVariantCalculateOne//userVariantCalculateTwo
                            return f"   |Ответ {userVariantCalculate}{RandomEmoji(1)}"
                    elif userVariantCalculate=="+":
                        userVariantCalculate=userVariantCalculateOne+userVariantCalculateTwo
                        return f"   |Ответ {userVariantCalculate}{RandomEmoji(1)}"
                    elif userVariantCalculate=="-":
                        userVariantCalculate=userVariantCalculateOne-userVariantCalculateTwo
                        return f"   |Ответ {userVariantCalculate}{RandomEmoji(1)}"
                    elif userVariantCalculate=="*":
                        userVariantCalculate=userVariantCalculateOne*userVariantCalculateTwo
                        return f"   |Ответ {userVariantCalculate}{RandomEmoji(1)}"
                    elif userVariantCalculate=="**":
                        userVariantCalculate=userVariantCalculateOne**userVariantCalculateTwo
                        return f"   |Ответ {userVariantCalculate}{RandomEmoji(1)}"
            print(calculate(userVariantCalculate))
        else:
            print ("ERROR (неверная операция Bip-Bop)\n"
        "     \\_/\n"
        "     (* *)\n"
        "    __)#(__\n"
    "   ( )...( )(_)\n"
    "   || |_| ||//\n"
    ">==() | | ()/\n"
        "    _(___)_\n"
    "   [-]   [-]")
    elif userVariant=="3":
        print ("   |Вы попали в химический калькулятор! Его функци:\n"
        "   |1 Подсчет молекулярной массы\n"
        "   |2 Рассчитать массовую долю")
        userVariantCheam=input("   |введите цифру желаемой функции: ")
        def UVHVariant(userVariantCheam):
            if userVariantCheam=="1":
                userVariantCheam=Compound(input("   |введите химические вещества: "))
                return ("   |Ответ "+'%.0f' % userVariantCheam.molar_mass()+RandomEmoji(1))
            elif userVariantCheam=="2":
                userVariantCheam=Compound(input("   |введите формулу: "))
                userVariantCheam2=input("   |чью массовую долю мы рассчитываем? -введите элемент:  ")
                return ("   |Ответ "+'%.0f' % userVariantCheam.percentage_by_mass(userVariantCheam2)+"%"+RandomEmoji(1))
        print(UVHVariant(userVariantCheam))
    elif userVariant!="1" or userVariant!="2" or userVariant!="3":
        print ("ERROR (неверная операция Bip-Bop)\n"
        "     \\_/\n"
        "     (* *)\n"
        "    __)#(__\n"
    "   ( )...( )(_)\n"
    "   || |_| ||//\n"
    ">==() | | ()/\n"
        "    _(___)_\n"
    "   [-]   [-]")
UV(userVariant)

window=Tk()
window.title("Калькулятор 0.3 by Artemii Polikarpov")
window.geometry("400x300+900+100")
frame=Frame(
    window,
    padx=100,
    pady=100
)
height_lb = Label(
   frame,
   text=f"{RandomEmoji(1)} Вас приветствует калькулятор 0.3"
)
height_lb.grid(row=3, column=1)

height_lb = Label(
   frame,
   text=f"{RandomEmoji(1)} выберите вид калькулятора:"
)
height_lb.grid(row=4, column=1)

frame.pack(expand=True)

height_lb = Label(
   frame,
   text=f"{RandomEmoji(1)} 1 - системы счисления"
)
height_lb.grid(row=5, column=1)
frame.pack(expand=True)

height_lb = Label(
   frame,
   text=f"{RandomEmoji(1)} 2 - обычный"
)
height_lb.grid(row=6, column=1)
frame.pack(expand=True)

height_lb = Label(
   frame,
   text=f"{RandomEmoji(1)} 3 - химический"
)
height_lb.grid(row=7, column=1)
frame.pack(expand=True)

userVariant = Entry(
   frame,
)
userVariant.grid(row=8, column=1)

cal_btn = Button(
   frame,
   text='Выбор',
   command=UV(userVariant)
)
cal_btn.grid(row=9, column=1)

window.mainloop()
```
