from tkinter import *
from tkinter.ttk import *

screen = Tk()
screen.geometry("300x370")

screen.title("Bake Shop")


def bill():

    quantity1 = int(quantity.get())
    order = (Lb1.get(ACTIVE))

    total = ''

    if order == 'Option 1':
        total = 2.5 * quantity1
    if order == 'Option 2':
        total = 3 * quantity1
    if order == 'Option 3':
        total = 2.75 * quantity1

    result.set(f'''Your final bill is AED {total}
Thank You!''')


Label(text="Bake Shop").pack()
Label(text="").pack()

Label(text='''MENU
1) Brownie: AED 2.5
2) Croissant: AED 3
3) Chocolate Cookie: AED 2.75''').pack()
Label(text="").pack()

Lb1 = Listbox(height=3)
Lb1.insert(1, "Option 1")
Lb1.insert(2, "Option 2")
Lb1.insert(3, "Option 3")
Lb1.pack()
Label(text="").pack()

Label(text=f"How many do you wish to order?").pack()
quantity = Entry(screen)
quantity.pack()
Label(text="").pack()

Button(text="Finish Order", command=bill).pack()
Label(text="").pack()


Separator1 = Separator(screen, orient=HORIZONTAL)
Separator1.pack(fill=X)
Label(text="").pack()

result = StringVar()
Label(text="", textvariable=result).pack()

screen.mainloop()
