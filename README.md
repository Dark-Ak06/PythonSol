# PythonSol
In this kata you will create a function that takes a list of non-negative integers and strings and returns a new list with the strings filtered out.

def filter_list(l):
    result=[]
    for i in range(len(l)):
        if isinstance(l[i],int):
            result.append(l[i])
    return result
