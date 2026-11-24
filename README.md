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

`/pazarlama` yazınca bu liste önüne gelir. Tabloda her skill'in hangi istekle tetiklendiği ve ne iş yaptığı yazıyor.

### Araştırma ve strateji
| Skill | Ne zaman tetiklenir | Ne işe yarar |
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
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `voice-builder` | Benim sesimi çıkar | Kısa röportaj + 3–5 örnek yazıdan kişisel ses profili; gönderi skill'leri bunu okur |
| `newsletter-voice` | voice-builder sonrası, bülten için | Bülten yazım talimatları dosyası |
| `profile-optimizer` | LinkedIn profilimi baştan kur | Başlık, hakkında, deneyim, öne çıkanlar önerileri |

### Gönderi üretimi (LinkedIn ağırlıklı)
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `post-writer` | Gönderi yaz | Kişinin sesine göre LinkedIn gönderisi |
| `post-formatter` | PAS / AIDA / BAB ile yaz | Çerçeveye oturtulmuş, mobil biçimli gönderi |
| `hook-generator` | Kanca, açılış cümlesi | 6 kanca varyasyonu |
| `quote-post` | Alıntı gönderisi | Kısa özgün alıntılar + görsel promptu |
| `pinned-comment` | Sabit yorum | Gönderi altı sabit yorum + görsel promptu |
| `post-scorer` | Bu gönderiyi puanla | Geçmiş performansla puanlama (geçmiş veri için ücretli Apify ister; yalnızca kullanıcı açıkça isterse) |

### Metin
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `copywriting` | Başlık, vaat, çağrı yaz | İkna edici metin |
| `copy-editing` | Var olan metni toparla | Sıkılaştırma, düzeltme |

### Görsel
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `graphic-designer` | Gönderiye görsel | HTML/CSS grafik ya da yapay zekâ infografiği seçer |
| `gemini-carousel` | Carousel | Slayt slayt marka uyumlu carousel promptları |
| `gemini-infographic` | Beyaz tahta infografik | El çizimi infografik promptu |
| `banner-design` | Kapak, banner | Sosyal medya, reklam ve kapak görselleri |

### Video
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `watch` / `video-understand` | Bir video linki | Kareleri ve dökümü çıkarıp videoyu anlatır |
| `reels-scripting` | Şu Reel'den kendi Reel'imi yaz | Referans Reel → kendi senaryon |
| `youtube-seo` | YouTube başlık, açıklama | Başlık seçenekleri, zaman damgalı bölümler, eşlik eden gönderiler |
| `derin-ads-hook-generator` | Reklam için video linki | Videodan Meta reklam başlığı ve metni |

### Dağıtım
| Skill | Ne zaman tetiklenir | Ne işe yarar |
|---|---|---|
| `parasite-and-pr` | Basın bülteni, LinkedIn makalesi | Üçüncü taraf yayın paketi |

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
