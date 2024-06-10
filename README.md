# Yildizlarla-Harf
Python dilinde yıldız ifadesiyle harf oluşturma.
E=[[" "for i in range(7)]for j in range(7)]
B=[[" "for i in range(7)]for j in range(7)]

for sutun in range(7):
    for satir in range(7):
        if satir==0 or sutun==0 or sutun==3 or sutun==6:
          E[sutun][satir]="*"
    for sutun in range(7):
        for satir in range(7):
           if (satir==0) or (satir==4 and (sutun!=0 and sutun!=3 and sutun!=6))or ((sutun==0 or sutun==3 or sutun==6) and (satir>0 and satir<4)):
            B[sutun][satir]="*"


for i in range(7):
    for j in range(5):
       print(E[i][j],end=" ")
    print(end="  ")
    for j in range (5):
       print(B[i][j],end=" ")
    print()
