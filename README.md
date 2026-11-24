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

| Alan | Skill'ler |
|---|---|
| Araştırma ve strateji | product-marketing, understand-customers, customer-journey, competitor-analysis, social-content, content-strategy, marketing-psychology, launch, content-matrix |
| Ses ve profil | voice-builder, newsletter-voice, profile-optimizer |
| Gönderi üretimi | post-writer, post-formatter, hook-generator, quote-post, pinned-comment, post-scorer |
| Metin | copywriting, copy-editing |
| Görsel | graphic-designer, gemini-carousel, gemini-infographic, banner-design |
| Video | watch, video-understand, reels-scripting, youtube-seo, derin-ads-hook-generator |
| Dağıtım | parasite-and-pr |

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
