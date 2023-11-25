# Java Döngü Yapıları

- **Eski Döngü Yapıları:**
  - `for` Döngüsü
    - Java'nın eski sürümlerinde sıkça kullanılan döngü yapısı.
    - Belirli bir aralıkta veya koşula göre tekrarlanan işlemler için kullanılır.
  - `while` Döngüsü
    - Belirli bir koşul sağlandığı sürece tekrarlanan işlemler için kullanılır.
    - Genellikle bir sayaç artırılarak veya azaltılarak kontrol edilir.

- **Yeni Döngü Yapıları:**
  - For-each Döngüsü
    - Java 5 ve sonrasında eklenen bir döngü yapısı.
    - Koleksiyonlarda (List, Set, vb.) ve dizilerde rahatça gezinmek için kullanılır.
  - Stream API ile Döngü
    - Java 8 ve sonrasında eklenen Stream API, işlemleri daha fonksiyonel bir şekilde tanımlamanıza olanak tanır.
    - Paralel işlemleri destekler ve kodu daha okunabilir hale getirir.

- **Eski ve Yeni Döngü Yapıları Karşılaştırması:**
  - Eski `for` Döngüsü ile Liste Gezme
    - Java'nın eski sürümlerinde kullanılan yöntem.
  - Yeni For-each Döngüsü ile Liste Gezme
    - Java 5 ve sonrasında eklenen daha sade ve okunabilir bir yöntem.

- **Yenilikler ve Eklemeler:**
  - Java 5 ile birlikte For-each döngüsü (enhanced for loop) eklenmiştir.
  - Java 8 ile Stream API tanıtılmıştır. Bu API, koleksiyonlarda veri işleme yeteneklerini artırır ve kodu daha işlevsel hale getirir.
  - Yeni döngü yapıları, kodun daha sade ve okunabilir olmasını sağlar.

## Örnek Kullanım:
```Java

public class Main {
    public static void main(String[] args) {
        // Eski for döngüsü
        for (int i = 0; i < 5; i++) {
            System.out.println("Eski for döngüsü: " + i);
        }

        // Eski while döngüsü
        int j = 0;
        while (j < 5) {
            System.out.println("Eski while döngüsü: " + j);
            j++;
        }

        // Yeni for-each döngüsü
        int[] numbers = {1, 2, 3, 4, 5};
        for (int number : numbers) {
            if (number == 3) {
                break; // Döngüyü sonlandırır
            }
            System.out.println("Yeni for-each döngüsü: " + number);
        }

        // Yeni Stream API ile döngü
        List<String> names = Arrays.asList("Alice", "Bob", "Charlie");
        names.stream().forEach(name -> {
            if (name.equals("Bob")) {
                return; // Döngüyü sıradaki adıma geçirir
            }
            System.out.println("Yeni Stream API döngüsü: " + name);
        });

        // Eski for döngüsü ile liste gezme ve break
        List<String> colors = Arrays.asList("Red", "Green", "Blue");
        for (int k = 0; k < colors.size(); k++) {
            if (k == 1) {
                break; // Döngüyü sonlandırır
            }
            System.out.println("Eski for döngüsü ile liste gezme: " + colors.get(k));
        }

        // Yeni for-each döngüsü ile liste gezme ve continue
        List<String> colorsNew = Arrays.asList("Red", "Green", "Blue");
        for (String color : colorsNew) {
            if (color.equals("Green")) {
                continue; // Döngüyü sıradaki adıma geçirir
            }
            System.out.println("Yeni for-each döngüsü ile liste gezme: " + color);
        }
    }
}
