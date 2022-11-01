# Python Cheatsheet

## 1) Data Types
There are four data types:

i) Integer
```bash
a = 15
```
ii) Float
```bash
a = 15.0
```
iii) String
```bash
name = "John"
```
iv Boolean
```bash
isGoing = False"
```

```bash
print(type('hello'))
print(type(1))
print(type(1.64))
print(type(True))
```

## 2) Typecasting
Simply call the variable you want to typecast inside the data type:
```bash
a = int(1)        # a will be 1
b = int(2.5)      # b will be 2
c = int("3")      # c will be 3
#c1 = int("3.4")   # this gives an error since string cannot be cast to int
d = float(1)      # d will be 1.0
e = float(2.5)    # e will be 2.5
f = float("3")    # f will be 3.0
g = float("4.23") # g will be 4.23
h = str("80s")    # h will be '80s'
i = str(22)       # i will be '22'
j = str(3.01)     # j will be '3.01'

print([a,b,c,d,e,f,g,h,i,j])
```

## 3) Arithmetic Operators
```bash
a=6
b=2
print('Addition : ', a + b)
print('Subtraction : ', a - b)
print('Multiplication : ', a * b)
print('Division (float) : ', a / b)
print('Division (floor) : ', a // b)
print('Modulus : ', a % b)
print('Exponent : ', a ** b)
```

## 4) String Slicing
```bash
msg='welcome to Python 101: Strings'
msg1=msg[18]+' '+msg[:8]+msg[25:29]+msg[7:11]+msg[13]+msg[12]+msg[2]+msg[1]+msg[-5]  
print(msg1.title())
print(msg1[::-1].title()) # print a string backwards
```

## 5) Replace text
```bash
msg='Welcome to Python 101: Strings'
print(msg.replace('Python','Java'))
```

## 6) Print Format
```bash
name='TERRY'
color = 'RED'
msg = '[' + name + '] loves the color ' + color.lower() + '!'
msg1 = f'[{name}] loves the color {color.lower()}!'
print(msg)
print(msg1)
```
