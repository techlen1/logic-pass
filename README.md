# logic-pass
# Task solution
# Q1/Write a method that will remove any given character from a String? SOLUTION:
str = input("Enter a string: ")
str1 = ""
n = int(input("Character number want to remove: "))

for s in range(len(str)):
    if s == n:
        continue
    else:
        str1 = str1 + str[s]
print(str1)

# Q2/Write a program to find all prime numbers up to a given range
of numbers? SOLUTION:
s = int(input("Enter start number here: "))
e = int(input("Enter end number here: "))

for n in range(s, e):
    if n > 1:
        for i in range(2, n):
            if (n % i) == 0:
                break
        else:
            print(n)
            
# Q3/write a function that count how many the given character repeated
in a given string? SOLUTION:
def count(g, s) :
     
    # Count variable
    out = 0
     
    for o in range(len(g)) :
         
        # Checking character in string
        if (g[o] == s):
            out = out + 1
    return out
     
     
# Driver code
str= "AI Climate Change"
c = 'C'
print(count(str, c))
