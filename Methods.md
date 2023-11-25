# Java Metodları

Java'da metodlar, belirli bir işlevi yerine getiren kod bloklarıdır. İşte metodlarla ilgili temel bilgiler:

## Metod Tanımı

Metod tanımlamak için aşağıdaki form kullanılır:

```java
public class Main {
    public static void main(String[] args) {
        // Parametresiz, dönüş değeri olmayan metodun çağrılması
        printHello();

        // Parametreli ve dönüş değeri olan metodun çağrılması
        int sum = add(5, 3);
        System.out.println("Toplam: " + sum);

        // Dönüş değeri olmayan metodun çağrılması
        greet("John");

        // Overloading ile farklı parametre türleri
        double product = multiply(2.5, 3.0);
        System.out.println("Çarpım: " + product);
    }

    // Parametresiz ve dönüş değeri olmayan metod
    static void printHello() {
        System.out.println("Merhaba!");
    }

    // Parametreli ve dönüş değeri olan metod
    static int add(int num1, int num2) {
        return num1 + num2;
    }

    // Parametreli ve dönüş değeri olmayan metod
    static void greet(String name) {
        System.out.println("Merhaba, " + name + "!");
    }

    // Overloading: Farklı parametre türleri
    static double multiply(double num1, double num2) {
        return num1 * num2;
    }
}

