# PythonSol
In this kata you will create a function that takes a list of non-negative integers and strings and returns a new list with the strings filtered out.

def filter_list(l):
    result=[]
    for i in range(len(l)):
        if isinstance(l[i],int):
            result.append(l[i])
    return result

Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order.
Essentially, rearrange the digits to create the highest possible number.

def descending_order(num):
    return int("".join, (sorted(str(num), reverse=True)))
    
Complete the square sum function so that it squares each number passed into it and then sums the results together.

def square_sum(numbers):
    summa=0
    for el in numbers:
        summa+=el**2      
    return summa  

задача: «Пассажиры автобуса» 🚌

Суть: Посчитать, сколько человек осталось в автобусе после всех остановок.

Входные данные: Список пар чисел [[зашли, вышли], [зашли, вышли], ...].

def number(bus_stops):
    result=0
    for on,off in bus_stops:
        result+=on
        result-=off
    return result

    Write a function findNeedle() that takes an array full of junk but containing one "needle"
    def find_needle(haystack):
    count=-1
    for el in haystack:
        count+=1
        if el=="needle":
            return f"found the needle at position {count}" 
            
Начала и конец слово должны быть равны
def feast(beast, dish):
    return beast[0] == dish[0] and beast[-1] == dish[-1]


Complete the function that accepts a string parameter, and reverses each word in the string. All spaces in the string should be retained.

Examples
"This is an example!" ==> "sihT si na !elpmaxe"
"double  spaces"      ==> "elbuod  secaps"

def reverse_words(text):
    words=text.split(" ")
    sentence=[]
    for i in words:
        reverse=i[::-1]
        sentence.append(reverse)
        
    return " ".join(sentence)
    


        
        
