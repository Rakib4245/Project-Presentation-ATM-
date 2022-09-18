print("Welcome to MIU Bank\n\nInsert your card")

password=1234
balance=10000
choice=0

pin=int(input("Enter your four digit pin\n"))

if pin==password:
    while choice!= 4:
        print("\n\n**** Menu ****")
        print("1 == balance")
        print("2 == diposit")
        print("3 == withdraw")
        print("4 == cancel\n")
        
        choice=int(input("\nEnter you option:\n"))
        
        if choice==1:
            print("Balance = T",balance)
            
        elif choice==2:
                dep=int(input("Enter your deposit: T"))
                balance += dep
                print("\ndeposited amount: taka" ,dep)
                print("balance = T", balance)
                
        elif choice==3:
                wit=int(input("Enter the amount to withdraw: R"))
                balance -= wit
                print("\nwithdra amount: T" ,wit)
                print("balance = T", balance)
                
        elif choice==4:
                print("\nsession Ended!! Goodbye")
        else:
            print("\nInvalid Entry!!")
