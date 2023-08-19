# Java-Programlama-Dilinde-Deger-ve-Referans-Tipleri
Java Programlama Dilinde Değer ve Referans Tipleri

Java Programlama Dilinde Değer ve Referans Tipleri

Java programlama dili, değer tipleri ve referans tipleri olmak üzere iki temel veri tipi kategorisini destekler. Bu iki tipteki değişkenler ve nesneler, bellekte farklı şekillerde yönetilir ve davranış gösterir. İşte Java'daki değer ve referans tiplerinin anlatıldığı bir rehber:
Değer Tipleri

Değer tipleri, bellekte doğrudan değerlerini tutan veri türleridir. Bu türler, örneğin tam sayılar, ondalık sayılar ve karakterler gibi basit veri türlerini içerir. İşte bazı yaygın değer tipleri:

    int: Tam sayıları temsil eder. Bellekte 32 bit kullanır.
    double: Ondalık sayıları temsil eder. Bellekte 64 bit kullanır.
    char: Tek bir karakteri temsil eder. Bellekte 16 bit kullanır.
    boolean: Mantıksal değerleri (true veya false) temsil eder.

Değer tipleri, değişkenlerin doğrudan bellekteki değerlerini taşıdığı anlamına gelir. Bu türdeki değişkenler, birbirinden bağımsızdır ve bir değişkenin içeriği değiştirilse bile diğer değişkenler etkilenmez. Örnek:

java

int x = 10;
int y = x;
x = 20;

System.out.println("x: " + x); // Çıktı: x: 20
System.out.println("y: " + y); // Çıktı: y: 10

Yukarıdaki örnekte görüldüğü gibi, x ve y değişkenleri bağımsızdır ve x'in değeri değişse bile y bundan etkilenmez.
Referans Tipleri

Referans tipleri, bellekte değerlerin konumunu (adresini) tutan veri türleridir. Bu türler, nesneleri ve dizileri içerir. İşte bazı yaygın referans tipleri:

    class: Nesneleri temsil eder. Örnek olarak bir sınıfın örneği.
    array: Dizi veri yapılarını temsil eder. Aynı türdeki birden fazla öğeyi içerebilir.

Referans tipleri, bellekte değerlerin kendilerini değil, değerlerin bulunduğu bellek konumlarını tutar. Bu nedenle, bir referans tipindeki değişkenler aslında nesnenin veya dizinin bellek konumunu işaret eder. Örnek:

java

int[] array1 = { 1, 2, 3 };
int[] array2 = array1;
array1[0] = 10;

System.out.println("array1[0]: " + array1[0]); // Çıktı: array1[0]: 10
System.out.println("array2[0]: " + array2[0]); // Çıktı: array2[0]: 10

Yukarıdaki örnekte görüldüğü gibi, array1 ve array2 aynı bellek konumunu işaret eder, bu nedenle birinde yapılan değişiklik diğerini etkiler.
Değer ve Referans Tipleri Arasındaki Farklar

    Değer tipleri bellekte değerlerini doğrudan tutar, referans tipleri ise bellek konumlarını işaret eder.
    Değer tipleri birbirinden bağımsızdır, referans tipleri ise aynı bellek konumunu işaret edebilir.
    Değer tipleri hızlıdır ve bellekte daha az yer kaplar, referans tipleri daha fazla bellek kullanabilir.
