# Diziler (Arrays) 

Java'da diziler, aynı türdeki verileri içeren veri yapılarıdır. İşte temel özellikleri:

## Tanımlama

Dizi tanımlamak için veri tipi belirtilir, ardından dizi ismi ve boyutu belirtilir.

```java
public class Main {
    public static void main(String[] args) {
        // Dizi tanımlama ve başlangıç değerleri atama
        int[] numbers = {10, 20, 30, 40, 50};

        // Diziyi ekrana yazdırma
        System.out.print("Dizinin Elemanları: ");
        for (int number : numbers) {
            System.out.print(number + " ");
        }

        // Dizi elemanlarına ulaşma ve toplamını alma
        int sum = 0;
        for (int i = 0; i < numbers.length; i++) {
            sum += numbers[i];
        }

        // Dizi toplamını ekrana yazdırma
        System.out.println("\nDizinin Toplamı: " + sum);
    }
}

