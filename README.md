# Sort algoritmaları
## Selection Sort 
Dizinin en küçük elemanı bulunur ve yer değiştirme mantığıyla dizinin başından sonuna ilerlenir.

*Örneğin* : [5,7,2,9,6,1,3,75]

-Verilen dizide en küçük eleman 1 ve baştaki  ile yer değiştirir. Oluşan yeni dizi [1,7,2,9,6,5,3,75]

-Sırada dizinin ikinci elemanını bulmak var dizide 1 den sonra en küçük eleman 2 olduğundan 7 ile yer değiştirir. Dizinin yeni hali [1,2,7,9,6,5,3,75] bu şekilde son elemana kadar devam eder.

**Algoritmanın time complexity 'si O(n^2) 'dir.**



## Insertion Sort
Dizideki elemanlar 2 li gruplar halinde ele alınır. 1.sayı<2.sayı şeklinde sorgulanır ve dizinin sonuna kadar bu sorgu devam eder.

*Örneğin* : [33 44 21 83 56 73 22]

-Verilen dizide 33<44 doğrudur aynı kalır.
-44<21 yanlış 21 bir öne gelir 33<21 yanlış 1 adım daha gelir ve sıralama 21<33<44 olur. Dizi [21 33 44 83 56 73 22]. Bu şekilde son elemana kadar algoritma sorguya devam eder.

**Algoritmanın time complexity 'si O(n^2)'dir**

## Merge Sort 
Dizideki elemanlar sayısı her seferinde 2'ye bölünür en son 2 elemanlı gruplar kalır. Bu gruplar arası karşılaştırma yapılarak tekrar birleştirilir.
*Örneğin* : [5,7,2,9,6,1,3,7]

Dizi 2 ye bölünür. [5,7,2,9] ve [6,1,3,7] olur. 

Tekrar bölünür. [5,7]-[2,9]-[6,1]-[3,7] olur ilk önce kendi içlerinde bir sıralama yapılır. 

5<7, 2<9, 1<6, 3<7 ->-> [5,7]-[2,9]-[1,6]-[3,7] daha sonra yandaki grupla sorgu yapılır. 

2<5, 5<9 , 7<9 ve  1<3, 3<6, 6<7 ->-> Dizi [2,5,7,9] ve [1,3,6,7] tekrar birleştirme işlemi yapılır.

1<2, 2<3, 3<5, 5<6, 6<7, 7=7, 7<9 olduğundan dizi [1,2,3,5,6,7,7,9] olur.

**Algoritmanın time complexity 'si O(n*logn)'dir.**

## Binary search tree

Bir referans orta nokta seçilir ve seçilen orta noktaya göre elemanlar sırasıyla büyük olan sağa küçük olan sola gelicek şekilde yazılarak bir ağaç oluşturulur.

*Örneğin* : [13,3,4,12,14,10,5,1,8,2,7,9,11,6,18]

Referans noktası 10 olsun. Sırayla 13>10 sağa 3<10 sola 4<10 ve 3<4 olduğundan 3 ün sağına 4 gelir. Bu şekilde devam eder. 

![Oluşan binary search tree](https://github.com/Gizemlimsn/kodluyoruz-sort/blob/main/readmebinarysearch.png)
