Link to discussion : 
[click here!](https://github.com/HamidrezaRahimian/Python-Programming/discussions)

__________________________________________________________________________________________________________
Greather/Less than in Python is easy at it seems!
we can also combine the some conditions with and  - or
check the example :
```
a = 200
b = 33
c= 500
if c<a and a>b or b<c :
 print("At least one of em is true")
```
OUTPUT:

At least one of em is true

_____________________________________________________________________________________________________________

Dictionary makes things easier!  it same as case command but looks more proffessional

```
def get_grade2(score) :
    return{
        90 <= score <= 100 : "A",
        80 <= score < 90 : "B",
        70 <= score < 80 : "C",
        60 <= score < 70 : "D",
        score < 60 : "F"
    }.get(True,"Invalid score")
#get takes care that if input is weird he will write Invalid score
print(get_grade2(85))
```

OUTPUT:

is the Grade haha!
_____________________________________________________________________________________________________________

small Tipppp : Order is important for if commands!
check the example out

```
def get_grade (score) :
    if score >= 90 :
        return "A"
    elif score >= 80 :
        return "B"
    elif score >= 70 :
        return "C"
    
    elif score >= 60 :
        return "D"
    else :
        return "F"
    
print(get_grade(85))
```

#reihenfolge ist richtig!!!!!!!!!!!

OUTPUT:

B

```

def get_grade2 (score) :
    if score >= 60 :
        return "D"
    elif score >= 70 :
        return "C"
    elif score >= 80 :
        return "B"
    elif score >= 90 :
        return "A"
    else :
        return "F"
    
print(get_grade2(85))

```

OUTPUT:

D

_____________________________________________________________________________________________________________

and here is a nice training-task :
make an XOR table using Dictionary!
Check it out :
```
def XOR (a,b) :
    return{
        a == 1 and b ==1 : "0",
        a == 1 and b ==0 : "1",
        a == 0 and b ==1 : "1",
        a == 0 and b ==0 : "0",
    }.get(True,"Invalid score")

print("________________________________________")
print(" a | b | a XOR b")
print("________________")
print(f" 1 | 1 | {XOR(1,1)}")
print(f" 1 | 0 | {XOR(1,0)}")
print(f" 0 | 1 | {XOR(0,1)}")
print(f" 0 | 0 | {XOR(0,0)}")
```


OUTPUT:


 a | b | a XOR b
 1 | 1 | 0
 1 | 0 | 1
 0 | 1 | 1
 0 | 0 | 0


![image](https://github.com/HamidrezaRahimian/Python-Programming/assets/143603503/f8365b9e-ee4c-4052-9b6d-a2d5ddb2760c)


SOS : are you able to format the table more professional (like real tables) ??? when yes i'll be happy about the comments