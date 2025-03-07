# MDP REPRESENTATION

## AIM:
The MDP Represntation of reaching a college from home without any traffic.

## PROBLEM STATEMENT:
To travel from home to college in an optimal path where you are not facing any traffic.

### Problem Description
To reach college from home without any traffic.

### State Space
```
I    ->>  Start(home)
II    ->> Terminal state(traffic)
III    ->> Intermediate state(no traffic)
IV    ->> Goal(College)
```
### Sample State
![image](https://github.com/user-attachments/assets/a3ba5517-7553-48f5-b81e-cc046bb4b168)


### Action Space:
```
Action Space:{0,1,2,3,4}
0    ->>  Same State
1    ->> Left
2    ->> Down
3    ->> Right
4    ->> Up
```
### Sample Action
![image](https://github.com/user-attachments/assets/33c2abd0-82e0-44a6-86e8-cbf4e2f2bbd3)

### Reward Function
![image](https://github.com/user-attachments/assets/af22e027-ac99-41ca-9d8e-5c683eaabe5c)

### Graphical Representation
![image](https://github.com/user-attachments/assets/a414eba3-74f9-4394-a6d7-cb9814cbd158)


## PYTHON REPRESENTATION:
```
mdp={
    1:{
    0:[(1,0,0,False)],
    1:[(1,0,0,False)],
    2:[(0.95,3,0,False),(0.05,2,0,True)],
    3:[(0.05,2,0,True),(0.95,3,0,False)],
    4:[(1,0,0,False)]},
    2:{
       0:[(1,2,0,True)],
       1:[(1,2,0,True)],
       2:[(1,2,0,True)],
       3:[(1,2,0,True)],
       4:[(1,2,0,True)]}, 
    3:{
       0:[(1,3,0,False)],
       1:[(1,3,0,False)],
       2:[(1,3,0,False)],
       3:[(0.99,4,1,True),(0.01,1,0,False)],
       4:[(0.01,1,0,False),(0.99,4,1,True)]}, 
    4:{
       0:[(1,4,0,True)],
       1:[(1,4,0,True)],
       2:[(1,4,0,True)],
       3:[(1,4,0,True)],
       4:[(1,4,0,True)]}   
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/0f3cba83-ca18-499f-b505-73916bd4fb89)


## RESULT:
Thus, The MDP Represntation of reaching a college from home without any traffic is successfully executed.

