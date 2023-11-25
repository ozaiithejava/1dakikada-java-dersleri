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
```
## OverLoading Methodlar
```Java
public class Main {
    public static void main(String[] args) {
        // İki tam sayı ile çarpma
        int resultInt = multiply(5, 3);
        System.out.println("Çarpım (int): " + resultInt);

        // İki double sayı ile çarpma
        double resultDouble = multiply(2.5, 3.0);
        System.out.println("Çarpım (double): " + resultDouble);

        // Üç sayı ile çarpma
        int resultTriple = multiply(2, 3, 4);
        System.out.println("Çarpım (üç sayı): " + resultTriple);
    }

    // İki tam sayı ile çarpma
    static int multiply(int num1, int num2) {
        return num1 * num2;
    }

    // İki double sayı ile çarpma
    static double multiply(double num1, double num2) {
        return num1 * num2;
    }

    // Üç sayı ile çarpma (overloading)
    static int multiply(int num1, int num2, int num3) {
        return num1 * num2 * num3;
    }
}
```
## Scope Örneği
```Java
public class Main {
    // Global (class) kapsamında bir değişken
    static int globalVariable = 10;

    public static void main(String[] args) {
        // Local (metod) kapsamında bir değişken
        int localVariable = 5;
        System.out.println("Local Değişken: " + localVariable);

        // Global değişkene erişim
        System.out.println("Global Değişken: " + globalVariable);

        // Blok kapsamında bir değişken
        {
            int blockVariable = 8;
            System.out.println("Blok Değişken: " + blockVariable);

            // Blok içinde global değişkene erişim
            System.out.println("Global Değişken (Blok): " + globalVariable);
        }

        // Blok dışında blok değişkenine erişim yok
        // System.out.println("Blok Değişken: " + blockVariable); // Hata!

        // Global değişkeni güncelleme
        globalVariable = 20;
        System.out.println("Güncellenmiş Global Değişken: " + globalVariable);
        
        // Method çağrısı ile global değişkeni kullanma
        useGlobalVariable();
    }

    // Başka bir metod içinde global değişken kullanma
    static void useGlobalVariable() {
        System.out.println("Global Değişken (Metod): " + globalVariable);
    }
}
```
## Recursion
```Java
public class Main {
    public static void main(String[] args) {
        int result = factorial(5);
        System.out.println("5 faktöriyel: " + result);

        int fibonacciResult = fibonacci(7);
        System.out.println("Fibonacci(7): " + fibonacciResult);
    }

    // Faktöriyel hesaplayan recursive metod
    static int factorial(int n) {
        if (n == 0 || n == 1) {
            return 1;
        } else {
            return n * factorial(n - 1);
        }
    }

    // Fibonacci sayıları hesaplayan recursive metod
    static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        } else {
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
    }
}
```
