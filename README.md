# /pazarlama — Claude Code için pazarlama ve sosyal medya skill paketi

Enis Akarsu'nun günlük kullandığı pazarlama skill'leri tek bir komutta toplandı.
`/pazarlama` yazınca tüm liste önüne gelir; ihtiyacın olanı seçip tetiklersin.

## Kurulum

Claude Code'a şu promptu yapıştır:

```
Install the /pazarlama skill package from github.com/enisakarsu/pazarlama-skill globally.
Run: npx skills add enisakarsu/pazarlama-skill -g
Then install every skill listed in its "Kurulum" section, globally, and confirm with a list.
```

Ya da elle:

```
npx skills add enisakarsu/pazarlama-skill -g
```

Ardından `skills/pazarlama/SKILL.md` içindeki "Kurulum" komutlarıyla alt skill'leri kur.

## İçindekiler

| Alan | Skill'ler |
|---|---|
| Araştırma ve strateji | product-marketing, understand-customers, customer-journey, competitor-analysis, social-content, content-strategy, marketing-psychology, launch |
| Metin | copywriting, copy-editing |
| Video | watch, youtube-seo, derin-ads-hook-generator |
| Dağıtım | parasite-and-pr |

## Kaynaklar

Bu paket bir yönlendiricidir; alt skill'ler kendi depolarından kurulur ve haklar sahiplerine aittir:

- [hsynozdamar-byte/claude-skills-edited](https://github.com/hsynozdamar-byte/claude-skills-edited)
- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
- [Illyism/seo-skills](https://github.com/Illyism/seo-skills)
- [every-app/open-seo](https://github.com/every-app/open-seo)
- [bradautomates/claude-video](https://github.com/bradautomates/claude-video)
- [enisakarsu/derin-ads-hook-generator](https://github.com/enisakarsu/derin-ads-hook-generator)

Daha fazlası: [enisakarsu.com](https://enisakarsu.com)

## Lisans

Yönlendirici (`skills/pazarlama/SKILL.md`) MIT lisanslıdır. Alt skill'ler kendi lisanslarına tabidir.
