# Boolean Operatörler ve Metodlar

| Operatör/Metod | Açıklama                                          | Örnek Kullanım                        |
|-----------------|---------------------------------------------------|---------------------------------------|
| `==`            | Eşittir.                                           | `true == false` - Sonuç: false       |
| `!=`            | Eşit değildir.                                     | `true != false` - Sonuç: true        |
| `!`             | Mantıksal değildir. (Değilse)                      | `!true` - Sonuç: false               |
| `&&`            | Mantıksal ve. (Her iki şart da doğru ise)          | `true && false` - Sonuç: false       |
| `||`            | Mantıksal veya. (Herhangi bir şart doğru ise)      | `true || false` - Sonuç: true        |

| Metot           | Açıklama                                          | Örnek Kullanım                        |
|-----------------|---------------------------------------------------|---------------------------------------|
| `equals()`      | İki boolean değeri karşılaştırır.                | `true.equals(false)` - Sonuç: false  |

Bu tabloda, `boolean` veri türüyle ilgili temel operatörler ve `equals` metodu bulunmaktadır. Her birinin açıklaması ve örnek kullanımı eklenmiştir.
## Örnek Kullanım:
```Java
public class Main {
    public static void main(String[] args) {
        // Boolean operatörleri
        boolean isEqual = true == false;
        boolean isNotEqual = true != false;
        boolean notOperation = !true;
        boolean andOperation = true && false;
        boolean orOperation = true || false;

        System.out.println("Eşittir: " + isEqual);         // false
        System.out.println("Eşit Değildir: " + isNotEqual); // true
        System.out.println("Mantıksal Değil: " + notOperation); // false
        System.out.println("Mantıksal Ve: " + andOperation);    // false
        System.out.println("Mantıksal Veya: " + orOperation);   // true

        // Boolean metodu (equals)
        Boolean bool1 = true;
        Boolean bool2 = false;

        boolean equalsResult = bool1.equals(bool2);
        System.out.println("Boolean Equals: " + equalsResult); // false
    }
}
