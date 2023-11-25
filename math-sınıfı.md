# Math Sınıfı Metotları

| Metot                | Açıklama                                          | Örnek Kullanım                         |
|----------------------|---------------------------------------------------|----------------------------------------|
| `abs(x)`             | Bir sayının mutlak değerini döndürür.             | `Math.abs(-5)` - Sonuç: 5              |
| `ceil(x)`            | Bir sayıyı bir üst tam sayıya yuvarlar.           | `Math.ceil(4.2)` - Sonuç: 5            |
| `floor(x)`           | Bir sayıyı bir alt tam sayıya yuvarlar.           | `Math.floor(4.9)` - Sonuç: 4           |
| `round(x)`           | Bir sayıyı en yakın tam sayıya yuvarlar.          | `Math.round(4.5)` - Sonuç: 5           |
| `max(x, y)`          | İki sayı arasındaki maksimum değeri döndürür.    | `Math.max(3, 8)` - Sonuç: 8            |
| `min(x, y)`          | İki sayı arasındaki minimum değeri döndürür.     | `Math.min(3, 8)` - Sonuç: 3            |
| `sqrt(x)`            | Bir sayının karekökünü döndürür.                 | `Math.sqrt(25)` - Sonuç: 5.0           |
| `pow(x, y)`          | Bir sayının üssünü alır.                         | `Math.pow(2, 3)` - Sonuç: 8.0          |
| `random()`           | 0 ile 1 arasında rastgele bir ondalıklı sayı üretir. | `Math.random()` - Örnek: 0.785...   |
| `sin(x)`             | Bir sayının sinüsünü hesaplar.                    | `Math.sin(Math.PI / 2)` - Sonuç: 1.0  |
| `cos(x)`             | Bir sayının kosinüsünü hesaplar.                  | `Math.cos(Math.PI)` - Sonuç: -1.0     |
| `tan(x)`             | Bir sayının tanjantını hesaplar.                  | `Math.tan(Math.PI / 4)` - Sonuç: 1.0 |

## Örnek kullanım:

```JAVA
public class Main {
    public static void main(String[] args) {
        // Mutlak değer hesaplama
        int absoluteValue = Math.abs(-5);
        System.out.println("Mutlak Değer: " + absoluteValue);

        // Yuvarlama işlemleri
        double ceilResult = Math.ceil(4.2);
        double floorResult = Math.floor(4.9);
        long roundResult = Math.round(4.5);

        System.out.println("Yukarı Yuvarlama: " + ceilResult);
        System.out.println("Aşağı Yuvarlama: " + floorResult);
        System.out.println("Yuvarlama: " + roundResult);

        // İki sayı arasındaki maksimum ve minimum
        int maxResult = Math.max(3, 8);
        int minResult = Math.min(3, 8);

        System.out.println("Maksimum: " + maxResult);
        System.out.println("Minimum: " + minResult);

        // Karekök ve üs alma
        double sqrtResult = Math.sqrt(25);
        double powResult = Math.pow(2, 3);

        System.out.println("Karekök: " + sqrtResult);
        System.out.println("Üs Alma: " + powResult);

        // Rastgele sayı üretme
        double randomResult = Math.random();
        System.out.println("Rastgele Sayı: " + randomResult);

        // Trigonometrik fonksiyonlar
        double sinResult = Math.sin(Math.PI / 2);
        double cosResult = Math.cos(Math.PI);
        double tanResult = Math.tan(Math.PI / 4);

        System.out.println("Sinüs: " + sinResult);
        System.out.println("Kosinüs: " + cosResult);
        System.out.println("Tanjant: " + tanResult);
    }
}

