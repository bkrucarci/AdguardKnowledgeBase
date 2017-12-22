---
title: 'AdGuard Filtre Politikası'
taxonomy:
    category:
        - docs
visible: true
---

AdGuard reklam filtrelerini tartışırken, anlaşmazlıkların ortaya çıktığı durumlar var – AdGuard bu reklamı mı yoksa o reklamı mı engellemeli. Kurallarımızı bir çerçevede özel kriterlere bağlı tutarız. Şimdi onları açıklama zamanı geldi. Kriterlerimiz, bizimde uygun ve doğru bulduğumuz [EasyList Politikası](https://easylist.to/pages/policy.html) ile çok benzerdir. Bununla birlikte, bazı noktalarda değişiklikler yaptık.

![](https://vgy.me/Th5m2e.png)


## Reklam filtreleri

Bunlar aslında dil filtreleridir: Rusça, İngilizce, Almanca, Flemenkçe, İspanyolca, Portekizce, Japonca.

##### Bu filtreler neyi engelliyor?

- Filtreler reklamları mümkün olan her yerde engelleyecektir. 
- Reklamlar, reklamın amaç ve nedenlerine bakılmaksızın engellenir.
- Zararlı yazılımların ya da eklentilerin ortaya çıkardığı reklamları engelleyeceğiz. Bunu, yalnızca bu uygulamanın veya eklentinin nasıl kurulacağını belirteceğiniz koşullarla gerçekleştirdiğimizi lütfen unutmayın.

##### Kısıtlamalar ve İstisnalar

Bir kural aşağıda açıklanan kısıtlamalara uyarsa ana filtrelere eklenmez.

- Websitelerinin öz reklamları kasıtla engellenmez. Diğer taraftan engellemeyi kaldırmamalısınız, çünkü bu engellemenin kaldırılması üçüncü taraf reklamlarının görüntülenmesine neden olabilir.
- Belli sitelere özgü kurallar, eğer o siteye yeteri kadar tıklanma (trafik) varsa eklenir.  
 Trafik, açık istatistikler (varsa) veya diğer yollarla belirlenir.  
 Sitenin trafiği, ayda 30 bin ziyaretçisi olduğunda yeterli sayılır.
- Reklam engelleyiciyi önleyen komutlar, yalnızca sitenin işlevselliğini sınırlarlarsa veya
  kullanımına engellenirse filtreye eklenir.
- Bazı sitelerin işleyişi ile ilgili sürekli sorunlara neden olan kurallar kaldırılır.


## Casus Engelleme filtresi

##### Bu filtre ile ne engellenecek?

- Bu filtre, kullanıcıların kişisel verilerini toplayan tüm sayaçları engelleyecektir.

##### Kısıtlamalar ve İstisnalar

Bir kural aşağıda açıklanan kısıtlamalara uyarsa bu filtreye eklenmez.

- Sitelerin işleyişi ile ilgili sorunlara neden olan kurallar kaldırılır.
- Belli sitelere özgü kurallar, eğer o siteye yeteri kadar tıklanma (trafik) varsa eklenir.  
 Trafik, açık istatistikler (varsa) veya diğer yollarla belirlenir.  
 Sitenin trafiği, ayda 30 bin ziyaretçisi olduğunda yeterli sayılır.


## Sosyal Medya filtresi

##### Bu filtre ile ne engellenmelidir?

- Filtre (üçüncü parti sitelerde bulunan) “Beğen” ve “Paylaş” butonları gibi sosyal medya araçlarını engellemelidir.

##### Kısıtlamalar ve İstisnalar

Bir kural aşağıda açıklanan kısıtlamalara uyarsa bu filtreye eklenmez.

- Sitenin işleyişinde kullanılan, sitenin bir parçası olan araçlar engellenmez.  
 “Yorumlar”, “Gömülü Gönderiler”, “Anketler” gibi araçlar ya da sosyal ağlar aracılığıyla yetkilendirme yapanlar.
- Sitelerin kendi sosyal medya hesaplarını açan bağlantılar engellenmez.
- Sitelerin işleyişi ile ilgili sorunlara neden olan kurallar kaldırılır.
- Belli sitelere özgü kurallar, eğer o siteye yeteri kadar tıklanma (trafik) varsa eklenir.  
 Trafik, açık istatistikler (varsa) veya diğer yollarla belirlenir.  
 Sitenin trafiği, ayda 30 bin ziyaretçisi olduğunda yeterli sayılır.


## Filtre kuralları için kalite gereksinimleri

- Kurallar performans açısından olabildiğince verimli olmalıdır.
- İstisna kuralları, reklamları kaçırmadan engellemeye devam etmek için mümkün olduğunca özelleştirilmelidir.
- CSS ve JS enjeksiyon kuralları mümkün olduğunca az ve sadece onlar olmadan reklam engelleme imkansız olduğunda kullanılacaktır.
