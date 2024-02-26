Link to discussion : 
[click here!](https://github.com/HamidrezaRahimian/Python-Programming/discussions)

__________________________________________________________________________________________________________



Data Types baby!!!!
which are in python also same as most other programm languages which are :

**Numeric Types: | int, float, complex
Sequence Types: | list, tuple, range
Mapping Type: | dict
Set Types: | set, frozenset
Boolean Type: | bool
Binary Types: | bytes, bytearray, memoryview
None Type: | NoneType**

here are some simple example for it :

x = "Hello World"                                                       	str	
x = 20	                                                                       int	
x = 20.5	                                                                       float	
x = 1j	                                                                     complex	
x = ["apple", "banana", "cherry"]                          	list	
x = ("apple", "banana", "cherry")	                            tuple	
x = range(6)                                                          	range	
x = {"name" : "John", "age" : 36}	                             dict	
x = {"apple", "banana", "cherry"}	                           set	
x = frozenset({"apple", "banana", "cherry"})	frozenset	
x = True	                                                                       bool	
x = b"Hello"	                                                        bytes	
x = bytearray(5)	                                                   bytearray	
x = memoryview(bytes(5))                    	memoryview	
x = None	                                                       NoneType

😅 😅 😅 😅 😅 😅 😅 😅 😅 😅 😅 😅 😅 😅 
![image](https://github.com/HamidrezaRahimian/Python-Programming/assets/143603503/a2c40061-7762-4010-83cc-933fbe079a3f)


______________________________________________________________________________________________________
here is a link to a simple exam if u wanna try your self 

https://www.w3schools.com/python/exercise.asp?filename=exercise_datatypes1



______________________________________________________________________________________________________
time to get busy with Arrays !

lets start with a real easy function which can provide us the MIN and MAX of an array :

```
def find_max_and_min (list):
   return max(list) , min (list)
```

it was super easy wasnt it ? 

______________________________________________________________________________________________________
now lets define a funciton which will remove duplicate form a list :

```
def remove_duplicates(list):
   return (list(set(list)))
```

we just used the functionality of set to remove duplicate and then forced the file into a list again haha easy

![image](https://github.com/HamidrezaRahimian/Python-Programming/assets/143603503/f873a5d3-0c0f-4e99-83ee-e38b08a25b7a)


______________________________________________________________________________________________________

now lets take a look at the code for Transaction task.
we have a list of tranasaciton and we want to figure out how much was the total transactions that was done yesterday

```
# List of transactions, each represented as a dictionary simple and easy haha
transactions = [
    {'type': 'Purchase', 'amount': 450, 'date': '15-01-2024'},
    {'type': 'Sale', 'amount': 60, 'date': '14-01-2024'},
    {'type': 'Purchase', 'amount': 72, 'date': '14-01-2024'},
]

# Extracting values from the first transaction was not asked but i wrote it here anyway
transaction_type = transactions[0]['type']  # Get the 'type' value from the first transaction
transaction_amount = transactions[0]['amount']  # Get the 'amount' value from the first transaction
transaction_date = transactions[0]['date']  # Get the 'date' value from the first transaction

# Function to create a list of values for a given key (long story short , ask a key and get the value haha)
def list_of(my_key):
    # Use a loop to go through each transaction and get the value associated with the given key
    amount_values = [transaction[my_key] for transaction in transactions]
    return amount_values

# Calling the function with the argument 'amount'
# This creates a list of 'amount' values from each transaction
amount_list = list_of('amount')

# Printing the result
print(amount_list)
```
so the out put of this code will be :
[450, 60, 72]

but since we want SUM of them all need to add some lines of code :((((
lets do it:
```
# List of transactions, each represented as a dictionary
transactions = [
    {'type': 'Purchase', 'amount': 450, 'date': '15-01-2024'},
    {'type': 'Sale', 'amount': 60, 'date': '14-01-2024'},
    {'type': 'Purchase', 'amount': 72, 'date': '14-01-2024'},
]

# Extracting values from the first transaction
transaction_type = transactions[0]['type']  # Get the 'type' value from the first transaction
transaction_amount = transactions[0]['amount']  # Get the 'amount' value from the first transaction
transaction_date = transactions[0]['date']  # Get the 'date' value from the first transaction

# Function to create a list of values for a given key
def list_of(my_key):
    # Use a loop to go through each transaction and get the value associated with the given key
    amount_values = [transaction[my_key] for transaction in transactions]
    return amount_values

# Calling the function with the argument 'amount'
# This creates a list of 'amount' values from each transaction
amount_list = list_of('amount')

# Printing the result
print(amount_list)
```