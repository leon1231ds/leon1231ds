a=float(input("Nhập a là:"))
b=float(input("Nhập b là:"))
c=float(input("Nhập C là:"))
if a==0:
    if b==0 and c==0:
        print("PTVSN")
    if b!=0 and c==0:
        print("PT có nghiệm = 0")
    if b!=0 and c!=0:
        print("PT có 1 nghiệm là x=", -c/b)
    if b==0 and c!=0:
        print("PTVN")
else:
    D=b**2-4*a*c
    if D>0:
        x1=float((-b-sqrt(D))/(2*a))
        x2=float((-b+sqrt(D))/(2*a))
        print("x1=", x1)
        print("x2=", x2)
    elif D==0:
        print("PT có nghiệm kép x1=x2=", -b/(2*a))
    else:
        print("PTVN")
        
        
