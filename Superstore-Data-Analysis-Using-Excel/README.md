
# Excel ile Mağaza Satış Verisi Analizi 

Bu projede ABD'de bulunan küçük bir parekende mağazasının satışlarını inceleyeceğiz.
Amacımız veri setini analiz ederek mağazanın kârını artırmasına ve büyümesine 
yardım edebilecek çıkarımlar yapmaktır.

Veri seti, ABD'nin 49 eyaletinde 500'ün üzerinde şehre yapılan satışların "ship mode, customer segment, 
product category, sub-category, sales, quantity, discount, profit" bilgilerini göstermektedir.

Veri seti: https://www.kaggle.com/datasets/bravehart101/sample-supermarket-dataset

#### Keşifsel Veri Analizi Temel Soruları
- Satış adedi, gelir ve kâr bilgilerine göre en iyi olan kategoriler hangileri?
- Gelir ve kâr bilgilerine göre en iyi olan alt kategoriler hangileri?
- En fazla kullanılan teslimat yöntemi hangisi?
- En kârlı müşteri segmenti hangisi?
- Gelir ve kâr bilgilerine göre en iyi eyaletler hangileri?


## Veriyi Hazırlama
Veri seti zaten temizlenmiş bu yüzden bu aşamada sadece "country" kolonunu siliyorum tüm satışlar 
ABD'de olduğu için. Veride aynı satırlar var ancak silme gereği duymadım çünkü satışları birbirinden 
ayıracak satış_id gibi bir kolon yok yani benzer satın alımlar yapılmış olabilir.

---

## Kişifsel Veri Analizi

#### Satış adedi, gelir ve kâr bilgilerine göre en iyi olan kategoriler hangileri?

![img1](img/quantity-sales-profit-by-category.png)

Verimiz bize en fazla miktarda satışın belirgin farkla ofis ürünlerinde yapıldığını, 
en fazla gelirin teknoloji ürünlerinden elde edildiğini ve en fazla kârın yine teknoloji 
ürünlerinden elde edildiğini gösteriyor. Ancak burada mobilya ürünlerinden
yüksek gelir elde edilmesine rağmen edilen kârın çok az olduğunu görüyoruz.

Verinin grafikle gösterimi.

![img2](img/quantity-sales-profit-by-category-chart.png)

---

#### Gelir ve kâr bilgilerine göre en iyi olan alt kategoriler hangileri?

![img3](img/quantity-sales-profit-by-subcategory.png)

Alt kategorilere göre miktar, gelir ve kâra baktığımızda dikkat çeken nokta 3 alt kategorinin 
zarar etmekte olduğunu görüyoruz. Özellikle masa alt kategorisi çok fazla zarar ediyor.
Bir diğer nokta teknolojinin alt kategorisi copier en az satış yapılan kategori olmasına reğmen
en fazla kâr eden kategori konumunda.

Verinin grafikle gösterimi.

![img4](img/sales-by-subcategory.png)

![img5](img/profit-by-subcategory.png)

### En fazla kullanılan teslimat yöntemi hangisi?

![img6](img/ship-mode.png)

Teslimat yöntemi olarak standart teslimatın 60% oranında, aynı gün teslimatın ise 
5% oranında kullanıldığını görüyoruz. Teslimat fiyatlarını bilmiyoruz ancak 
muhtemelen en ucuz seçenek standart teslimattır. Aynı gün teslimat ise ekstra pahalıdır bu yüzden
çok az tercih edilmektedir.

Verinin grafikte gösterimi.

![img7](img/ship-mode-chart.png)

