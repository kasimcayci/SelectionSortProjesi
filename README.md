# SelectionSortProjesi
Veri Yapıları ve Algoritmalar Dersi Selection Sort Projesi
# Proje Hakkında


Proje 1 Insertion sort
22,27,16,2,18,6 dizisinin sıralanması aşamaları

i. Öncelikle ilk sıradaki veri ile dizideki en küçük veri yer değiştirir. Yani 22 ile 2 yer değiştirecek. 
Yeni dizimiz 2, 27, 16, 22, 18, 6 n tane veri tarandı

ii. Dizimizde en küçük sayıyı yerine yerleştirdik. 2, 27, 16, 22, 18, 6 dizisinde artık 2 yi göz önüne almadan ikinci sıradaki 27 ile kalan sayılar arasında en küçük değer araştırıldığında değerin 6 olduğu görülüp 27 ile 6 yer değiştirecek.
Yeni dizimiz 2, 6, 16, 22, 18, 27 n-1 tane veri tarandı

iii. Dizimizde en küçük ikinci sayıyı da yerine yerleştirdik. 2, 6, 16, 22, 18, 27 dizisinde artık 2 ve 6 göz önüne alınmadan üçüncü sıradaki 16 ile kalan sayılar arasında en küçük değer araştırıldığında kendisinin en küçük olduğu görülüp yer değiştirme yapılmadı
Dizimiz 2, 6, 16, 22, 18, 27 n-2 tane veri tarandı

iv. Dizimizde en küçük üçüncü sayı da yerinde dizimiz 2, 6, 16, 22, 18, 27 artık 2, 6 ve 16 yı göz önüne almadan dördüncü sıradaki 22 ile kalan sayılar arasında en küçük değer araştırıldığında değerin 18 olduğu görülüp 22 ile 18 yer değiştirecek
Yeni dizimiz 2, 6, 16, 18, 22, 27 n-3 tane veri tarandı

v. Dizimizde dördüncü en küçük sayı da yerine geçti. dizimiz 2 ,6, 16, 18, 22, 27 artık 2, 6, 16 ve 18 göz önüne alınmadan yine 22 ile kalan sayılar arasında en küçük değer araştırılacak zaten 2 tane veri kaldı. kalan sayıların sıralı olduğu görülüp yer değiştirme olmayacak böylelikle beşinci ve altıncı sıradaki sayılar da yerini bulmuş oldu.
Dizimiz 2, 6, 16, 18, 22, 27 1 tane veri tarandı


Big-O gösterimi 

i. aşama n tane veri tarandı bu dizide 6 veri var
ii. aşama n-1 tane veri tarandı yeni dizide 5 veri var
iii. aşama n-2 tane veri tarandı yeni dizide 4 veri var
iv. aşama n-3 tane veri tarandı yeni dizide 3 veri var
v. aşama 1 tane veri tarandı yeni dizide 2 veri vardı.

O(n^2)

Time Complexity: 18 sayısı aradığımız dizinin ortası sayılabilecek bir yer olan 4. sırada olduğundan dolayı average case olarak kabul edilse de kendisinden sonra işlem aşamalarında son iki sayının değerlendirilmesi kaldığı için benim bakış açıma göre worst case olarak değerlendirilmelidir.


7,3,5,8,2,9,4,15,6 dizisinin selection sort'a göre sıralama aşamaları

i. ilk önce birinci sıradaki değer ile bütün veriler taranıp saptanan en küçük değer yer değiştirir. Yani 7 ile 2 yer değiştirecek. Yeni dizimiz 2, 3, 5, 8, 7, 9, 4, 15, 6

ii. 2 sabit kalacağı için göz önüne alınmadan ikinci sıradaki 3 sayısı ile sonrasındaki veriler karşılaştırıldığında daha küçük değer olmadığından yer değiştirme yapılmayacak. 
Dizimiz 2, 3, 5, 8, 7, 9, 4, 15, 6

iii. 2 ve 3 sabit kalacağı için göz önüne alınmadan üçüncü sıradaki 5 sayısı ile sonrasındaki veriler karşılaştırıldığında daha küçük değer olarak 4 sayısı görülüp 5 ile 4 yer değiştirecek. 
Yeni dizimiz 2 ,3, 4, 8, 7, 9, 5, 15, 6

iv. 2, 3 ve 4 sabit kalarak göz önüne alınmayacak ve dördüncü sıradaki 8 sayısı ile sonrasındaki veriler daha küçük değer için karşılaştırılacak ve en küçük değerin 5 olduğu görülünce 8 ile 5 yer değiştirecek. Yeni dizimiz 2, 3, 4, 5, 7, 9, 8, 15, 6

