## my work in python
```python
import random
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
print (" /\\__________________________________________/\\")
print ("/Вас( (|) ) приветствует калькулятор( (|) )0.1!\\")
print("\\  выберите вид калькулятора:                  /\n"
      " \\ 1 - системы счисления                      /\n"
      "  \\2 - обычный                               /\n"
      "  /3 - -\\")
userVariant=input(" /выбор: ")
if userVariant=="1":
    print("\\  выберите функцию:                /\n"
      " \\ 1 - перевод в двоичную          /\n"
      "  \\2 - перевод в восьмиричную     /\n"
      "  /3 - перевод в шестнадцатеричную\\")
    userVariantInCode=(input("функция: "))
    print ("примечание! Вы можете ввести несколько чисел в одну строку ")
    userInput=[int(x) for x in input("введите чис -ло -ла: ").split()]
    for i in range(len(userInput)):
        if userVariantInCode=="1":
            userInput[i]=bin(userInput[i])[2:]
            print (f"Число в 2-ичной системе счисления {userInput[i]}{RandomEmoji(1)}")
        elif userVariantInCode=="2":
            userInput[i]=oct(userInput[i])[2:]
            print (f"Число в 8-ричной системе счисления {userInput[i]}{RandomEmoji(1)}")
        elif userVariantInCode=="3":
            userInput[i]=hex(userInput[i])[2:]
            print (f"Число в 16-тиричной системе счисления {userInput[i]}{RandomEmoji(1)}")
if userVariant=="2":
    userVariantCalculateOne=int(input("|введите 1 число: ")) # // +- *
    userVariantCalculateTwo=int(input("|введите 2 число: "))
    userVariantCalculate=input("|введите действие: ")
    if userVariantCalculate=="/":
        if userVariantCalculateOne==0 or userVariantCalculateTwo==0:
            print ("|на 0 делить нельзя")
        elif userVariantCalculateOne!=0 or userVariantCalculateTwo!=0:
            userVariantCalculate=userVariantCalculateOne//userVariantCalculateTwo
            print(f"|Ответ {userVariantCalculate}{RandomEmoji(1)}")
    elif userVariantCalculate=="+":
        userVariantCalculate=userVariantCalculateOne+userVariantCalculateTwo
        print(f"|Ответ {userVariantCalculate}{RandomEmoji(1)}")
    elif userVariantCalculate=="-":
        userVariantCalculate=userVariantCalculateOne-userVariantCalculateTwo
        print(f"|Ответ {userVariantCalculate}{RandomEmoji(1)}")
    elif userVariantCalculate=="*":
        userVariantCalculate=userVariantCalculateOne*userVariantCalculateTwo
        print(f"|Ответ {userVariantCalculate}{RandomEmoji(1)}")
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


```



