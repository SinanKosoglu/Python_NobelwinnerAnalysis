***BASİT KOMUTLAR***

### Hello World

print("hello world")

### Sayılar(numbers) ve karakter diziler(string)

* int : 9 
* float : 9.2

# intege#r : tam sayı 
# float : ondalıklı sayı 

9

9.6

print(9.13)

### Veri tipini sorgulama

type(9)

type(9.4)

type("hello world") # string : text yani yazı türündeki kodlar 



### Atamalar ve Değişkenler(Assignments & Variables)

a = 9 

a 

b = 24.56

b

print(a + b)

print(a * b)

d = a + b

d



### Data Structures (Veri Yapıları)

* en küçük yapı taşıdır
* veri yapılarına giriş ve hızlı özet
* sayılar(numbers) : int, float,complex
* karakter dizileri(string) : str
* boolen(true - false) : bool
* liste(list)
* sözlük (dictionary)
* demet (tuple)


### Veri Yapılarına Giriş ve Hızlı Özet

# int 
x = 53

### Sayılar (numbers) : int , float, complex

x = 53 # int 

x

type(x)

# float 

y = 53.6

y 

type(y)

# boolen : true false 

5 == 4

x = 5 == 4

x

type(x)

# liste 

l = ["ali", "ahmet", "ahmet"]

l

type(l)

# sözlük (dictionary)

s = {"isim":"tolga", "yas":25}

s

type(s)

# set :küme 

ss = {"python","ml","data science"}

ss

type(ss)



### Tipleri Değişirme

# ondalık sayıyı integer a çevirelim


c = 24.5

# int - float 

int(c)

type(c)

d = int(c)

d

type(d)

### String(Karakter Dizileri)

print("tolga")

# atama yaparak deneyelim

name = "tolga" 

print(name)

name

# çok satırlı karakter dizileri

long_str = """  
merhaba bugün basit komutları işliyoruz

"""

long_str

# değişken karakterlerine erişmek istersek  
# index :0 dan başlar  

long_str[3]

long_str[0:10]

### String(Karakter Dizisi) Methodları

dir(str)

# len : stringlerdeki boyut bilgisine erişmenizi sağlar 
# len ler 1 den başlar 

mat = "statistics"

len(mat)

# upper() : küçük yazılmış ifadeleri büyütür
# lower() : büyük yazılmış ifadeleri küçültür

"statistics".upper()

"STATISTICS".lower()

# replace : karakter değiştirir 

hi = "hello friends" 

# ilk önce değiştirmek istediğiniz harfi seçiyorsunuz sonra ne ile değiştirmek istediğinizi yazıyorsunuz 

hi.replace("o","f")

# split : böler 

"hello friends".split()

# capitalize : ilk harfi büyür 

"foo".capitalize() 

dir(str)

### Liste(list)

* değiştirilebilir
* sıralıdır.Index işlemleri yapılabilir
* kapsayıcıdır

notes = [1,2,3,4]
notes 

type(notes)

# kapyasıcıdır : yani sadece a ve b yi almaz içindeki tüm elamanları alır 

not_name = [1,2,3,4, "a","b",True,[12,24,56]]

not_name

type(not_name)

# elamana erişmek istiyorum
# indexten saymaya başlar 

not_name[5]

not_name[7]

not_name[7][2]

type(not_name[7][2])

dir(not_name)

notes = [45, 67, 89, 100]

# listede kaç eleman var 
# len saymaya 1 den başlar 

len(notes)

# append methodu liste sonuna eklemeler yapar 

notes.append(78)

notes

# pop : indexe göre elaman siler 

notes.pop(0)

notes

notes.pop(1)

### Sözlük(dictionary)

* değiştirilebilir
* sırasızdır ( 3.7 sürümünden sonra sıralı)
* kapsayıcıdır

# key - value 

# key : anahtardır value onun ifade ettiği değerdir

dictionary = {"Regresyon": "linear regression",
             "categoric": "rekler", 
              "numeric" : "yaş"}

dictionary

# bir keyin içerisindeki value değerini göstermek istersek 

dictionary["Regresyon"]

# key sorgulama

"tolga" in dictionary

"Regresyon" in dictionary

# değiştirebilirlik

dictionary["Regresyon"] = ["logistic regression"]

dictionary

dir(dictionary)

# sadece bana keyleri ver 

dictionary.keys()

# sadece valueları ver

dictionary.values()

# hepsine erişmek isterseniz 2. yol

dictionary.items()

# eklemek isterseniz :update 

dictionary.update({"logaritma": "aritmek"})

dictionary

### Demet(Tuple)

* değiştirilemez
* sıralıdır
* kapsayıcıdır

t = ("mark","john",35,40)

type(t)

t[0]

# eleman değiştiremezsin

t[0] = 99

# eğer değiştirmek isterseniz listeye çevirmek zorundasınız 

t = list(t)

type(t)

t[0] = 99

t

### Set (küme işlemleri)

* değiştirilebilir
* sırasız + eşsizdir
* kapsayıcıdır

# liste üzerinde set oluşturulur gibi düşünülebilir 

set1 = set([2,5,7])
set2 = set([2,4,7])

type(set1)

type(set2)

# difference : set1 de olup set2 de olmayanlar 

set1.difference(set2)

set2.difference(set1)

# intersection : iki kümenin kesişimi

set1.intersection(set2)

set1 & set2 # kesişim 

set1 | set2 # birleşim

# Fonksiyonlar

* belirli görevleri yerine getirmeyi amaçlayan kod parçalarıdır

**Fonksiyon Okuryazarlığı** 

* ?print ile alakalı bilgiler ve argümanlar geldi 
* arg: fonksiyonların görevini yerine getirmeyi amaçlayan alt görevcilerdir 
* docstring : tüm argümanların dökümanları vardır ve buna docstring denir

print("a")

?print

help("print")

# sep : boşluk bırakır ve arasına ifade ekler 

print("a", "b")

print("a","b",sep = "__")

print("a","b", sep = "--")

13 * 5

# girilen sayıları 2 ile çarpacak bir fonksiyon yazalım

def calculate(x):
    #body 
    print(x * 2)

calculate(5) # x yerine sayı koymalıyım ki 2 ile çarpsın 

# iki argümanlı / parametreli fonksiyon yazalım

def summer(arg1, arg2):
    
    # ne iş yapacak 
    print(arg1 + arg2)

summer(13,5)

def say_hi(): 
    print("merhaba")
    print("bugün")

say_hi()

**Fonksiyonların statement body bölümü**

def say_hi(string):
    print(string)
    print("merhaba")

say_hi()

def carpma(a,b):
    c = a * b
    print(c)

carpma(19,7)

list_store = [] 

# definiton : tanımlamak , yapacağımız işlemlerde isimlendirmeyi kendimiz istediğimiz şekilde kullanırız.
def add_element(a,b): 
    c = a * b
    list_store.append(c)
    print(list_store)

add_element(1,6)

add_element(4,7)

**Ön Tanımlı Argümanlar / Parametreler : (Default Parameters / Arguments)**

def bölme(a,b): 
    print(a / b)

print(1,3)

# ön tanımlı değerler değiştirilebilir

def say_hello(string = "merhaba"):
    print(string)
    print("hi")
    print("tolga")

say_hello()

# değiştirilebilirlik 

say_hello("naber")



Ne zaman fonksiyon yazılır ?

sokak lambalarından ısı, nem, şarj gibi bilgiler geliyor diyelim gelen bilgileri kullanarak bazı hesaplamalar yapmak istiyoruz.

bunları tek tek yazmak yerine fonksiyonel yazmak daha az zaman kaybettirir(don't repeat yourself)

(54 + 40) / 50

# fonksiyonel yazacam 

def hesapla(nem,ısı, şarj):
    print((nem + ısı) / şarj)

# pazartesi günü şarj durumu / ısı durumu gibi 

hesapla(35,67,89)



### Return
fonksiyon çıktılarını girdi olarak kullanmak

### Print vs Return

return ve print Python dilinde iki farklı işlevi olan kelimelerdir. Aşağıda bu iki kelime arasındaki farklardan bahsedebiliriz:

**return:** Bu kelime, bir fonksiyonun çalışmasını tamamladıktan sonra fonksiyonun değer döndürdüğü anlamına gelir. Örneğin, bir fonksiyon içinde bir hesaplama yaptıktan sonra, hesaplamanın sonucunu döndürmek için return kelimesini kullanırsınız.

**print:** Bu kelime, bir ifadenin ekrana yazdırılmasını sağlar. Örneğin, bir değişkenin değerini ekrana yazdırmak için print kelimesini kullanırsınız.

![image.png](attachment:image.png)

def topla1(x, y):
    sonuc = x + y
    return sonuc

print(topla1(10,5))

def hesapla(nem, ısı, şarj):
    return((nem + ısı) / şarj) # argümanlara hangi işlemleri yaptıracaksın

hesapla(45,67,88)



### Koşullar (conditions)

kodların belirli koşullara göre nasıl hareket etmesi gerektiğini tasarlar

# true - false
# bool
1 == 1

1 == 2

# if else 

if 1 == 1: 
    print("doğru")
else:
    print("yanlış")


if 1 == 2: 
    print("doğru")
else:
    print("yanlış")

number = 13

if number == 10: 
    print("sayı 10 dur")
else: 
    print("sayı 10 değildir")

Kendini tekrar etme fonksiyon yaz

def number_check(number):
    if number == 10: 
        print("sayı 10 dur")
    else: 
        print("sayı 10 değildir")

number_check(10)

number_check(11111)

# 1. koşulu sağlamıyor ama 2. koşulu sağlıyorsa "elif" dir

def number_check(number):
    if number > 10: 
        print("büyüktür 10'dan") 
    
    elif number < 10: 
        print("küçüktür 10'dan")
    
    else: 
        print("eşittir")

number_check(10)

number_check(111)

number_check(7)

### Döngüler(Loops)

* for
* while


students = ["tolga","ahmet","selin","sena"]
students[0]

### FOR

# fonksiyonel yazalım : for loop 
# for yazarken bizden beklediği 2 şey var 1. bu döngüyü nerede gerçekleştireceksin , 2 si de hangi isimlendirmeyle yapacaksın
for student in students: 
    print(student)

# her bir öğrencinin isimlerini büyütelim

for student in students: 
    print(student.upper())

# maaşlarla alakalı 

salaries = [20000, 30000, 40000, 50000]

for salary in salaries: 
    print(salary)

# ocak ayı geldi tüm personellere % 20 zam uygulayalım

for salary in salaries: 
    print(salary * 20/100 + salary)

def new_salary(salary, zam): 
    return int(salary * zam /100 + salary)

new_salary(20000,10)

salaries2 = [20000, 30000, 40000, 50000]
 # for döngüsünü kullanarak tüm listeyi dahil edebileyim aksi halde hepsini tek tek hesaplayacaktım. 
    
for salary in salaries2: 
    print(new_salary(salary,15))

### Break & While & Continue

* Break : ilgili elamana gelince durur 
* Continue : atla, pas geç

# break 

salaries = [20000, 30000, 40000, 50000]

for salary in salaries: 
    if salary == 40000: 
        break
    print(salary)


# continue : atla, pas geç 

for salary in salaries: 
    if salary == 30000:
        continue
    print(salary)





### While : dı sürece

number = 1 

while number < 5:
    print(number)
    number +=1



### Enumerate : Otomatik Conuter / Indexer ile for loop

* işlem uygulanan listelerin index bilgisini takip etmek için kullanılır.

# index bilgisine erişmek için kullanılır 

students = ["tolga","ahmet","selin","sena"] 

for index, student in enumerate(students):
    print(index, student)



### Zip

* elimizde 3 farklı isimde liste var ve biz bu listelerin elamanlarını eşlemek yani beraber kullanmak istiyoruz

students = ["tolga","ahmet","selin","sena"] 

department = ["data", "IT", "security","business"]

yas = [24, 67, 78, 89]

list(zip(students, department, yas))



### Lambda & Map & Filter & Reduce

* vector seviyesinden işlem yapmasına hitap eden araçlardır
* en önemlisi "lambda"dır
* lambdaya ek olarak "apply" dır burada yok ama lambda ile beraber kullanılır

def summer(a,b):
    return a + b

summer(5,6)



**Lambda :** kullan at fonksiyonudur, bir kereliğine kullanabiliriz

# lambda fonksiyonunu içerisinde a ve b parametreleri var : ile toplar

new_sum = lambda a,b : a + b

new_sum(35,67)

**Map:** bize döngü yazmaktan kurtarır, nesne ver ve uygulamak istediğinizi ilet der ve işlemi yapar

# eski yöntem 

salaries = [20000, 30000, 40000, 50000] 

def yeni_maas(x): 
    return x * 20 / 100 + x


yeni_maas(10000)

# for yazmaktan bile kurtardı.

list(map(yeni_maas, salaries))





**Filter**

filtreleme yapar, kullanımı azdır

# lambda ile beraber kullanılır

list_store = [1, 2, 3, 4, 5, 6] 

list(filter(lambda x: x % 2 == 1, list_store))

list(filter(lambda x: x % 2 == 0, list_store))

**Reduce**

Indergemek
reduce fonksiyonu, bağımsız değişkeninde geçirilen belirli bir işlevi , geçirilen dizide belirtilen tüm liste öğelerine uygulamak için kullanılır.

from functools import reduce 
list_store = [1,2,3,4] 

reduce(lambda a, b : a + b , list_store)



**Comprehension**

**List Comprehensions**

fazla satırda yazılan kodlar yerine işlemleri tek satırda yazmak

![image.png](attachment:image.png)

![image.png](attachment:image.png)

# klasik yol 

salaries = [20000, 30000, 40000, 50000] 

for salary in salaries: 
    print(yeni_maas(salary))

# zam yapılan işlemleri ayrı bir liste yapalım 

bos_liste = [] 

for salary in salaries: 
    bos_liste.append(yeni_maas(salary))

bos_liste

# yine klasik yoldan 2. şey eklemek istiyorum
# if else li bir şey de ekle

for salary in salaries: 
    if salary > 30000: 
        bos_liste.append(yeni_maas(salary)) 
    else: 
        bos_liste.append(yeni_maas(salary * 2)) 

bos_liste

[yeni_maas(salary * 2) if salary < 3000 else yeni_maas(salary) for salary in salaries]

# not : else var ise if bloğu ortada olur
