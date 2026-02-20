# huebanden.dk

Officiel hjemmeside for Huebanden, hostet via [GitHub Pages](https://pages.github.com/).

## Sådan redigerer du siden

Siden er bygget med [Jekyll](https://jekyllrb.com/) og bruger Markdown til alt indhold.

### Tilføj et nyt indlæg

1. Kopiér `_templates/new-post.md` til mappen `_posts/`.
2. Omdøb filen til formatet `ÅÅÅÅ-MM-DD-dit-titel.md` (f.eks. `2026-03-15-sommerfest.md`).
3. Udfyld frontmatter-felterne øverst i filen og skriv dit indhold i Markdown nedenunder.
4. Commit og push – siden opdateres automatisk.

### Tilføj en ny side

1. Kopiér `_templates/new-page.md` til mappen `_pages/`.
2. Giv filen et sigende navn (f.eks. `kontakt.md`).
3. Udfyld `title`, `permalink` og indholdet.
4. Commit og push.

### Tilføj billeder

Læg billedfiler i `assets/images/` og referer til dem i Markdown:

```markdown
![Billedbeskrivelse](/assets/images/mit-billede.jpg)
```

### Indlejr en video

Brug `video`-inkluderingen i et indlæg eller en side:

```liquid
{% include video.html url="https://www.youtube.com/watch?v=VIDEO_ID" title="Titel" %}
{% include video.html url="https://vimeo.com/VIDEO_ID" title="Titel" %}
```

### Frontmatter-felter for indlæg

| Felt         | Påkrævet | Beskrivelse                                      |
|--------------|----------|--------------------------------------------------|
| `layout`     | Ja       | Brug `post` for indlæg                           |
| `title`      | Ja       | Titel på indlægget                               |
| `date`       | Ja       | Dato i formatet `ÅÅÅÅ-MM-DD HH:MM:SS +0100`      |
| `author`     | Nej      | Forfatter                                        |
| `categories` | Nej      | Liste af kategorier – bruges til sortering       |
| `tags`       | Nej      | Liste af tags                                    |
| `image`      | Nej      | Sti til forsidebillede, f.eks. `/assets/images/x.jpg` |
| `image_alt`  | Nej      | Alt-tekst til forsidebilledet                    |
| `excerpt`    | Nej      | Kort beskrivelse der vises på forsiden           |

## Lokal udvikling

```bash
bundle install
bundle exec jekyll serve
```

Åbn herefter <http://localhost:4000> i din browser.