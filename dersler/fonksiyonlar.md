# Fonksiyonlar 

 Belirli bir işlevi yapmak için oluşturulan komutlar kümesidir. Özellikle sıklıkla tekrar eden işlemlerin tek bir noktadan daha pratik olarak yönetilmesi için fonksiyonlar devreye girer.

````python
def toplama(sayi1,sayi2):
   return sayi1+sayi2

def ortalama_hesapla(liste):
    ort = sum(liste) / len(liste)
    return ort

# fibonacci: Her sayının kendinden önceki iki sayının toplanması ile oluşan dizedir.
# 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55
def fibonacci(sayi):
    if sayi == 0:
        return 0
    if sayi == 1:
        return 1
    return fibonacci(sayi-1) + fibonacci(sayi-2)
````



## Kod satırlarını azaltır

​	Tekrar eden işlemler için tek seferlik oluşturacağımız bir fonksiyonu çağırdığımızda her seferinde 1'den fazla satır kodlamak yerine fonksiyonu tek satır ile çağırmamız yeterli olacaktır.

```python
# iki sayı arasındaki kalan sayıların toplamını buldurun.

sayi1 = input("Birinci sayıyı girin: ")
sayi2 = input("İkinci sayıyı gitin: ")

# Fonksiyon kullanmadan yazacak olsaydık
toplam: int = 0
if sayi1 < sayi2:
	for i in range(sayi1, sayi2):
        toplam += i
elif sayi2 < sayi1:
    for i in range(sayi2, sayi1):
        toplam += i
else:
    print("Sayılar eşit olduğundan sonuç 0 dır")
 
print("İki sayı arasındaki sayılar toplamı: ", toplam)


# fonksiyon ile yazacak olursak

def hesapla(sayi1: int, sayi2: int) -> int:
    toplam: int = 0
	if sayi1 < sayi2:
		for i in range(sayi1, sayi2):
        	toplam += i
	elif sayi2 < sayi1:
    	for i in range(sayi2, sayi1):
        	toplam += i
	else:
   		print("Sayılar eşit olduğundan sonuç 0 dır")
    return toplam

toplam: int = hesapla(sayi1, sayi2)

```



## Tekrar eden işlemlerde hatadan kaçınmanızı sağlar

```python
# Celsius cinsinden girilen sıcaklığı Fahrenheit’a dönüştüren fonksiyon
def	celsius_to_fahrenheit(celsius_sicaklık: float) -> float:
    celsius	= celsius_sicaklık
    fahrenheit = (9/5) * celsius + 32
    return fahrenheit

celsius_sicaklık = eval(input("Sıcaklık derecesini giriniz. "))
print("Sıcaklık ", celsius_to_fahrenheit(celsius_sicaklık), "Fahrenheit derecedir.")
```



# Built-in (Gömülü) fonksiyonlar

- print()

- abs()  # mutlak değeri alma

- round()  # sayıyı yuvarlama 

- all() ve any()  # veya ile ve mantığında

- bool(), list(), str(), dict(), set(), tuple()  # tip dönüşümleri için fonksiyonlar

- callable()  # Parametre olarak verilen nesnenin çağırılabilir olup olmadığını döner.

- eval() ve exec()

  - Python'da ifade(expression) ve deyim şeklinde iki farklı kavram vardır. 

    - **İfade (expression)** : Bir değer üretmek için kullanılan kod parçalarıdır.

      - Örnek: 

        ```python
        'Kalem'
        2+2
        [eleman for eleman in [1,2,3,4,5]]
        abs(-10)
        ```

    - **Deyim (statement)**: İfadeleri de kapsayan daha geniş bir kavramdır. Bütün ifadele bir deyimdir ya da ifadelerin bir araya gelmesi deyimleri oluşturur diyebiliriz.

      - Örnek:

        - ````python
          isim = 'Can'
          if True:
              print("Sonuç Doğru")
          ````

      ​		

> `eval()` fonksiyonuna parametre olarak yalnızca ifadeler verilebilir.
>
> exec()  fonksiyonu ise deyimleri alır ve işler.

- globals()  # O anki tanımlı olan global değişkenleri bir liste olarak bize döner.
- locals()  #  Çalıştığı fonksiyon veya sınıf içeriisndeki değişkenleri liste olarak döner.

- copyright(), credits(), license(), dir(), help(), id()  -> sizler de bu fonksiyonları çalıştırıp neler yaptıklarına bakın.

# Kaynakça

https://www.mobilhanem.com/





