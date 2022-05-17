# 1- Döngüler
_________________________________________________________

### Döngü Tipleri

#### -  For döngüsü

​	Bir liste, demet'in veya sözlüğün her elemanını sıralı şekilde elde etmemize yarayan işlemdir.

~~~python
# Örnek 1
kullanicilar = ['Ahmet', 'Can', 'Ali']
for kullanici in kullanicilar:
    print("Kullanıcı ->", kullanici)

    
# Örnek 2
kullanici_ve_puanlari = [('Ahmet', 90), ('Can', 50), ('Ali', 87)]
for kullanici_ve_puan in kullanici_ve_puanlari:
    print(f"Kullanıcı -> {kullanici_ve_puan[0]}, Puanı: {kullanici_ve_puan[1]}")

# Örnek 3

-> listeyi tersten okumaya başlama
notlar = [1, 5, 100, 55, 200, 2]
for not in notlar:
    print("not -> ", not)

-> listeyi sıralayarak okuma
for not in notlar.sort():
    print("not ->", not)

# Örnek 4

-> Rastgele iki sayı arasında döngü oluşturma

for i in range(1, 100):
    print("sayı ->", i)

# Örnek 5

-> listenin belirli aralığında döngü oluşturma

renkler = ["mavi", "sarı", "yeşil", "kırmızı", "turuncu", "mor"]

for renk in renkler[1:4]:
    print("renk ->", renk)
~~~

#### - While döngüsü tanımlama örneği

Bir koşul sağlanana kadar ya da kod bloğu içerisinde yapılacak müdahale ile kırılana kadar devam eden sonsuz döngü tipleridir.

~~~python
# Örnek 1
limit = 10
sira = 1
while limit <= 10:
    print("sıra ->", sira)
    site += 1
    
    
# Örnek 2
limit_var = True
sira = 1
while limit_var:
    print("sıra ->", sira)
    sira += 1
    if sira == limit:
        limit_var = False

# Örnek 3 
limit = 10
sira = 1
while True:
    print("sıra ->", sira)
    sira += 1
    if sira == limit:
        break
~~~

### Kaynakça
____________________________________________________________________

www.python.org