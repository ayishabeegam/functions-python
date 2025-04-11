# functions-python
#len() function returns the number of items in an object
my_list=['12','55','76','34','87']
print(my_list)
print(len(my_list))


def greetname():
    name=input("Enter your name: ")
    print('hello',name)

greetname()


#Write a Python function find_maximum(numbers)
list = list(input('enter the numbers : ').split(','))

def max_numbers():
    max = list[0]
    for i in list:
     if i > max:
        max = i
    print(max)


max_numbers()


#Local variables can be accessed only within the function or block where it is defined, whereas global variables are accessed throughout the entire program.
x=10
def modify_global():
    global x
    x=20
    print('after modification',x)

print('value before modification',x)
modify_global()



#Create a function calculate_area(length, width=5) that calculates the area of a rectangle
def calculate_area(length,width=5):
    area=length*width
    print(area)


calculate_area(10,4)
calculate_area(10)
