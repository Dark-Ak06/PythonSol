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

Create a function which answers the question "Are you playing banjo?".
If your name starts with the letter "R" or lower case "r", you are playing banjo!

The function takes a name as its only argument, and returns one of the following strings:

name + " plays banjo" 
name + " does not play banjo"

def are_you_playing_banjo(name):
    return name + " plays banjo" if name[0]=="R" or name[0]=="r" else name + " does not play banjo"

Return the number (count) of vowels in the given string.
We will consider a, e, i, o, u as vowels for this Kata (but not y).
The input string will only consist of lower case letters and/or spaces.
    
def get_count(sentence):
    count=0
    vowel="aeiou"
    for char in sentence:
        if char in vowel:
            count+=1
    return count

You get an array of numbers, return the sum of all of the positives ones.

Example
[1, -4, 7, 12] => 1+7+12=20
1+7+12=20
Note
If there is nothing to sum, the sum is default to 0.

def positive_sum(arr):
    return sum(number for number in arr if number>0)
     
"camelCasing"  =>  "camel Casing"
"identifier"   =>  "identifier"
""             =>  ""

def solution(s):
    text=""
    for char in s:
        if char.isupper():
            text+= " "
        text+=char  
    return text
        
        
