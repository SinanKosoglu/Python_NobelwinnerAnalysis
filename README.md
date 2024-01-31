# GİRİŞ KONULARI VE BASİT KOMUTLAR:
.
.
.
.
.
.
.
.
.
.
# BASİT KOMUTLAR

# Hello World
print("hello world")


### Sayılar (numbers) ve karakter dizileri (string)

int : 9

float : 9.2

# integer : tam sayı

# float : ondalıklı sayı

### Veri tipini sorgulama

type(9)
#integer

type(9.4)
#float

type("hello world")
#string

### Atamalar ve Değişkenler(Assignments & Variables)


a = 9
b = 24.56

print(a + b)

print(a * b)

d = a + b
d

### Data Structures (Veri Yapıları)


* en küçük yapı taşıdır
* veri yapılarına giriş
* sayılar(numbers) : int, float,complex
* karakter dizileri(string) : str
* boolen(true - false) : bool
* liste(list)
* sözlük (dictionary)
* demet (tuple)
* Küme işlemleri (set)

## Veri Yapılarına Giriş

### Sayılar (numbers) : int , float, complex

x = 53

type(x)

y = 53.6

type(y)

### boolen : true veya false

5 == 4
# eşit olup olmadığını kontrol edilir.
x = 5 == 4
# burda çıkan sonuç x değişkenine aktarılır.
x

### liste (list)

l = ["ali", "ahmet", "ahmet"]

l

type(l)

### sözlük (dictionary)

s = {"isim":"sinan", "yas":35}

s

type(s)

### set :küme

ss = {"python","ml","data science"}

ss

type(ss)

## Tipleri Değişirme

# float sayıyı integer a çevirme

c = 24.5

d = int(c)

type(d)


# integer'dan  float türüne çevirme)
b = 24

a = float(b)

type(a)


## String(Karakter Dizileri)

print("sinan")

# atama yaparak yazımı)

name = "sinan"

## çok satırlı karakter dizileri

long_str = """

merhaba bugün basit komutları işliyoruz.

"""

long_str


# değişken karakterlerine erişmek istersek
# index :0 dan başlar

long_str[3]

long_str[0:10]

### String(Karakter Dizisi) Methodları

# len : stringlerdeki boyut bilgisine erişmenizi sağlar
# len ler 1 den başlar

mat = "statistics"

len(mat)

# upper() : küçük yazılmış ifadeleri büyütür
# lower() : büyük yazılmış ifadeleri küçültür

"statistics".upper()

"STATISTICS".lower()

### replace : karakter değiştirir

hi = "hello friends"

# ilk önce değiştirmek istediğiniz harfi seçiyorsunuz sonra ne ile değiştirmek istediğinizi yazıyorsunuz

hi.replace("o","f")

### split : böler

"hello friends".split()

### capitalize : ilk harfi büyür

"foo".capitalize()

### Liste(list)

* değiştirilebilir
* sıralıdır.Index işlemleri yapılabilir
* kapsayıcıdır

notes = [1,2,3,4]
notes

type(notes)

# kapyasıcıdır : yani sadece a ve b yi almaz içindeki tüm elemanları alır

not_name = [1,2,3,4, "a","b",True,[12,24,56]]

not_name

type(not_name)

# not_name listesinin içinden bir veriye ulaşmak istersek;
# index ten saymaya başlıyor.
not_name[5]

not_name[7][2]

type(not_name[7][2])


notes = [45, 67, 89, 100]
# listede kaç veri var ??

# len saymaya 1 den başlar

len(notes)

# append methodu liste sonuna eklemeler yapar

notes.append(78)

notes


# pop : indexe göre veri siler

notes.pop(0)

notes

### Sözlük(dictionary)


* değiştirilebilir
* sırasızdır ( 3.7 sürümünden sonra sıralı)
* kapsayıcıdır


# key - value

# key : anahtardır value onun ifade ettiği değerdir

dictionary = {"Regresyon": "linear regression",
             "categoric": "renkler",
              "numeric" : "yaş"}

dictionary


# bir keyin içerisindeki value değerini göstermek istersek

dictionary["Regresyon"]


# key sorgulama

"sinan" in dictionary

"Regresyon" in dictionary


# değiştirebilirlik

dictionary["Regresyon"] = ["logistic regression"]

dictionary



# sadece bana keyleri ver

dictionary.keys()


# sadece valueları ver

dictionary.values()


# hepsine erişmek isterseniz 2. yol

dictionary.items()


# eklemek isterseniz :update

dictionary.update({"logaritma": "aritmek"})

dictionary


### TUPLE (Demet)

* değiştirilemez
* sıralıdır
* kapsayıcıdır


t = ("mark","john",35,40)

type(t)



t[0]

# eleman değiştiremezsin

t[0] = 99

'tuple' object does not support item assignment

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

# difference : set1 de olup set2 de olmayanlar

set1.difference(set2)

set2.difference(set1)

# intersection : iki kümenin kesişimi

set1.intersection(set2)

set1 & set2 # kesişim

set1 | set2 # birleşim


