---
num: "Lecture 2"
desc: "Python Strings and Functions"
pdfurl: /lectures/pdf/lect02.pdf
ready: true
date: 2018-10-02 9:30:00.00-7:00
---


# Resources from lecture

* [Link to all code written in lecture](https://github.com/ucsb-cs8-f18/cs8-f18-lecture-code)

## Announcements: 

* Complete [ic00](/hwk/ic00) and bring it to your lab section tomorrow
* During the first 10 minutes of the lab, try to find a suitable lab partner 
* My office hours: Wed 3:30 - 5:00 pm (HFH 1155)

## Concept Questions

* Check your understanding: [Lect 02 Concept Questions](lect02-concept.md){:data-ajax ="false"}
* You'll need your iclickers to participate in class


## Today's lecture:

* Python as a calculator
* Storing data using variables
* More than just a calculator (working with other data types)

 

* Indexing strings and substrings
    - In a string, we can extract certain pieces from it.
    - This is known as "parsing" a string
    - Positions in a string start at index 0

```python
schoolName = "UCSB"
print(len(schoolName)) # 4
print(type(schoolName)) # str
print(schoolName[0])
print(schoolName[3])
#print(schoolName[4]) #ERROR
print(schoolName[-1]) # B - refers to the last index
#print(schoolName[-5]) # ERROR

#Extract a substring
print(schoolName[1:3]) # from position 1 up to (but not
                       # including) position 3
                       
# compute salary
hours = 40
rate = 10
salary = hours * rate
print("Salary is $", salary) # Notice quotes aren't displayed on the string in the outpout

```
 
# We use something called ESCAPE CHARACTERS to print
# special characters including quotes.

print("\"Hi!\"") # \" is the double quote characters
print("Hi\nthere\n!") # \n is the newline character


# Another larger example
TAX_RATE = 0.1
print("Hi, please enter your name: ")
userName = input()
print("Hi", userName, ". What is the amount of your bill \
(not including tax and tip)?")
totalBill = float(input()) #be careful, will crash if not float
print("What is the tip percentage you would like to leave?")
tipPercentage = float(input())
taxAmount = totalBill * TAX_RATE
tipAmount = totalBill * (tipPercentage / 100)
print("The total amount to pay is $", totalBill + taxAmount + tipAmount)
```

