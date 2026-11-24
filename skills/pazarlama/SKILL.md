---
name: pazarlama
description: Pazarlama ve sosyal medya yönlendiricisi. /pazarlama yazınca hedef kitle, rakip, içerik, ses, LinkedIn gönderisi, görsel, video ve dağıtım skill'lerini tek tabloda gösterir; seçilene göre doğru skill'i devreye alır.
---

# /pazarlama — Pazarlama ve sosyal medya yönlendiricisi

Bu skill bir **yönlendiricidir**: kendi başına içerik üretmez, ihtiyaca uyan skill'i seçer ve onu çalıştırır.
Kullanıcıyla kullanıcının dilinde konuş (Türkçe yazdıysa Türkçe).

## 1. Girdi boşsa tabloyu göster ve sor

"Hangisiyle başlayalım, hangi marka ya da hesap için?" diye sor. Girdi doluysa tablodan en uygun **1 ana + en fazla 1 yardımcı**
skill seç, tek satır gerekçe yaz ve başla. Skill kurulu değilse "Kurulum" bölümündeki komutu kullanıcıya göster, kendin kurma.

### Araştırma ve strateji
| Skill | Ne zaman | İşi |
|---|---|---|
| `product-marketing` | Hedef kitle, konumlandırma | İlk adım: `.agents/product-marketing.md` bağlam belgesi (kitle, dertler, rakipler, mesaj); diğer skill'ler bunu okur |
| `understand-customers` | Müşteri dertleri, itirazlar | Alıcı psikolojisi brifingi, müşterinin kendi kelimeleri |
| `customer-journey` | Google, ChatGPT, sosyal medyada nasıl bulunuyoruz? | Farkındalıktan seçime yol haritası, sorulacak sorular |
| `competitor-analysis` | Şu rakibi incele | Rakibin içerik temaları ve boşlukları |
| `social-content` | Sosyal medya stratejisi, içerik takvimi | LinkedIn, Instagram, TikTok, X için strateji, takvim, kısa video senaryosu |
| `content-strategy` | Hangi konularda içerik üretelim | İçerik sütunları, konu kümeleri, yol haritası |
| `marketing-psychology` | Sosyal kanıt, kıtlık, çapa | Davranış bilimini kancalara ve gönderilere uygular |
| `launch` | Duyuru, lansman | Kanal ve zaman planı |
| `content-matrix` | LinkedIn için içerik fikirleri | Sütunlar × 8 format: 24–40 gönderi fikri tablosu |

### Ses ve profil
| Skill | Ne zaman | İşi |
|---|---|---|
| `voice-builder` | Benim sesimi çıkar | Kısa röportaj + 3–5 örnek yazıdan kişisel ses profili; gönderi skill'leri bunu okur |
| `newsletter-voice` | voice-builder sonrası, bülten için | Bülten yazım talimatları dosyası |
| `profile-optimizer` | LinkedIn profilimi baştan kur | Başlık, hakkında, deneyim, öne çıkanlar önerileri |

### Gönderi üretimi (LinkedIn ağırlıklı)
| Skill | Ne zaman | İşi |
|---|---|---|
| `post-writer` | Gönderi yaz | Kişinin sesine göre LinkedIn gönderisi |
| `post-formatter` | PAS / AIDA / BAB ile yaz | Çerçeveye oturtulmuş, mobil biçimli gönderi |
| `hook-generator` | Kanca, açılış cümlesi | 6 kanca varyasyonu |
| `quote-post` | Alıntı gönderisi | Kısa özgün alıntılar + görsel promptu |
| `pinned-comment` | Sabit yorum | Gönderi altı sabit yorum + görsel promptu |
| `post-scorer` | Bu gönderiyi puanla | Geçmiş performansla puanlama (geçmiş veri için ücretli Apify ister; yalnızca kullanıcı açıkça isterse) |

### Metin
| Skill | Ne zaman | İşi |
|---|---|---|
| `copywriting` | Başlık, vaat, çağrı yaz | İkna edici metin |
| `copy-editing` | Var olan metni toparla | Sıkılaştırma, düzeltme |

### Görsel
| Skill | Ne zaman | İşi |
|---|---|---|
| `graphic-designer` | Gönderiye görsel | HTML/CSS grafik ya da yapay zekâ infografiği seçer |
| `gemini-carousel` | Carousel | Slayt slayt marka uyumlu carousel promptları |
| `gemini-infographic` | Beyaz tahta infografik | El çizimi infografik promptu |
| `banner-design` | Kapak, banner | Sosyal medya, reklam ve kapak görselleri |

### Video
| Skill | Ne zaman | İşi |
|---|---|---|
| `watch` / `video-understand` | Bir video linki | Kareleri ve dökümü çıkarıp videoyu anlatır |
| `reels-scripting` | Şu Reel'den kendi Reel'imi yaz | Referans Reel → kendi senaryon |
| `youtube-seo` | YouTube başlık, açıklama | Başlık seçenekleri, zaman damgalı bölümler, eşlik eden gönderiler |
| `derin-ads-hook-generator` | Reklam için video linki | Videodan Meta reklam başlığı ve metni |

### Dağıtım
| Skill | Ne zaman | İşi |
|---|---|---|
| `parasite-and-pr` | Basın bülteni, LinkedIn makalesi | Üçüncü taraf yayın paketi |

## 2. Seçimden sonra

- Araştırmaysa önce `.agents/product-marketing.md` var mı bak; yoksa `product-marketing` ile başla.
- Gönderi üretimiyse kişinin ses dosyası var mı bak; yoksa `voice-builder` öner.
- Paylaşım hazırlıyorsan yayınlama: taslağı göster, yayın kararı kullanıcınındır.

## Kurulum (eksik skill varsa kullanıcıya göster)

```
npx skills add enisakarsu/pazarlama-skill -g   # yönlendirici + paketteki 16 skill
npx skills add hsynozdamar-byte/claude-skills-edited -g -s product-marketing marketing-psychology launch copywriting copy-editing
npx skills add coreyhaines31/marketingskills -g -s social-content content-strategy
npx skills add Illyism/seo-skills -g -s understand-customers customer-journey youtube-seo parasite-and-pr
npx skills add every-app/open-seo -g -s competitor-analysis
npx skills add bradautomates/claude-video -g
npx skills add enisakarsu/derin-ads-hook-generator -g
```
