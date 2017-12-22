---
title: 'Reklam engelleme nasıl çalışır'
taxonomy:
    category:
        - docs
visible: true
---

*   [Açıklama](#introduction)
*   [Reklam engelleme](#filtering)
*   [Sayfa kod filtreleme](#html)
*   [İstek engelleme](#block)
*   [CSS Enjekte ve Javascript](#inject)
*   [Sayfaların sonradan işlenmesi](#cosmetic)
*   [Yardım etmek ister misiniz?](#report)

<a name="introduction"></a>

## Açıklama

AdGuard'ın temel işlevlerinden birisi, websitelerini reklamlardan arındırmaktır. Bu makalede, AdGuard'ın çevrimiçi reklamları nasıl filtrelediğini ayrıntılarıyla açıklayacağız.

Adguard'ın çalışması, içinde reklam engelleyen kuralların toplandığı, çeşitli reklam filtrelerinin kullanımına dayanır. AdGuard farklı reklam filtreleri kullanabilir. Bazı filtreler tarafımızdan oluşturulurken ([bu sayfada](/general/adguard-ad-filters.html) filtreler hakkında daha fazla bilgi edinebilirsiniz), bazı filtreler ise meraklıları tarafından oluşturuldu.



<a name="filtering"></a>

## Reklam engelleme

Reklam filtreleme mekanizması, hangi AdGuard ürününü kullandığınıza bağlıdır. Tarayıcı eklentileri, tarayıcıların kendilerine sağladığı yeteneklerle sınırlıdır. Windows, Mac ve Android için AdGuard tamamen farklı bir filtreleme algoritması kullanır ve tarayıcınızdan bağımsız olarak çalışır. Aşağıda, AdGuard'ın kullandığı reklam filtreleme yeteneklerini tüm aşamaları ile açıklıyoruz.



<a name="html"></a>

#### Sayfa kod filtreleme

Bir sayfa tarayıcıya yüklenmeden önce AdGuard; reklam kodu öğelerini, kod filtreleme kurallarına göre işler. Bu şekilde internet tarayıcısı, bu sayfada aslında bu öğelerin var olup olmadığını anlayamıyor ve bu kodları yüklemeye çalışmıyor.

![Adguard: Sayfa kod filtreleme](https://vgy.me/Th5m2e.png)

Sayfa kod filtreleme teknolojisi **yalnızca Windows, Mac ve Android için AdGuard (yüksek kaliteli filtreleme etkin ise)** üzerinde kullanılır. Bunun nedeni, tarayıcı uzantılarının yeteneklerinin sınırlı olması ve tarayıcı eklentilerinin sayfa kodunu filtreleyemeyecekleri gerçeğidir.



<a name="block"></a>

#### İstek engelleme

İnternet tarayıcısı, sayfaların kodunda tanımlanan tüm gerekli öğeleri başka bir sayfadan yükler. Filtreleme kurallarına dayanarak, AdGuard, afiş reklamları veya Flash nesneleri gibi reklamcılık öğelerinin yüklenmesini engelleyebilir.

![Adguard: İstekleri engelleme](https://vgy.me/bl9hk9.png)



<a name="inject"></a>

#### CSS Enjekte ve Javascript

Tüm reklamlar şimdiye kadar açıklanan 2 yöntemle engellenemeybilir. Örneğin, Javascript yardımıyla sayfaya dinamik olarak gömülmüş bir reklam örneği var ve engelleyebileceğimiz ek öğelerin yüklenmesini gerektirmiyor.

CSS, web sayfaları tasarımı için kullanılan özel bir dildir. Bir web sayfasındaki öğelerin görünümü kurallara göre ayarlanabilir. Görünüm demek renk, yazı tipi, sayfaya yerleşimi ve elementin görünürlüğü demektir. Ve bu, bizi ilgilendiriyor çünkü reklam afişlerini gizlemek istiyoruz. Javascript ayrıca sayfadaki herhangi bir öğeyi dinamik olarak değiştirmenize izin veren özel bir dildir.



<a name="cosmetic"></a>

#### Sayfaların sonradan işlenmesi

Bu, yalnızca tarayıcı eklentileri için geçerli bir yöntemdir. Bu gereklidir, çünkü ilk adımda filtrelemeyi (sayfa kodu filtrelemesi) eklentiler yapamaz. Sayfaların sonradan işlenmesi sırasında tarayıcı eklentisi, yüklenmesi engellenen tüm öğeleri sayfadan kaldırır. Eğer o oğeleri kaldırmazsak, örneğin bozulmuş şekilde "grafikler" gibi tam olarak yüklenmemiş sayfalar göreceksiniz.



<a name="report"></a>

## Yardım etmek ister misiniz?

Tüm reklam filtreleri, kullanıcılardan gelen reklamlarla ilgili şikayetler üzerine elle oluşturulmuştur. Programın kendisi aracılığıyla bize bir şikayet gönderebilirsiniz veya [Forum sayfamız](http://forum.adguard.com/forumdisplay.php?51-Filter-Rules) üzerinden bildirebilirsiniz.
