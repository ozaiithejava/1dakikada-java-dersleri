# Java switch-case Tablosu

Java'da `switch-case` tablosu, bir değişkenin belirli değerlerine göre farklı kod bloklarının çalıştırılmasını sağlar.

| Yapı                                          | Açıklama                                               | Örnek Kullanım                                         |
|-----------------------------------------------|--------------------------------------------------------|--------------------------------------------------------|
| ```java switch (değişken) { case değer: ... }``` | `değişken` belirli bir `değer`e eşitse ilgili kod bloğunu çalıştırır. | ```java switch (gun) { case 1: System.out.println("Pazartesi"); break; case 2: System.out.println("Salı"); break; default: System.out.println("Geçersiz Gün"); break; }``` |

- `switch` ifadesi içinde belirtilen değişkenin değeri, her `case` ifadesi ile karşılaştırılır.
- Eğer bir `case` ifadesi sağlanırsa, o `case` ifadesinin altındaki kod bloğu çalıştırılır ve `break` ifadesi ile switch-case tablosundan çıkılır.
- Eğer hiçbir `case` ifadesi sağlanmazsa, `default` bloğu (opsiyonel) çalıştırılır.
- `break` ifadesi kullanılmazsa, `case` ifadesi sağlansa bile altındaki diğer `case` ifadeleri de çalıştırılır.

**Örnek Kullanımlar:**

1. Günlerin Kontrolü:
    ```java
    int gun = 3;

    switch (gun) {
        case 1:
            System.out.println("Pazartesi");
            break;
        case 2:
            System.out.println("Salı");
            break;
        default:
            System.out.println("Geçersiz Gün");
            break;
    }
    ```

2. Ay İsimleri:
    ```java
    int ay = 5;

    switch (ay) {
        case 1:
            System.out.println("Ocak");
            break;
        case 2:
            System.out.println("Şubat");
            break;
        case 3:
            System.out.println("Mart");
            break;
        // Diğer aylar...
        default:
            System.out.println("Geçersiz Ay");
            break;
    }
    ```

3. Haftanın Günleri (String):
    ```java
    String gunAdi = "Pazartesi";

    switch (gunAdi) {
        case "Pazartesi":
        case "Salı":
        case "Çarşamba":
        case "Perşembe":
        case "Cuma":
            System.out.println("Hafta içi");
            break;
        case "Cumartesi":
        case "Pazar":
            System.out.println("Hafta sonu");
            break;
        default:
            System.out.println("Geçersiz Gün");
            break;
    }
    ```

Bu örneklerde, farklı değişken değerlerine göre `switch-case` yapısının nasıl kullanıldığını görebilirsiniz.
