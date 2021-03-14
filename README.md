#the-brogrammers
import time
from os import system, name
def clear(): 
    if name == 'nt': 
        _ = system('cls') 
    else: 
        _ = system('clear') 
print("Enter No of Roads:",end=" ") 
noOfRoad=int(input())
for i in range(noOfRoad):
    print("Enter no of Vech on road %d: "%(i+1),end=" ")
    noOfVech=int(input())
    print("Enter threshold value for road %d: "%(i+1),end=" ")
    threshold=int(input())
    print("Is ambulance there on road(Enter 0 or 1) %d: "%(i+1),end=" ")
    isAmbulance=int(input())
    print("Enter Waiting time:",end=" ")
    waittime=int(input())
    amb=15
    if(isAmbulance):
        while(amb):
            clear()
            print("Signal Status: Green - for ambulance")
            print(amb)
            time.sleep(1)
            amb-=1
    waittime=int(waittime*(noOfVech/threshold))
    
    while(waittime):
        clear()
        print("Signal Status: Red")
        print(waittime)
        time.sleep(1) 
        waittime-=1
    clear()
print("Over") 
