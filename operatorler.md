# Java Operatörleri

Java'da birçok operatör bulunmaktadır. Bu operatörler aritmetik, karşılaştırma, mantıksal ve atama gibi farklı kategorilere ayrılabilir.

| Operatör | Açıklama               | Örnek                 |
|----------|------------------------|-----------------------|
| `+`      | Toplama                | `a + b`               |
| `-`      | Çıkarma                | `a - b`               |
| `*`      | Çarpma                 | `a * b`               |
| `/`      | Bölme                  | `a / b`               |
| `%`      | Mod (Kalan)            | `a % b`               |
| `++`     | Bir artırma            | `a++` (a'nın değerini artırır) |
| `--`     | Bir azaltma            | `a--` (a'nın değerini azaltır) |

| Operatör | Açıklama               | Örnek                 |
|----------|------------------------|-----------------------|
| `==`     | Eşittir                | `a == b`              |
| `!=`     | Eşit değildir          | `a != b`              |
| `>`      | Büyüktür               | `a > b`               |
| `<`      | Küçüktür               | `a < b`               |
| `>=`     | Büyük veya eşittir     | `a >= b`              |
| `<=`     | Küçük veya eşittir     | `a <= b`              |

| Operatör | Açıklama               | Örnek                 |
|----------|------------------------|-----------------------|
| `&&`     | Mantıksal ve           | `a && b`              |
| `||`     | Mantıksal veya          | `a || b`              |
| `!`      | Mantıksal değil         | `!a`                  |

| Operatör | Açıklama               | Örnek                 |
|----------|------------------------|-----------------------|
| `=`      | Atama                  | `a = b`               |
| `+=`     | Toplama ile ata        | `a += b`              |
| `-=`     | Çıkarma ile ata        | `a -= b`              |
| `*=`     | Çarpma ile ata         | `a *= b`              |
| `/=`     | Bölme ile ata          | `a /= b`              |
| `%=`     | Mod ile ata            | `a %= b`              |

Bu tabloda, temel aritmetik, karşılaştırma, mantıksal ve atama operatörleri bulunmaktadır. Her operatörün ne işe yaradığını ve nasıl kullanılacağını açıklayan örnekler eklenmiştir. Bu sayede operatörleri anlamak ve kullanmak daha kolay olacaktır.

## Karşılaştırma Operatorleri
```Java
int x = 5;
int y = 10;

// Eşittir
boolean esittir = (x == y);    // Sonuç: false

// Eşit Değildir
boolean esitDegildir = (x != y);  // Sonuç: true

// Büyüktür
boolean buyuktur = (x > y);     // Sonuç: false

// Küçüktür
boolean kucuktur = (x < y);     // Sonuç: true

// Büyük veya Eşittir
boolean buyukEsittir = (x >= y);   // Sonuç: false

// Küçük veya Eşittir
boolean kucukEsittir = (x <= y);   // Sonuç: true
```
## Mantıksal Operatörler
```Java
boolean trueValue = true;
boolean falseValue = false;

// Mantıksal ve
boolean andSonuc = (trueValue && falseValue);  // Sonuç: false

// Mantıksal veya
boolean orSonuc = (trueValue || falseValue);   // Sonuç: true

// Mantıksal değil
boolean notSonuc = !trueValue;                 // Sonuç: false
```
## Atama Operatörleri
```Java
int a = 5;
int b = 3;

// Atama
int atama = a;            // atama değeri: 5

// Toplama ile Atama
a += b;                   // a'nın yeni değeri: 8

// Çıkarma ile Atama
a -= b;                   // a'nın yeni değeri: 5

// Çarpma ile Atama
a *= b;                   // a'nın yeni değeri: 15

// Bölme ile Atama
a /= b;                   // a'nın yeni değeri: 5

// Mod ile Atama
a %= b;                   // a'nın yeni değeri: 2
