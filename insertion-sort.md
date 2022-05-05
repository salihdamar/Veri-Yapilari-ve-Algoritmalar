# Proje-1
### [22,27,16,2,18,6] -> Insertion Sort

##### 1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Algoritma her seferinde dizinin üzerinde ileri doğru ilerleyerek, dizinin bir elemanını alıp geriye doğru elemanlar ile bir bir sıralar ve her bir sıralamasında, eğer sıraladığı elemandan daha küçükse o elemanla yer değiştirerek bir geriye atar.
   
ilk sayıdan bahsettiğimiz için ( 22 ) kendi başına sıralıdır. Hiç bir işlem yapmadan devam eder.
|1.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|
    
22 verisi ve 27 verisi karşılaştırma yapılır. 22, 27 küçük olduğunda ilk iki veri tamamlanır. Herhangi bir değişiklik yapılmaz.
|2.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|
    
16 ile bir gerisindeki sayıyı kıyaslar 16, 27 den küçüktür. 16 ile 27 yer değiştirir yani swap yapar. Daha sonra tekrar 16 ile 22 ü kıyaslar 16, 22 den de küçüktür. 16 ile 22 yer değiştirir.
|3.Adım|22|16|27|2|18|6|-->|16|22|27|2|18|6| 
|------|- |- |- |-|- |-|----|- |- |- |-|- |-|
       
2 ile bir gerisindeki sayıyı kıyaslar 2, 27 den küçüktür. 2 ile 27 yer değiştirir yani swap yapar. Daha sonra tekrar 2 ile 22 ü kıyaslar 2, 22 den de küçüktür. 2 ile 22 yer değiştirir. Daha sonra tekrar 2 ile 16 kıyaslar 2, 16 den de küçüktür. 2 ile 16 yer değiştirir.
|4.Adım|16|22|2|27|18|6|-->|16|2|22|27|18|6| 
|------|- |- |- |-|- |-|--|- |- |- |-|- |-|


|-->|2|16|22|27|18|6|
|-|- |- |- |-|- |-|
    
18 ile bir gerisindeki sayıyı kıyaslar 18, 27 den küçüktür. 18 ile 27 yer değiştirir yani swap yapar. Daha sonra tekrar 18 ile 22  kıyaslar 18, 22 den de küçüktür. 18 ile 22 yer değiştirir. Daha sonra tekrar 18 ile 16 kıyaslar 18, 16 den de büyüktür. Herhangi bir değişiklik yapılmaz.
|5.Adım|2|16|22|18|27|6|-->|2|16|18|22|27|6|
|------|- |- |- |-|- |-|---|- |- |- |-|- |-|
   
6 ile bir gerisindeki sayıyı kıyaslar 6, 27 den küçüktür. 6 ile 27 yer değiştirir yani swap yapar. Daha sonra tekrar 6 ile 22  kıyaslar 6, 22 den de küçüktür. 6 ile 22 yer değiştirir.  Daha sonra tekrar 6 ile 18 kıyaslar 6, 18 den de küçüktür. 6 ile 18 yer değiştirir. Daha sonra tekrar 6 ile 16  kıyaslar 6, 16 dan de küçüktür. 6 ile 16 yer değiştirir
|6.Adım|2|16|18|22|6|27|-->|2|16|18|6|22|27|
|------|- |- |- |-|- |-|-------|- |- |- |-|- |-|
    
|6.Adım|2|16|6|18|22|27|-->|2|6|16|18|22|27|
|------|- |- |- |-|- |-|-------|- |- |- |-|- |-|
     
##### 2. Big-O gösterimini yazınız.

   O(n^2)

##### 3. Time Complexity: 
###### - Worst case: Aradığımız sayının sonda olması,
Tam ters verilmiş dizi, bu durumda dizinin her bir elemanı bir gerisindekinden küçük olacaktır. Dolayısıyla 1inci eleman için iç döngü 0 2 eleman için geriye doğru 1, 3. eleman için iki daha sonra 3 4 5 6… n kadar geriye hareket yapacaktır. Yani 0+1+2+3+4…..+n-1 = [n*(n-1)]/2   :  n^2

###### - Average case: Aradığımız sayının ortada olması,
Worst case ile best casein ortalamasını aldığımızda   n^2 olarak buluruz.

###### - Best case: Aradığımız sayının dizinin en başında olması.
Tam sıralı dizi, n tane sayinin üzerinden birer defa geçer ve hiç birini geriye doğru ilerletme gereği olmadığı için bu tek geçişle kalır. Yani n

##### 4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
veri setinin sonunda olduğu için Worst case kapsamına girer.
    
#### 2. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
 |1.Adım|7|3|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |2.Adım|3|7|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |3.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |4.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
