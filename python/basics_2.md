# Python Cheatsheet

## 1) Lists
- Lists can contain a mixture of `strings`, `integers`,`booleans` and so on.
```bash
friends = ['John','Michael','Terry','Eric','Graham']

print(friends[1],friends[4])
print(len(friends)) # print length of list
print(friends.count('Eric')) # print number of times Eric appears in list
```

## 2) List Manipulation 
```bash
friends = ['John','Michael','Terry','Eric','Graham']
cars = [911,130,328,535,740,308]
print(friends)
cars.sort()                 # arrange in ascending order
print(cars)
friends.sort(reverse=True)  # arrange in descending order
print(friends)
friends.reverse()           # reverse string alignment
print(friends)
```

```bash
friends = ['John','Michael','Terry','Eric','Graham']
cars = [911,130,328,535,740,308]
friends.append('TerryG')    # add at end of list
friends.insert(1,'Kyalo')   # insert at position specified. DOES NOT replace.
friends[4]='EricM'          # replace at position specified
friends.extend(cars)        # add cars list at the end
friends.remove('John')      # remove specified element
friends.pop(1)              # pop specified index. Pops last position without input
friends.clear               # Clears whole list
del friends                 # deletes list
del friends[2]              # deletes specified index
new_friends = friends[:]    # copy list
new_friends = friends.copy()# copy list
new_friends = list(friends) # copy list
print(friends)
print(min(cars))  # print minimum value
print(max(cars))  # print maximum value
print(sum(cars))  # print sum
```

```bash
sales_w1 = [7,3,42,19,15,35,9]
sales_w2 = [12,4,26,10,7,28]
sales = []

new_day = input('Enter sales for new day: ')
sales_w2.append(int(new_day))                   # have to typecast string input
print(sales_w2)                                 # was looking for where error occurs
#sales.extend(sales_w1)
#sales.extend(sales_w2)                         # have to append one by one
sales = sales_w1 + sales_w2                     # sum allows to extend in one line
print(sales)                                    # looking for error
best_day = max(sales) * 1.5                     
worst_day = min(sales) * 1.5
w1 = sum(sales_w1) * 1.5
w2 = sum(sales_w2) * 1.5
print(f'Profit for the best day is {best_day}')
print(f'Profit for the worst day is {worst_day}')
print(f'Combined profit for both days is {w1+w2}')
```