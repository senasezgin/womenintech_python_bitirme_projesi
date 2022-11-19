# **SistersLab Women in Tech Academy Bitirme Projesi**

![covid-19-asisinin-dna-yi-degistirdigine-yonelik-iddialar](https://user-images.githubusercontent.com/83637039/202847597-924205aa-d55a-401e-9afd-ef082535e00e.jpg)

## Veri Seti Yorumlaması

Öncelikle bize verilen veri setindeki sütünları, bu sütündaki eksik değerleri ve eksik değerlerin oranlarını inceledim.

![2022-11-19](https://user-images.githubusercontent.com/83637039/202848306-38d908be-f4cc-4a3c-addc-4436d74f6514.png)

Verimde neyi inceleyebilirim

Bu veri seti içerisinde; covid-19 salgını ile ilgili :Kıtalar ve ülkeler bazında günlük vaka, günlük ölüm, günlük test sayısı, aşılma sayısı gibi veriler vardır.
Bunlardan çıkartabileceğimiz analizlere bakalım.


Nelere bakılması gerekiyor

1. Ülkelere göre günlük vaka sayısı.
2. Ülkelere göre ortalama vaka sayısı.
3. Ülkelere göre toplam aşılama sayısı.
4. Günlük ortalama vaka sayısı.
5. 65 yaşından büyük vakaların toplamı.


### 1. Ülkelere göre günlük vaka sayısı.

Tüm ülkeleri incelediğimde 'World'  diye bir satırlar olduğunu gördüm. Bu satırların ülke bazında yanlışlıklara yol açacağından satırları sildim.
Daha sonra ülke ve kıta bazında günlük vaka sayısını filtreledim.

![2022-11-19 (1)](https://user-images.githubusercontent.com/83637039/202855800-9daf23bd-ff16-48b1-ad83-6c5ede22c03c.png)

### 2. Ülkelere göre ortalama vaka sayısı.

![2022-11-19 (2)](https://user-images.githubusercontent.com/83637039/202856518-46fae68d-a5c4-45e6-94c9-7b3ea9adaa42.png)

### 3. Ülkelere göre toplam aşılama sayısı.

![2022-11-19 (3)](https://user-images.githubusercontent.com/83637039/202856690-7aa7edd6-f500-40f9-866f-0a669968c7d5.png)

### 4. Günlük ortalama vaka sayısı.

![2022-11-19 (7)](https://user-images.githubusercontent.com/83637039/202857117-a614fba9-8906-4d80-818c-345b69e522cb.png)

### 5. 65 yaşından büyük vakaların toplamı.
```
aged_65_sum = df["aged_65_older"].sum()+ df["aged_70_older"].sum() 
print(f" 65 yaşından büyük vakaların toplamı : {aged_65_sum} ")
```
 65 yaşından büyük vakaların toplamı : 2676555.0030000005 
 
 
 ## Veri Görselleştirmesi
 Verilerimizi inceledik şimdide bu incelediğimiz verilerin görselleştirmesine bakarak yorumlayalım.
 
### 
Bu görselleştirmede africa kıtasının oranın düşüklüğü saptadım. Bu düşüklüğün test sayısıyla ilgi bir bağlantısı var mı? diye merak ettim.
![test sayısı ile vaka oranı](https://user-images.githubusercontent.com/83637039/202858145-697f12b5-fe76-46bd-a9c9-a45ba01feca8.png)

 


