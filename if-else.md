 # Java if-else Tablosu

Java'da `if-else` tablosu, belirli koşullara bağlı olarak farklı kod bloklarının çalıştırılmasını sağlar.

| Yapı                   | Açıklama                                                                                                 | Örnek Kullanım                                 |
|------------------------|----------------------------------------------------------------------------------------------------------|------------------------------------------------|
| `if (koşul) { }`        | Koşul sağlandığında çalışacak bloktur.                                                                   | ```java if (sayi > 0) { System.out.println("Pozitif"); }``` |
| `else if (koşul) { }`   | Bir önceki `if` veya `else if` bloğunun koşulu sağlanmadığında ve bu koşul sağlandığında çalışacak bloktur. | ```java else if (sayi < 0) { System.out.println("Negatif"); }``` |
| `else { }`              | Hiçbir önceki koşul sağlanmadığında çalışacak bloktur.                                                  | ```java else { System.out.println("Sıfır veya Negatif"); }``` |

Her bir blok, süslü parantezler `{ }` içinde bulunan kodu içerir. Koşul sağlandığında ilgili bloktaki kod çalıştırılır. Birden fazla `else if` bloğu ekleyebilirsiniz ve her biri bir önceki koşulun sağlanmaması durumunda kontrol edilir. `else` bloğu ise hiçbir koşul sağlanmadığında çalıştırılır.

## Örnek Kullanım:
```Java
public class Main {
    public static void main(String[] args) {
        // Örnek 1: Pozitif, Negatif veya Sıfır Kontrolü
        int sayi = 10;

        if (sayi > 0) {
            System.out.println("Pozitif");
        } else if (sayi < 0) {
            System.out.println("Negatif");
        } else {
            System.out.println("Sıfır");
        }

        // Örnek 2: Haftanın Günleri
        int gun = 3;

        if (gun == 1) {
            System.out.println("Pazartesi");
        } else if (gun == 2) {
            System.out.println("Salı");
        } else if (gun == 3) {
            System.out.println("Çarşamba");
        } else if (gun == 4) {
            System.out.println("Perşembe");
        } else if (gun == 5) {
            System.out.println("Cuma");
        } else if (gun == 6) {
            System.out.println("Cumartesi");
        } else if (gun == 7) {
            System.out.println("Pazar");
        } else {
            System.out.println("Geçersiz Gün");
        }

        // Örnek 3: Not Durumu
        int not = 75;

        if (not >= 90 && not <= 100) {
            System.out.println("A");
        } else if (not >= 80 && not < 90) {
            System.out.println("B");
        } else if (not >= 70 && not < 80) {
            System.out.println("C");
        } else if (not >= 60 && not < 70) {
            System.out.println("D");
        } else if (not >= 0 && not < 60) {
            System.out.println("F");
        } else {
            System.out.println("Geçersiz Not");
        }
    }
}
