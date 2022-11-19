# **SistersLab Women in Tech Academy Bitirme Projesi**

![covid-19-asisinin-dna-yi-degistirdigine-yonelik-iddialar](https://user-images.githubusercontent.com/83637039/202847597-924205aa-d55a-401e-9afd-ef082535e00e.jpg)

## Veri Seti Yorumlaması

Verimde neyi inceleyebilirim?

Bu veri seti içerisinde; covid-19 salgını ile ilgili :Kıtalar ve ülkeler bazında günlük vaka, günlük ölüm, günlük test sayısı, aşılma sayısı gibi veriler vardır.
Bunlardan çıkartabileceğimiz analizlere bakalım.


Nelere bakılması gerekiyor

1. Ülkelere göre günlük vaka sayısı.
2. Ülkelere göre ortalama vaka sayısı.
3. Ülkelere göre toplam aşılama sayısı.
4. Günlük ortalama vaka sayısı.
5. 65 yaşından büyük vakaların toplamı.

Verimiz çeşitli pandas kodlarıyla verimi inceledim.

Veri sütünlardaki null değerleri, veri tiplerini, info

Öncelikle bize verilen veri setindeki sütünları, bu sütündaki eksik değerleri ve eksik değerlerin oranlarını inceledim.

![image](https://user-images.githubusercontent.com/83637039/202867288-9e9b0c9a-049b-474f-8617-10882f130bb2.png)

### 1. Ülkelere göre günlük vaka sayısı.

Tüm ülkeleri incelediğimde 'World'  diye bir satırlar olduğunu gördüm. Bu satırların ülke bazında yanlışlıklara yol açacağından satırları sildim.
Daha sonra ülke ve kıta bazında günlük vaka sayısını filtreledim.

![image](https://user-images.githubusercontent.com/83637039/202867338-55310e9c-edbe-4f5e-9199-2350833e3c20.png)

### 2. Ülkelere göre ortalama vaka sayısı.

![image](https://user-images.githubusercontent.com/83637039/202867361-51658356-7d78-4033-9af6-bcc5cc93a379.png)

### 3. Ülkelere göre toplam aşılama sayısı.

![image](https://user-images.githubusercontent.com/83637039/202867376-f9d6c79e-d49e-450c-8375-7ed0536550ce.png)

### 4. Günlük ortalama vaka sayısı.

![image](https://user-images.githubusercontent.com/83637039/202867391-11181d38-8a98-48fd-8ba3-66a242474d18.png)

### 5. 65 yaşından büyük vakaların toplamı.
```
aged_65_sum = df["aged_65_older"].sum()+ df["aged_70_older"].sum() 
print(f" 65 yaşından büyük vakaların toplamı : {aged_65_sum} ")
```
 65 yaşından büyük vakaların toplamı : 2676555.0030000005 
 
 
 ## Veri Görselleştirmesi
 Verilerimizi inceledik şimdide bu incelediğimiz verilerin görselleştirmesine bakarak yorumlayalım.
 
#### 1. Bu görselleştirmede önce test sayısıyla vakalar arasındaki ilişkiyi inceledim. Mesela africa kıtasının oranın düşüklüğü saptadım. Bu düşüklüğün test sayısıyla ilgi bir bağlantısı var mı diye karşılaştırdım.

![test sayısı ile vaka oranı](https://user-images.githubusercontent.com/83637039/202858145-697f12b5-fe76-46bd-a9c9-a45ba01feca8.png)

### 2. 'gdp_per_capita', 'extreme_poverty', 'diabetes_prevalence', 'female_smokers', 'male_smokers', 'handwashing_facilities', 'life_expectancy', 'human_development_index', 'population gibi verilerin bir biriyle ilişkisini korelasyon haritasında inceledim.

![corelasyon](https://user-images.githubusercontent.com/83637039/202862448-3e5bc85d-2677-4902-aa14-7c43971663af.png)

### 3. 65 yaş ve üstü vakaların 65 yaş altındaki vakalarına olan oranını inceledim. 

![65yaş](https://user-images.githubusercontent.com/83637039/202862543-efe1635c-b5f8-491a-a3d2-29d019405ff3.png)

### 4. Koronanın ilk çıktığı günden itibaren günlük vakalara göre görselleştirdim.

![outputvaka](https://user-images.githubusercontent.com/83637039/202862831-2279a0ab-1a1f-4f5f-bb28-5f07a70d40ff.png)

### 5. Kıtalara göre popülasyonun aşılanma oranına göre ilişkisini inceledim.

![aşılanma populasyon](https://user-images.githubusercontent.com/83637039/202862961-c3b8d68c-bf6d-4c77-8bcd-1d20a21e2763.png)

### 6. Korananın üreme oranını etkilemiş mi diye inceledim.

![üremeoranı](https://user-images.githubusercontent.com/83637039/202863013-2a0aa016-8a31-4887-8fb5-ead0ab2c1cfd.png)





 


