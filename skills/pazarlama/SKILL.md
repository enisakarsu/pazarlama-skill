---
name: pazarlama
description: Pazarlama ve sosyal medya yönlendiricisi. /pazarlama yazınca hedef kitle, rakip, içerik, gönderi, video ve dağıtım skill'lerini tek tabloda gösterir; seçilene göre doğru skill'i devreye alır.
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

### Metin
| Skill | Ne zaman | İşi |
|---|---|---|
| `copywriting` | Başlık, vaat, çağrı yaz | İkna edici metin |
| `copy-editing` | Var olan metni toparla | Sıkılaştırma, düzeltme |

### Video
| Skill | Ne zaman | İşi |
|---|---|---|
| `watch` | Bir video linki | Kareleri ve dökümü çıkarıp videoyu anlatır |
| `youtube-seo` | YouTube başlık, açıklama | Başlık seçenekleri, zaman damgalı bölümler, eşlik eden gönderiler |
| `derin-ads-hook-generator` | Reklam için video linki | Videodan Meta reklam başlığı ve metni |

### Dağıtım
| Skill | Ne zaman | İşi |
|---|---|---|
| `parasite-and-pr` | Basın bülteni, LinkedIn makalesi | Üçüncü taraf yayın paketi |

## 2. Seçimden sonra

- Araştırmaysa önce `.agents/product-marketing.md` var mı bak; yoksa `product-marketing` ile başla.
- Paylaşım hazırlıyorsan yayınlama: taslağı göster, yayın kararı kullanıcınındır.

## Kurulum (eksik skill varsa kullanıcıya göster)

```
npx skills add hsynozdamar-byte/claude-skills-edited -g -s product-marketing marketing-psychology launch copywriting copy-editing
npx skills add coreyhaines31/marketingskills -g -s social-content content-strategy
npx skills add Illyism/seo-skills -g -s understand-customers customer-journey youtube-seo parasite-and-pr
npx skills add every-app/open-seo -g -s competitor-analysis
npx skills add bradautomates/claude-video -g
npx skills add enisakarsu/derin-ads-hook-generator -g
```
