# Skabelon til nyt indlæg (post)
#
# Gem filen som: _posts/ÅÅÅÅ-MM-DD-dit-titel.md
# Eksempel:      _posts/2026-03-15-sommerens-begivenheder.md
#
# Obligatoriske felter: layout, title, date
# Valgfrie felter:      author, categories, tags, image, image_alt, excerpt

---
layout: post
title: "Dit indlæg titel"
date: ÅÅÅÅ-MM-DD HH:MM:SS +0100
author: Huebanden
categories:
  - kategori
tags:
  - tag1
  - tag2
# image: /assets/images/dit-billede.jpg
# image_alt: "Billedbeskrivelse"
excerpt: "Kort beskrivelse af indlægget (vises på forsiden)."
---

Skriv dit indhold her i Markdown.

## Overskrift

Brødtekst …

## Tilføj et billede

![Billedbeskrivelse](/assets/images/dit-billede.jpg)

## Tilføj en video

**YouTube:**

{% include video.html url="https://www.youtube.com/watch?v=VIDEO_ID" title="Video titel" %}

**Vimeo:**

{% include video.html url="https://vimeo.com/VIDEO_ID" title="Video titel" %}
