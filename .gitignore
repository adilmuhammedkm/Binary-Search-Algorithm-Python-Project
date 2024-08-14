# This program generates a list of random numbers with a difference of 2 between them, 
#and uses binary search algorithm to check if the user input number is in the list. 
#The program prompts the user to enter the number of elements in the list and the number to search for. 
#The generate_list() function generates the list, and the binary_search() function performs 
#the binary search on the list and returns a boolean indicating whether the number is in the list or not.
#The final result is printed to the user.


import random

# Function to generate a list of random numbers with a difference of 2 between them
def generate_list(Elements):
    list = [random.randint(0,100) for i in range(Elements)]
    list.sort()
    for i in range(1, len(list)):
        list[i] = list[i-1] + 2
    return list

# Function to perform binary search on the list
def binary_search(lst, Number):
    start = 0
    end = len(list) - 1
    while start <= end:
        mid = (start + end) // 2
        if list[mid] == Number:
            return True
        elif list[mid] < Number:
            start = mid + 1
        else:
            end = mid - 1
    return False

# Get input from the user
Elements = int(input("Enter the number of elements in the list: "))
Number = int(input("Enter the number to search for: "))

# Generate the list and perform binary search
list = generate_list(Elements)
result = binary_search(list, Number)

# Print the result
if result:
    print("The number is in the list.")
else:
    print("The number is not in the list.")
