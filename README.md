# Geometrii
def geometri(sekil):
    if len(sekil) == 3:
        a = sekil[0]
        b = sekil[1]
        c = sekil[2]
        if (a+b) >c and (a+c) >b and (b+c)> a:
            if (a==b) and (b==c) and (a==c):
                print("Eshkenar ucgen")
            elif (a==b) and (b==c):
                print("Ikizkenar ucgen")
            else:
                print("Chesitkenar ucgen")
            
        else:
            print("Ucgen belirmiyor")
        
    if len(sekil) == 4:
        a = sekil[0]
        b = sekil[1]
        c = sekil[2]
        d = sekil[3]
        if (a==b) and (b==c) and (c==d):
             print("Kare")
        elif (a==b) and (c==d):
            print("Dikdortken")
        else:
            print("Dortgen belirtmiyor")
            
while True: 
    eleman_sayisi = int(input("eleman sayisini giriniz:"))
    if eleman_sayisi == 3:
        a = int(input("a:"))
        b = int(input("b:"))
        c = int(input("c:"))
        geometri([a,b,c])
            
    elif eleman_sayisi ==4:
        a = int(input("a:"))
        b = int(input("b:"))
        c = int(input("c:"))
        d = int(input("d:"))
        geometri([a,b,c,d])
    else:
        print("Lutfen tekrar giriniz")
        
