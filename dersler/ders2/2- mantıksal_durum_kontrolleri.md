# 1- Koşullu İfadeler


### a. **Eğer (if)  ve, veya ise**

 -  Belirli bir koşulun sağlandığı durumda bazı kod bloklarını çalıştırmak istediğimizde kullanılan mantıksal kontrol ifadesidir.

#### 		Eğer (if) örnekleri

~~~python
durum = True

if durum:
    print("durum doğru ise işleyecek kod bloğu")

isim = "Can"
not = 90

if not > 70 and isim == "Can":
    print("Not 70 den büyük ve ismi Can ise işleyecek olan blok")
    
renk = "mavi"

if renk == "mavi" or renk == "Mavi":
    print("Renk mavi olduğu için uygundur")

-> alternatif kullanım
if renk.lowercase() == "mavi":
	print("Renk mavi olduğu için uygundur")

renk = "mavi"
uygun_renkler = ["kızmızı", "yeşil"]

if renk in uygun_renkler:
    print("Renk uygun renklerden biri olduğu için uygundur")

~~~

### b. **Eğer değilse(elif) ve ve, veya ise**

 - İlk koşul sağlanmadığı durumda ve başka bir koşulun kontrol edilmesi gerektiği durumda kullanılan mantıksal kontrol ifadedir. 

#### 		Eğer değilse (elif) örnekleri

~~~python
yon = "sağ"

if yon == "sag":
    print("sağa kaydır")
elif yon == "sol":
    print("sola kaydır")
elif yon != "sag" or yon != "sol":
    print("Hatalı yön")
    
~~~



### c.  **Değilse(else)**

 - Eğer ve Eğer değilse bloklarındaki koşullar sağlanmadığı durumda çalıştırılmak istenen bir kod bloğu için kullanılan mantıksal ifadedir.

#### 		Değilse (else)) örnekleri

~~~python
girdi = "can"
durum = type(girdi) is str

if durum:
    ...
else:
    print("girdi str değerinde değildir")
~~~




### d.  **Ortak Kullanım**

~~~python
not = 90
baraj = 60

if not >= baraj:
    print("Geçti")
else:
    print("Kaldı")
   
kosullu_baraj = 50

if not >= baraj:
    print("Geçti")
elif not >= kosullu_baraj:
    print("Koşullu geçti")
else:
    print("Kaldı")
   
~~~


### Kaynakça
____________________________________________________________________

www.python.org

www.sadikturan.com