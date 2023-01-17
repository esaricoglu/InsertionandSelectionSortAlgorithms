# Insertion Sort Projesi

1) [22,27,16,2,18,6] dizisini insertion sort türüne göre aşamalarına ayrılması.

* Öncelikle 22 ve 27 sayılarını karşılaştırıyoruz. 22<27 olduğu için bu ikilinin sırası değişmiyor.
 
    * [22,27,16,2,18,6]

* Daha sonra 16'ya bakıyoruz. 22>16 olduğu için 16 sıranın başına geçer.

    * [16,22,27,2,18,6]

* Sıradaki eleman olan 2'yi inceliyoruz. 16>2 olduğu için 2 sıranın başına geçer.

    * [2,16,22,27,18,6]

* Dizinin 5. elemanı olan 18'i ele alalım. 18>2, 18>16 ve 18<22 olduğu için 18, 16 ve 22'nin arasına yerleştirilmelidir.
 
    * [2,16,18,22,27,6]

* Son olarak geriye kalan tek elemanımız olan 6'yı inceleyelim. 6>2 ve 6<16 olduğu için 6, 2 ve 16 arasına yerleştirilmelidir.

    * [2,6,16,18,22,27]

Böylece dizi insertion sort algoritmasına göre sıralanmış olur
***
2. [22,27,16,2,18,6] dizisinin Big O Notation gösteriminin yapılması.

* Dizinin ilk elemanının başlangıçta sıralı olduğu varsayıldığı için herhangi bir karşılaştırma ihtiyacı duyulmaz.

* Dizinin ikinci elemanı sadece birinci elemanla karşılaştırılabilir ve sadece 1 kez yer değiştirebilir.

* Dizimizde n kadar eleman olduğunu düşünürsek son eleman (n-1) kez karşılaştırılmış ve yer değiştirmiş olabilir.

* Bütün elemanlar için bu hesaplama yapılırsa toplam (n-1) + (n-2) + (n-3) + ... + 1 kadar karşılaştırma ve yer değişikliği yapılmış olur. Sonuç olarak formülümüz (n-1)*(n-2)'dir.

    * (n-1)*(n-2) = $n^2$ - 3n + 2

    * Big O Notation = O( $n^2$ )'dir
    ***
3. Time Complexity : [22,27,16,2,18,6] dizisi sıralandıktan sonra 18 sayısı hangi case içinde yer almaktadır?

    * Average case: Aradığımız sayının ortada olması

    * Worst case: Aradığımız sayının sonda olması

    * Best case: Aradığımız sayının dizinin en başında olması

* Dizinin sıralanmış hali aşağıdaki gibidir.
  
    * [2,6,16,18,22,27]

* Bu durumda 18 sayısı dizinin ortasında bulunduğundan "Avarage case" kapsamına girer.
