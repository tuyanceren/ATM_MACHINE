# ATM_MACHINE
**Code example for an basic atm machıne with python language**
```sql
print("""
****************************
  WELCOME TO ATM MACHINE

Transactions;

1. Balance Inquiry

2. To deposit money

3. Withdrawal

Press 'q' to exit the program.

****************************
""")

balance = 1000

while True:
     action = input("choose your action:")

     if(operation=="q"):
         print("Try again")
         break
     elif(operation=="1"):
         print("your balance is {} TL.".format(balance))

     elif (operation=="2"):
         amount =int(input("enter amount:"))
         balance += amount
         print("your new balance:",balance)

     elif (operation=="3"):
         amount = int(input("enter amount:"))

         if(balance- amount <0):
             print("out of balance...")
             continue
         balance-=amount
         print("your remaining balance:",balance)

     else:
         print("invalid operation...")
```
