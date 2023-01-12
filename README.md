# lottery
# 1 ile 80 arasında rastgele 10 sayı seçen,
#kullanıcının girdiği sayılarla çıkan sayıların eşleşme durumuna göre ödül veren veya vermeyen bir piyango oyunu yazacağım. 
# Kullanılan (a,b,c,d,e,f,g,h,i,j) harfler rastgele seçilecek 10 sayıyı temsil ediyor. 
#(l,m,n,o,p,r,s,t,u,v) harfleri ise kullanıcıdan alınacak 10 sayıyı temsil ediyor. 



import random

a=random.randint(1,81)
b=random.randint(1,81)
c=random.randint(1,81)
d=random.randint(1,81)
e=random.randint(1,81)
f=random.randint(1,81)
g=random.randint(1,81)
h=random.randint(1,81)
i=random.randint(1,81)
j=random.randint(1,81)

pcGuess=[a,b,c,d,e,f,g,h,i,j]
final=list(pcTahmin)



l=int(input("Write your guess: "))
m=int(input("Write your guess: "))
n=int(input("Write your guess: "))
o=int(input("Write your guess: "))
p=int(input("Write your guess: "))
r=int(input("Write your guess: "))
s=int(input("Write your guess: "))
t=int(input("Write your guess: "))
u=int(input("Write your guess: "))
v=int(input("Write your guess: "))

guess=[l,m,n,o,p,r,s,t,u,v]



common=[]
for num in list(guess):
    if num in final:
        common.append(num)
print(f"Ortak sayılar: {common}")

print(f"Çekiliş sonuçları: {final}")
print(f"Seçtiğiniz sayılar: {guess}")

if len(common) == 0:
    print("Tebrikler, x lira kazandınız!")
elif len(common) > 0 and len(ortak) < 5:
    print("Üzgünüz, Kaybettiniz.")
elif len(common) == 5:
    print("Tebrikler, x lira kazandınız!")
elif len(common) == 6:
    print("Tebrikler, x lira kazandınız!")
elif len(common) == 7:
    print("Tebrikler, x lira kazandınız!")
elif len(common) == 8:
    print("Tebrikler, x lira kazandınız!")
elif len(common) ==9:
    print("Tebrikler, x lira kazandınız!")
elif len(common) ==10:
    print("Tebrikler, Büyük ikramiyeyi kazandınız!")
    
