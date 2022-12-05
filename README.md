# python-code
Random password generator


import random
import string
x=0
c1=1
c2=c3=c4=c5=0
len1=int(input("Enter the length of password: "))
lower=string.ascii_lowercase
upper=string.ascii_uppercase
digits=string.digits
symbols=string.punctuation
all=lower+upper+digits+symbols
temp=random.sample(all,len1)
a="".join(temp)
print(a)
for i in range (len(a)):
    if a[i]=='>' or a[i]=='<':
        c1=0
        break
       
for i in a:    
    if len (a)>12:
        c2=1
    if i.islower():
        c3=1
    if i.islower():
        c4=1
    if i.isdigit():
        c5=1

#print (c1, c2,c3,c4,c5)
if (c1==1 and c2==1 and c3==1 and c4==1 and c5==1):
    print("strong")
else :
    print("Invalid")
