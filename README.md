# Nested-Lists
Python Program for having the name(alphabetically)  of any student(s) having the second lowest grade for given names and grades of each student in a class (by storing them in a nested list)

list1=list()
list2=list()
list3=list()
n= int(input())
for _ in range(n):
        name = input()
        score = float(input())
        l=[name,score]
        list1.append(l)
x=0
if x<n:
        for i in list1:
                j= list1[x][1]
                list2.append(j)
                x=x+1
a=min(list2)
list2.remove(a)
while (min(list2)==a):
        list2.remove(a)
    
b=min(list2)
y=0
z=0
if (y<n and z<n):
        for i in list1:
                if list1[y][1]==b:
                        list3.append(list1[z][0])
                y=y+1
                z=z+1
    
list4=sorted(list3)
for i in list4:
        print(i)        
        

