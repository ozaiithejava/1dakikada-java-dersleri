# Java String ve String Metodları

Java'da `String` sınıfı metinleri temsil etmek için kullanılır. İşte bazı temel `String` metodları:

| Metod            | Açıklama                                             | Örnek Kullanım                     |
|------------------|------------------------------------------------------|------------------------------------|
| `length()`       | String'in uzunluğunu döndürür.                       | `"Merhaba".length()` - Sonuç: 7    |
| `charAt(index)`  | Belirtilen indeksteki karakteri döndürür.           | `"Java".charAt(1)` - Sonuç: 'a'    |
| `concat(str)`    | String'i başka bir String ile birleştirir.          | `"Hello".concat(" World")` - Sonuç: "Hello World"  |
| `toUpperCase()`  | String'i büyük harfe dönüştürür.                    | `"java".toUpperCase()` - Sonuç: "JAVA"    |
| `toLowerCase()`  | String'i küçük harfe dönüştürür.                    | `"JAVA".toLowerCase()` - Sonuç: "java"    |
| `substring(beginIndex)`| Belirtilen indeksten itibaren alt dizesini döndürür. | `"Merhaba".substring(3)` - Sonuç: "haba" |
| `equals(str)`    | İki String'in eşit olup olmadığını kontrol eder.  | `"Java".equals("java")` - Sonuç: false  |
| `startsWith(prefix)`| Belirtilen önek ile başlayıp başlamadığını kontrol eder. | `"Merhaba".startsWith("Mer")` - Sonuç: true |
| `endsWith(suffix)`| Belirtilen sone erip ermediğini kontrol eder.     | `"Java".endsWith("va")` - Sonuç: true    |
| `contains(str)`  | Belirtilen alt dizenin String içinde olup olmadığını kontrol eder. | `"Merhaba".contains("rha")` - Sonuç: true  |
| `replace(oldChar, newChar)`| Belirtilen eski karakteri yeni karakterle değiştirir. | `"Hello".replace('l', 'w')` - Sonuç: "Hewwo"   |
| `trim()`         | String'in başındaki ve sonundaki boşlukları kaldırır. | `"   Java   ".trim()` - Sonuç: "Java"    |

## Örnek Kullanımlar

```java
public class Main {
    public static void main(String[] args) {
        // String oluşturma
        String text = "Merhaba, Dünya!";

        // length(): String'in uzunluğunu döndürür.
        int length = text.length(); // Sonuç: 15

        // charAt(index): Belirtilen indeksteki karakteri döndürür.
        char charAtIndex = text.charAt(7); // Sonuç: 'ü'

        // concat(str): String'i başka bir String ile birleştirir.
        String concatResult = text.concat(" Nasılsınız?"); // Sonuç: "Merhaba, Dünya! Nasılsınız?"

        // toUpperCase(): String'i büyük harfe dönüştürür.
        String upperCaseText = text.toUpperCase(); // Sonuç: "MERHABA, DÜNYA!"

        // toLowerCase(): String'i küçük harfe dönüştürür.
        String lowerCaseText = text.toLowerCase(); // Sonuç: "merhaba, dünya!"

        // substring(beginIndex): Belirtilen indeksten itibaren alt dizesini döndürür.
        String substringResult = text.substring(8); // Sonuç: "Dünya!"

        // equals(str): İki String'in eşit olup olmadığını kontrol eder.
        boolean isEqual = text.equals("Merhaba, Dünya!"); // Sonuç: true

        // startsWith(prefix): Belirtilen önek ile başlayıp başlamadığını kontrol eder.
        boolean startsWith = text.startsWith("Merhaba"); // Sonuç: true

        // endsWith(suffix): Belirtilen sone erip ermediğini kontrol eder.
        boolean endsWith = text.endsWith("Nasılsınız?"); // Sonuç: false

        // contains(str): Belirtilen alt dizenin String içinde olup olmadığını kontrol eder.
        boolean contains = text.contains("Dünya"); // Sonuç: true

        // replace(oldChar, newChar): Belirtilen eski karakteri yeni karakterle değiştirir.
        String replaceResult = text.replace('a', 'e'); // Sonuç: "Merhebe, Dünye!"

        // trim(): String'in başındaki ve sonundaki boşlukları kaldırır.
        String withSpaces = "   Java   ";
        String trimmedText = withSpaces.trim(); // Sonuç: "Java"
    }
}
