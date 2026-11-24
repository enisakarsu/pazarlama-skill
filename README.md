# /pazarlama — Claude Code için pazarlama ve sosyal medya skill paketi

Enis Akarsu'nun günlük kullandığı pazarlama skill'leri tek bir komutta toplandı.
`/pazarlama` yazınca tüm liste önüne gelir; ihtiyacın olanı seçip tetiklersin.

## Kurulum

Claude Code'a şu promptu yapıştır:

```
github.com/enisakarsu/pazarlama-skill adresindeki /pazarlama paketini global olarak kur.
Şu komutu çalıştır: npx skills add enisakarsu/pazarlama-skill -g
Ardından skills/pazarlama/SKILL.md dosyasının "Kurulum" bölümündeki dış kaynaklı skill'lerin hepsini global olarak kur ve kurulanları liste halinde göster.
```
Ya da elle:

```
npx skills add enisakarsu/pazarlama-skill -g
```

Bu komut yönlendiriciyi ve paketin içindeki 16 skill'i kurar. Dış kaynaklı skill'ler için `skills/pazarlama/SKILL.md` içindeki "Kurulum" komutlarını çalıştır.

## İçindekiler

`/pazarlama` yazınca bu liste önüne gelir. İhtiyacın olanı seç ya da derdini kendi cümlenle yaz; doğru skill devreye girer.

### Araştırma ve strateji
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `product-marketing` | "Hedef kitlemi çıkaralım" | İşini, müşterini ve rakiplerini tek bir tanıtım dosyasına yazar. Diğer skill'ler bu dosyayı okuyup ona göre çalışır, her seferinde baştan anlatmazsın. | Kafe sahibisin: "Müşterim kim, neden bana geliyor?" diye sorar, cevaplarından bir sayfalık özet çıkarır. |
| `understand-customers` | "Müşterim neden almıyor?" | Müşterinin derdini, çekincelerini ve kullandığı kelimeleri ortaya koyar. | Online kurs satıyorsun: "Pahalı", "vaktim yok" gibi itirazları ve her birine verilecek cevabı listeler. |
| `customer-journey` | "İnsanlar beni nasıl buluyor?" | Müşterinin seni ilk duymasından satın almasına kadar hangi adımlardan geçtiğini çizer; Google, ChatGPT ve sosyal medyada nerede görünmen gerektiğini söyler. | Diş kliniği: "Önce Google'da 'implant fiyatı' arar, sonra Instagram yorumlarına bakar" gibi bir yol haritası çıkarır. |
| `competitor-analysis` | "Şu rakibi incele" | Rakibin hangi konularda içerik ürettiğini ve senin boş kalan alanlarını gösterir. | Rakip mobilyacının sitesini verirsin; "Onlar bakım rehberi yazmamış, sen yaz" der. |
| `social-content` | "Ne paylaşayım?" | Platforma göre içerik planı ve paylaşım takvimi hazırlar, kısa video senaryosu da yazar. | Butik otel için bir aylık Instagram ve LinkedIn takvimi: hangi gün, ne paylaşılacak. |
| `content-strategy` | "Hangi konularda içerik üretelim?" | İçerik ana başlıklarını ve konu gruplarını belirler, uzun vadeli yol haritası çıkarır. | Muhasebe bürosu: "Vergi takvimi", "şirket kurma", "e-fatura" diye üç ana başlık ve altlarında 20 konu. |
| `marketing-psychology` | "İnsanları nasıl ikna ederim?" | Sosyal kanıt, kıtlık gibi ikna ilkelerini gönderine ve teklifine uygular. | "Son 3 kontenjan" ya da "200 işletme kullanıyor" gibi ifadeleri doğru ve dürüst yerde kullanmayı önerir. |
| `launch` | "Yeni ürün çıkarıyorum" | Duyurunun hangi kanalda, hangi gün, hangi sırayla yapılacağını planlar. | Yeni menü lansmanı: 1 hafta önce merak uyandıran gönderi, açılış günü video, ertesi gün müşteri yorumları. |
| `content-matrix` | "LinkedIn için fikir lazım" | Ana konularını 8 farklı gönderi biçimiyle eşleyip 24–40 hazır fikir tablosu çıkarır. | "Liderlik" konusu için hikâye, liste, karşılaştırma, soru gibi biçimlerde 8 ayrı gönderi fikri. |

### Ses ve profil
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `voice-builder` | "Benim gibi yazsın" | Birkaç soru sorar, eski yazılarını okur ve senin yazma tarzını bir dosyaya çıkarır. Sonraki gönderiler senin ağzından çıkmış gibi olur. | 3 eski LinkedIn gönderini verirsin; kısa cümle, esprili kapanış gibi alışkanlıklarını yakalar. |
| `newsletter-voice` | "E-bülten yazacağım" | Senin tarzına göre bülten yazma kuralları hazırlar. | Haftalık müşteri bülteni için "selamlama, 3 haber, tek çağrı" kalıbını senin dilinle kurar. |
| `profile-optimizer` | "LinkedIn profilimi düzelt" | Başlık, hakkında ve deneyim bölümlerini yeniden yazar. | "Satış Müdürü" yerine "B2B şirketlere 6 ayda yeni pazar açan satış lideri" gibi bir başlık önerir. |

### Gönderi üretimi
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `post-writer` | "Gönderi yaz" | Konuyu verirsin, senin tarzınla LinkedIn gönderisi yazar. | "Bugün ilk çalışanımı işe aldım" deyince bunu anlatan hazır bir gönderi çıkarır. |
| `post-formatter` | "Şu kalıpla yaz" | Gönderiyi bilinen ikna kalıplarına (sorun-çözüm, önce-sonra gibi) oturtur, telefonda rahat okunacak şekilde böler. | "Eskiden Excel'le uğraşıyorduk, şimdi 10 dakikada bitiyor" diye önce-sonra kurgusuyla yazar. |
| `hook-generator` | "Dikkat çekici bir giriş lazım" | Gönderinin ilk iki satırı için 6 farklı açılış önerir. | "Müşterilerimin yarısını kaybettim. Sebebi fiyat değildi." gibi açılışlar. |
| `quote-post` | "Alıntı paylaşmak istiyorum" | Kısa, akılda kalan cümleler ve bunlar için görsel tarifi hazırlar. | "Plan yapmayan işletme, başkasının planının parçası olur." ve yanına sade bir görsel önerisi. |
| `pinned-comment` | "Gönderinin altına sabit yorum" | Gönderinin altına iliştirilecek, linki ya da çağrıyı taşıyan yorumu yazar. | "Ücretsiz kontrol listesini buradan indirebilirsiniz 👇" gibi bir yorum. |
| `post-scorer` | "Bu gönderi tutar mı?" | Gönderiyi 5 ölçüte göre puanlar, eski gönderilerinle karşılaştırır. (Eski gönderileri çekmek için ücretli Apify hesabı ister.) | "Açılış güçlü 8/10, çağrı zayıf 4/10, sona bir soru ekle." |

### Metin
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `copywriting` | "Satış metni yaz" | Web sayfası, ilan ya da broşür için ikna edici metin yazar. | Kuaför sitesinin ana sayfası için başlık, kısa açıklama ve "Randevu al" butonu metni. |
| `copy-editing` | "Bu metni toparla" | Var olan metni kısaltır, netleştirir, hatalarını düzeltir. | 300 kelimelik dağınık "Hakkımızda" yazısını 120 kelimelik akıcı bir metne çevirir. |

### Görsel
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `graphic-designer` | "Gönderiye görsel lazım" | Gönderine uygun görseli seçer ve hazırlar: tablo, kart ya da infografik. | "3 adımda e-fatura" gönderisine üç kutulu, markana uygun bir görsel. |
| `gemini-carousel` | "Kaydırmalı gönderi yap" | Tek bir konudan slayt slayt kaydırmalı gönderi (carousel) çıkarır. | "Yeni başlayanlar için 7 bütçe hatası" konusunu 7 slayta böler, her slaytın metnini ve görselini hazırlar. |
| `gemini-infographic` | "Elle çizilmiş gibi bilgi görseli" | Yazını beyaz tahtaya çizilmiş gibi duran bir bilgi görseline çevirir. | Blog yazındaki 5 maddeyi oklarla bağlı, el çizimi bir şemaya dönüştürür. |
| `banner-design` | "Kapak görseli lazım" | Sosyal medya kapağı, reklam ve afiş görselleri tasarlar. | LinkedIn kapak fotoğrafın ya da indirim kampanyası afişi. |

### Video
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `watch` / `video-understand` | Bir video linki verince | Claude videoyu izler: görüntüleri ve konuşmaları çıkarıp ne anlatıldığını özetler, sorularını cevaplar. | Rakibin 10 dakikalık YouTube videosunun linkini verirsin; "Ana mesajı ne, hangi teklifi yapıyor?" sorusunu cevaplar. |
| `reels-scripting` | "Şu Reel gibi bir video çekmek istiyorum" | Beğendiğin bir Reel'i inceler, aynı kurguyla senin işine uygun yeni bir senaryo yazar. | Viral bir kahve Reel'ini verirsin; senin pastanen için sahne sahne çekim senaryosu çıkarır. |
| `youtube-seo` | "YouTube videom bulunsun" | Video için başlık seçenekleri, açıklama ve bölüm zamanlarını yazar. | "Evde ekmek yapımı" videona 5 başlık önerisi ve "0:45 Hamur hazırlama" gibi bölümler. |
| `derin-ads-hook-generator` | Reklam için video linki verince | Önce siteni tanır, sonra videoyu izleyip Meta (Instagram, Facebook) reklamı için başlık ve metin yazar. | Ürün tanıtım videonun linkini verirsin; 5 farklı reklam başlığı ve metni hazırlar. |

### Dağıtım
| Skill | Ne zaman tetiklenir | Ne işe yarar | Örnek |
|---|---|---|---|
| `parasite-and-pr` | "Başka sitelerde de görüneyim" | Basın bülteni, LinkedIn makalesi gibi başka platformlarda yayınlanacak içerik paketi hazırlar. | Yeni şubeni duyuran bir basın bülteni ve aynı haberin LinkedIn makalesi versiyonu. |

## Kaynaklar

Pakette 30 skill var: 16'sı bu depoda (`skills/`), diğerleri kendi depolarından kurulur ve hakları sahiplerine aittir:

- [hsynozdamar-byte/claude-skills-edited](https://github.com/hsynozdamar-byte/claude-skills-edited)
- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
- [Illyism/seo-skills](https://github.com/Illyism/seo-skills)
- [every-app/open-seo](https://github.com/every-app/open-seo)
- [bradautomates/claude-video](https://github.com/bradautomates/claude-video)
- [enisakarsu/derin-ads-hook-generator](https://github.com/enisakarsu/derin-ads-hook-generator)

Daha fazlası: [enisakarsu.com](https://enisakarsu.com)

## Lisans

Bu depodaki skill'ler MIT lisanslıdır. Dış kaynaklı skill'ler kendi lisanslarına tabidir.
