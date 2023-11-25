
# Tür Dönüşümü (Type Casting)

Tür dönüşümü (type casting), bir veri tipini diğerine dönüştürme işlemidir. Java'da iki tür tür dönüşümü bulunur: 

1. **Büyükten Küçüğe Otomatik Dönüşüm (Widening or Implicit Casting):** Bu, küçük bir veri tipinin, büyük bir veri tipine otomatik olarak dönüştürülmesidir. Bilgi kaybı olmaz, çünkü büyük veri tipi küçük veri tipini kapsar.

    ```java
    int intValue = 42;
    long longValue = intValue;  // int otomatik olarak long'a dönüştürülür.
    ```

2. **Küçükten Büyüğe Explicit Dönüşüm (Narrowing or Explicit Casting):** Bu, büyük bir veri tipinden küçük bir veri tipine dönüşümü ifade eder. Bu durumda, açıkça belirtilmiş bir dönüşüm operatörü kullanılmalıdır ve veri kaybı riski vardır.

    ```java
    double doubleValue = 3.14;
    int intValue = (int) doubleValue;  // double'ı int'e dönüştürme, veri kaybı riski var.
    ```

## Örnek Kullanım

```java
public class TypeCastingExample {
    public static void main(String[] args) {
        // Otomatik Dönüşüm (Widening)
        int intValue = 42;
        long longValue = intValue;

        System.out.println("int Değeri: " + intValue);
        System.out.println("long Değeri: " + longValue);

        // Explicit Dönüşüm (Narrowing)
        double doubleValue = 3.14;
        int truncatedValue = (int) doubleValue;

        System.out.println("double Değeri: " + doubleValue);
        System.out.println("Truncated (int) Değeri: " + truncatedValue);
    }
}
