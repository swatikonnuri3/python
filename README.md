menu={
    "Pizza":100,
    "Pasta":120,
    "Burger":110,
    "Pepsi":70,
    "Salad":60,
    "Coffee":40
}
print("welcome to PYTHON RESTAURANT")
for key,value in menu.items():
    print(key,":",value)
total=0
item1=input("Please enter the name of the item that u want to order:")
if item1 in menu:
    total+=menu[item1]
    print(f"your {item1} has been added to your order")
else:
    print(f"Sorry,ordered {item1} is not avaialable yet")
item_2=input("Do you want to add another item ? (Yes/No)")
if item_2=="Yes":
    item2=input("Please enter the name of the item that u want to order:")
    if item2 in menu:
        total+=menu[item2]
        print(f"your {item2} has been added to your order")
    else:
         print(f"Sorry,ordered {item2} is not avaialable yet")
print("The total amount of your ordered items is",total)
        
