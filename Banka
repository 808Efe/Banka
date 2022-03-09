from time import sleep


kartsifre = int(input("Kart şifrenizi belirleyiniz : "))
giris = False

while True:
    if giris == False:
        sifre = int(input("Şifrenizi giriniz : "))
        if sifre == kartsifre:
            giris == True
            break

print("Hoşgeldiniz!")

sleep(0.5)

print("Bankaya yönlendiriliyorsunuz...")

sleep(3)

print('''BANKA       
 (1) Para Yatır
 (2) Para Çek
 (3) Bakiye Sor
 (4) Çık
''')

bakiye = 1000

while True:
    islem = input("Hangi işlemi yapmak istiyorsunuz? : ")
    if islem == "4":
        print("İyi günler dileriz...")
        sleep(2)
        break
    elif (islem == "3"):
        print("Bakiyeniz : {}".format(bakiye))
    elif (islem == "2"):
        para = int(input("Ne kadar çekmek istiyorsunuz? : "))
        if (bakiye - para < 0 ):
            print("Yetersiz bakiye.")
            continue
        bakiye -= para
        print("Yeni bakiyeniz : {}".format(bakiye))
    elif (islem == "1"):
        para = int(input("Ne kadar yatırmak istiyorsunuz? : "))
        bakiye += para
        print("Yeni bakiyeniz = {} TL".format(bakiye))
    else:
        print("Geçersiz işlem!")
