# PythonSol
In this kata you will create a function that takes a list of non-negative integers and strings and returns a new list with the strings filtered out.

def filter_list(l):
    result=[]
    for i in range(len(l)):
        if isinstance(l[i],int):
            result.append(l[i])
    return result

Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

def descending_order(num):
    return int("".join, (sorted(str(num), reverse=True)))
    
