# odev---Beyaz-t-Bestami-zer
=====================> 3. HAFTA ÖDEVİ <======================
3 tane matamatik ya da fizik formüllünün ne işe yaradığından kısaca bahsedip, o kodu çalıştıracaksın.

1 . ==> Üç kenarı bilinen üçgenin türünü ve alanını hesaplama:
Girilen 3 kenar ile bir üçgen oluşup oluşmadığı tespit edilmeli , girilen değerlerle bir üçgen çizilebiliniyorsa bu üçgenin kenarlarına göre ne tür üçgen olduğu bulunmalı (eşkenar üçgen, ikiz kenar üçgen ve çeşitkenar üçgen) ve alanı hesaplanmalıdır.

NOT: kenar sayılarını tam sayı giriniz.

1
a = input('Birinci kenarı girin: ')
2
b = input('İkinci kenarı girin: ')
3
c = input('Üçüncü kenarı girin: ')
4
if a.isnumeric() and b.isnumeric() and c.isnumeric():
5
    a=int(a)
6
    b=int(b)
7
    c=int(c)
8
    if (a+b)>c and (b+c>a) and (c+a>b):
9
        print("üçgen oluşur.")         
10
        u = (a + b + c) / 2
11
        alan = (u*(u-a)*(u-b)*(u-c)) ** 0.5
12
        print('Üçgenin alanı:{}'.format(alan))
13
        if a==b==c:
14
           print(a,b,c, "kenarları eşkenar üçgen oluşturur.")
15
        elif a!=b!=c:
16
           print(a,b,c, "kenarları çeşitkenar üçgen oluşturur.") 
17
        else:
18
           print(a,b,c, "kenarları ikizkenar üçgen oluşturur.") 
19
    else:
20
        print("Girdiğiniz kenar uzunlukları bir üçgen oluşturulamaz.") 
21
else:
22
    print("Lütfen kenar uzunluklarını tam sayı giriniz.")  
23
​
Birinci kenarı girin: 6
İkinci kenarı girin: 8
Üçüncü kenarı girin: 4
üçgen oluşur.
Üçgenin alanı:11.61895003862225
6 8 4 kenarları çeşitkenar üçgen oluşturur.
2. ==> Mükemmel Sayıyı Bulma:
Bir sayı kendi dışındaki pozitif çarpanlarının toplamına eşitse, o sayı ' Mükemmel Sayı ' olarak adlandırılır.

NOT: Mükemmel sayılar pozitif sayılardır ve en küçük Mükemmel sayı 6'dır.

1
sayı = int(input("Sayı Giriniz:"))
2
​
3
toplam=0
4
if sayı >=0:
5
    for i in range(1,sayı):
6
       if(sayı%i == 0):
7
          toplam +=i
8
          print(i)
9
print('Pozitif bölenlerin toplamı:{}'.format(toplam))
10
if(sayı == toplam):
11
        print("Mükemmel Sayıdır.")
12
else:
13
        print("Mükemmel Sayı Degildir")
Sayı Giriniz:68
1
2
4
17
34
Pozitif bölenlerin toplamı:58
Mükemmel Sayı Degildir
3. ==> Faktöriyel Hesaplama:
n bir sayma sayısı olmak üzere 1’den n’ye kadar olan sayıların çarpımına n faktöriyel denir ve n! ile gösterilir.

NOT: Yukarıdaki kurala '0' sayısı uymadığı halde 0!=1' dir.

1
sayı = int(input("Faktöriyelini Hesaplamak için sayı giriniz:"))
2
değer = 1
3
for i in range(sayı):
4
    değer = değer * (i+1)
5
 
6
print("Faktoriyel : ", değer)
Faktöriyelini Hesaplamak için sayı giriniz:0
Faktoriyel :  1
