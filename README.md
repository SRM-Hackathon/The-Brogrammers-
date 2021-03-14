# The-Brogrammers-
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
