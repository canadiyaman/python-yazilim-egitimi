# 1- Python Yazılım Dili Veri Tipleri
_________________________________________________________

### Veri Tipleri

Veri, beynimizde algılayabildiğimiz hayatımızdaki tüm tanımlamalardır.
Yazılım dilinde veri, bir programa girdi olarak alınan ve işlenen her şeydir.

- **int** (tam sayı tipi)
- **float** (ondalık sayı tipi)
- **str** (metin tipi)
- **bool** (mantıksal evet-hayır tipi)
- **list** (Çoklu veri tutabilen veri tipi)
- **tuple** (Liste ile aynı amaçlı ancak tanımlandıktan sonra içeriği değiştirilemez -Demet)
- **dict** (Sözlük yapısında anahtar:değer biçiminde toplu veri tutan tiptir)


#### a. Tam sayı değişken tanımlama örneği

~~~~python
age: int = 22

piece: int = 5

min_value: int = 5

phone_number: int = 905554443322

~~~~

#### b. Ondalık sayı değişken tanımlama örneği

~~~~python
salary: float = 4500.91

weight: float = 85.15

pi_number: float = 3.14159

~~~~

#### c. Metin değişken tanımlama örneği

~~~~python
my_name: str = "Can Adiyaman"

the_name_of_the_course: str = "Python Yazılım Dili"

a_long_text: str = """
    Lorem Ipsum is simply dummy text of 
    the printing and typesetting industry. 
    Lorem Ipsum has been the industry's 
    standard dummy text ever since the 
    1500s, when an unknown printer took 
    a galley of type and scrambled it to
    sheets containing Lorem Ipsum passages, 
    and more recently with desktop publishing 
    software like Aldus PageMaker including 
    versions of Lorem Ipsum
"""
~~~~

#### d. Mantıksal değişken tanımlama örneği

~~~~python
is_open, is_left = False, True
is_active: bool = True
~~~~

#### e. Liste veri tipi örneği

~~~~python
the_numbers: list = [11, 22, 33, 44, 55]

mixed: list = [1, False, "Ahbap", 44.55]


# Listeye yeni bir eleman ekleme
mixed.append("new guy")

# Listedeki bir elemanı değiştirme
mixed[3] = "new value"

# Listedeki bir elemanı çıkarma
the_index = mixed.index(False)
mixed.pop(the_index)
~~~~

#### f. Demet veri tipi örneği

~~~~python
the_numbers: tuple = (11, 22, 33, 44, 55)

mixed: tuple = (1, False, "Ahbap", 44.55)
~~~~

#### f. Sözlük veri tipi örneği

sozluk = { anahtar: değer }

- Anahtarlar eşsizdir.
- Değerler herhangi bir veri tipi olabilir. Limit yoktur

~~~~python

students = {
    123: "Can",
    124: "Melis",
    125: "Salih"
}

# Sözlüğe yeni bir eleman ekleme
students[126] = "Kiraz"

# Sözlükten bir değeri alma
the_student: str = students[123]
the_student2: str = students.get(123)

# Sözlükten bir değeri değiştirme
students[125] = "Salih Akgün"

# Sözlükten bir değeri silme
del students[123]

~~~~

____________________________________________________________________
> **Type safety** (Değişken tipi güvenliği) nedir ?
>> Bir değişkenin tanımlandığı sırada ne türde veri tutacağının belirtilmesidir.

> Python type safety değildir. ilk önce bir metin alan değişken daha sonra sayı değeri tutabilir.
____________________________________________________________________

### Veri Tipleri Arasında Geçiş

~~~python
converted_to_int = int(22.14)
converted_to_float = float("22.11")
converted_to_str = str(22)
converted_to_bool = bool("1")
~~~

____________________________________________________________________
> Bir değişkenin tipini öğrenmek için **type** anahtar kelimesi kullanılır.
~~~python
age = 15
type(age) # -> <class 'int'>

name = "Hello World"
type(name) # -> <class 'str'>

name = bool(name)
type(name) # -> <class 'bool'>
~~~
____________________________________________________________________

### Kaynakça
____________________________________________________________________

www.azkod.com

www.python.org
