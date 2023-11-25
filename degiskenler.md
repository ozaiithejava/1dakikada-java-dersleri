
# Java Veri Tipleri

Bu dökümantasyon, Java programlama dilinde kullanılan temel veri tiplerini ve örneklerini içermektedir.

## Veri Tipleri

| Veri Tipi | Örnek Değişken | Açıklama |
|------------|----------------|----------|
| `byte`     | `byteVariable` | 8-bit işaretli tam sayı, -128 ile 127 arasında değer alabilir. |
| `short`    | `shortVariable`| 16-bit işaretli tam sayı, -32768 ile 32767 arasında değer alabilir. |
| `int`      | `intVariable`  | 32-bit işaretli tam sayı, -2147483648 ile 2147483647 arasında değer alabilir. |
| `long`     | `longVariable` | 64-bit işaretli tam sayı, -9223372036854775808 ile 9223372036854775807 arasında değer alabilir. (sonuna "L" eklenmelidir) |
| `float`    | `floatVariable`| 32-bit ondalık sayı, yaklaşık 7 haneli kesirli sayıları ifade eder. |
| `double`   | `doubleVariable`| 64-bit ondalık sayı, yaklaşık 15 haneli kesirli sayıları ifade eder. |
| `char`     | `charVariable` | 16-bit Unicode karakter, tek bir karakteri temsil eder. |
| `boolean`  | `booleanVariable`| `true` veya `false`, mantıksal durumu ifade eder. |
| `String`   | `stringVariable`| Metin dizisi, metin verilerini ifade eder. |
| `Object`   | `objectVariable`| Nesne, Java'daki tüm sınıfların temel sınıfıdır, her şeyin bir nesne olduğunu temsil eder. |

## Kullanım Örnekleri

```java
// Örnek Kullanım
byte byteVariable = 42;
short shortVariable = 300;
int intVariable = 5000;
long longVariable = 123456789L;

float floatVariable = 3.14f;
double doubleVariable = 2.71828;

char charVariable = 'A';

boolean booleanVariable = true;

String stringVariable = "Merhaba, Dünya!";
Object objectVariable = new Object();
