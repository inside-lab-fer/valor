# VALOR – mrežna stranica projekta

Stranica projekta VALOR (FER, NPOO / NextGenerationEU), na hrvatskom i engleskom.
Izrađena je u Jekyllu i objavljuje se preko GitHub Pages: https://inside-lab-fer.github.io/valor/

## Objava vijesti

Svaka vijest su dvije datoteke, jedna po jeziku:

- `hr/_posts/GGGG-MM-DD-kratki-naslov.md`
- `en/_posts/GGGG-MM-DD-short-title.md`

Obje imaju isti `ref`, pa poveznica „English / Hrvatski” vodi na drugu inačicu iste vijesti.

```markdown
---
title: Naslov vijesti
ref: radionica-2027
summary: Jedna rečenica za popis vijesti.
image: /assets/img/vijesti/radionica-2027.jpg   # neobavezno
image_alt: Opis slike                            # obavezno ako postoji image
---
Tekst vijesti u Markdownu.
```

Vijest se može dodati i izravno na GitHubu: *Add file → Create new file* u mapi `hr/_posts/`,
pa isto u `en/_posts/`. GitHub Pages objavi promjenu za minutu-dvije.

Datum u nazivu datoteke je datum objave. Vijest s datumom u budućnosti ne prikazuje se dok taj dan ne dođe.

Pravila (Opći uvjeti, čl. 7.1 i `IP_Visibility.docx`):

- radovi navode potporu: „This research was funded by the European Union NextGenerationEU through the National Recovery and Resilience Plan 2021-2026, under the institutional grant of the University of Zagreb Faculty of Electrical Engineering and Computing, project Value-aligned and interpretable optimization and reasoning (VALOR).”;
- amblem EU i odricanje od odgovornosti nalaze se u podnožju svake stranice (`_includes/funding.html`), ne treba ih dodavati u vijesti;
- ne objavljivati radove u dvostruko slijepoj recenziji s imenima autora.

## Ostale izmjene

- tim: `_data/team.yml`
- tekstovi sučelja i podaci o projektu: `_data/i18n.yml`
- naslovnice: `index.md` (EN, zadana) i `hr/index.md` (HR), uključujući popis rezultata

## Pokretanje lokalno

```bash
docker run --rm -v "$PWD":/srv/jekyll -p 4000:4000 jekyll/jekyll:4.2.2 jekyll serve
```

Stranica je tada na http://localhost:4000/valor/.

## Objava

1. Na GitHubu izraditi organizaciju (npr. `inside-lab-fer`) i u njoj repozitorij `valor`.
2. `git init && git add . && git commit -m "Initial site" && git branch -M main && git remote add origin git@github.com:inside-lab-fer/valor.git && git push -u origin main`
3. *Settings → Pages → Build and deployment*: Source *Deploy from a branch*, branch `main`, mapa `/ (root)`.
4. Ako je ime organizacije ili repozitorija drukčije, promijeniti `url` i `baseurl` u `_config.yml`.
