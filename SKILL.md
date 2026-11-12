---
name: instagram-aciklama-carousel-metni
description: "Instagram açıklaması (caption), hashtag, alt metin ve 1080x1350 carousel slayt metinlerini yazar ve kurallara göre denetler. Caption yaz, carousel yap, slayt, hashtag istendiğinde kullan."
---

# Instagram Caption ve Carousel

Python linter yerine aşağıdaki kontrol listesini Claude kendisi uygular ve sayıları gösterir. Hiçbir şey paylaşılmaz; kullanıcı yapıştırır. Taslakları göstermeden önce `sosyal-medya-metni-insanlastirma` kuruluysa ondan geçir. Renk ve font için bir marka stil dosyası varsa onu kullan, palet uydurma.

## Caption

### Önce görevi seç (atlanırsa caption bozulur)

- **Görev A: Video zaten kancaladı.** Reels'in kancası ilk iki saniyede. Caption ikinci kanca değildir; işi tek çağrı, o çağrıyı anlamlı kılan bağlam ve aranan kelimeler.
- **Görev B: Caption içeriğin kendisi.** Fotoğraf, carousel. Birinci satır kancadır; somut, kısa, cümlenin ortasında değil bir uçurumda kesilir.
Hangisini yazdığını söyle.

### Şekil

```
Satır 1   Akışta "...devamı"ndan önce görünen ilk ~125 karakter. A: çağrı, sade. B: kanca.
          Asla selamlama, hashtag veya ilk karakter olarak emoji değil.
Gövde     2–6 kısa paragraf, aralarında boş satır. Arama terimleri burada.
Çağrı     Tek bir tane: kaydet, paylaş, bir anahtar kelime yorumla veya takip et.
Hashtag   En fazla 5, en altta ayrı satırda, ya da hiç.
```
Sınır 2.200 karakter; neredeyse hiçbir şey buna ihtiyaç duymaz. 600 karakter teslim eden caption, 1.800 karakterlikten iyidir.

### Hashtag gerçeği

Instagram 18–19 Aralık 2025'te gönderi ve Reels başına hashtag'i 30'dan 5'e indirdi; Adam Mosseri spesifik etiketlerin uzun listelerden iyi çalıştığını söyledi: hashtag erişim kolu değil, etikettir. En fazla 5, spesifik, konu etiketi olarak. Sınır gönderinin tamamı için geçerli; ilk yoruma ek etiket koymak çözüm değil. #viral, #keşfet, #explore, #fyp hiçbir şey anlatmaz, çıkar.

### Arama terimleri hashtag'den önemli

Instagram araması caption metnini okur. Bulunmak istenen ifadeyi (ör. "aile şirketi", "kurucu hikayesi", "marka stratejisi") bir insanın yazacağı şekilde normal bir cümlenin içinde kullan. Kullanıcıdan 2–3 terim al ya da öner.

### Kurallar

- Caption'da link yok (tıklanmaz). Bio, story linki veya DM.
- Tek çağrı. İki çağrı hiç çağrı yokla aynıdır.
- Anahtar kelime çağrısı: tek kelime, boşluksuz, emojisiz, yazması kolay ("HİKAYE yaz"), videoda da söylenir.
- Link gerekiyorsa ilk yorumu ayrı yaz.
- Emoji noktalama gibi, süs gibi değil: 100 karakterde 4'ten fazla olmasın.
- Kaynak: hikayedeki rakam ve tarihler için gövdenin sonunda kısa "Kaynak:" satırı. Doğrulanmamış bilgiyi yazma.
- Alt metin (alt text) carousel ve fotoğraflar için 20 saniyeye değer; yaz.

### Kontrol ve makbuz

Taslaktan sonra bu kontrolleri sayılarıyla göster, her BAŞARISIZ'ı düzelt, her UYARI'ya açıkça karar ver:
```
CAPTION HAZIR
görev:       A - kancayı reel taşıyor
görünen:     125 karakterin 118'i kesimden önce kullanıldı
çağrı:       1 (kaydet)
hashtag:     3
arama:       "aile şirketi" 3. satırda, "marka hikayesi" 5. satırda
link:        yok
emoji:       100 karakterde 1,2
```
Ardından kopyalanmaya hazır caption bloğunu ver.

## Carousel

Carousel ızgaradaki en yüksek bekleme süreli formattır (kaydırma bir etkileşimdir). Instagram etkileşmeyen kişiye carousel'i sonraki bir slayttan tekrar gösterebilir; bu yüzden 2. slayt da tek başına ayakta durmalı.

**Ne zaman carousel:** fikir sıralı ve yeniden okunmayı gerektiriyorsa (adımlar, parçalı çerçeve, önce/sonra, ekran görüntüsü alınacak liste, zaman çizelgesi). Hareket, yüz veya görülmesi gereken bir ödül varsa Reels. Fikir tek iddiaysa ikisi de değil; Reels'e çevir ve söyle.

### Yapı (6–10 slayt; 5'in altında kaydırma başlamaz)
```
1         KAPAK      kanca, 6 kelime veya az, küçük resimde okunacak boyut + altında tek satır vaat
2         KAZANÇ     neden önemli, tek cümle. Bu ikinci kapaktır, kurulum olamaz
3..N      HER SLAYTA BİR FİKİR: 3–7 kelimelik başlık + en fazla 25 kelime
N+1       ÖZET       her şey liste halinde. Ekran görüntüsü alınan ve gönderilen slayt
SON       ÇAĞRI      tek eylem: kaydet, paylaş, takip et
```
Hikaye carousel'i (vaka, şirket hikayesi) için tipik ark: kapak (sonuç veya ters köşe) → bağlam (yıl, kişi, yer) → 3–5 dönüm noktası (ama/bu yüzden) → sonuç rakamı → ders/özet → çağrı.

### Slayt kuralları

- Kapak sonucun %80'idir. Altı kelime, büyük.
- Boyut 1080x1350 (4:5), JPEG/PNG, en fazla 20 öğe. Kapak yazısını her kenardan 120 px içeride tut; profil ızgarası kırpması önemsizleşir.
- Slaytları numarala (3/8); sonu görünce tamamlama artar.
- Hiçbir slayt paragraf değildir; 25 kelimeye sığmıyorsa iki slayttır.
- Her slaytta küçük köşe handle'ı; ekran görüntüleri sensiz dolaşır.
- Tek vurgu rengi, 32 px'ten küçük yazı yok (telefonda gerçek boyutun üçte biri okunur).
- Gerçek kişi/şirket görseli kullanılacaksa telif ve kaynağı not et.

### Dosyaları üretme

Önce slayt metnini numaralı liste olarak ver; kullanıcı 10 saniyede okuyup düzenleyebilsin. Onaydan sonra üret: Canva bağlıysa Canva'da, değilse her slaytı 1080x1350 bir `<section>` olarak HTML'de yazıp PNG'ye çevir (`instagram-carousel-design-system` bunu kalıcı marka spesifikasyonuyla yapar). Carousel caption'ı Görev B'dir (kapak altı kelimesini zaten harcadı).

Çıktı örneği:
```
CAROUSEL · 8 slayt
1 KAPAK   5.126 KEZ BAŞARISIZ
          Dyson'ın elektrik süpürgesi hikayesi.
2 KAZANÇ  Bugün herkesin bildiği bir marka. Yıllarca tek bir ürün satamadı.
...
7 ÖZET    Beş dersin hepsi, sırayla.
8 ÇAĞRI   Kaydet; bir sonraki fikrin tıkandığında aç.
Caption: Görev B, kanca 1. satırda, tek çağrı, 3 etiket.
```

Kaynak: github.com/Jakeschincariol/instagram-agent-skill (MIT) içindeki ig-caption ve ig-carousel skill'lerinden uyarlanmıştır.