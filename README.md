Word=input("Enter a word/sentence: ")
ch=input("Enter a character: ")
count=0
i=0
while i<len(Word):
    if Word[i]==ch:
        count=count+1
    i=i+1
print("Number of character",ch,"Occures in",Word,"is",count)

l=int(input("Enter Lower range: "))
u=int(input("Enter Upper range: "))
print("The prime number between ",l,"and ",u,"are: ")
for num in range(l,u+1):
    if num>1:
        for i in range(2,num):
            if (num%2)==0:
                break
        else:
            print(num)
