# Mediakit — Domovina

Službeni brand resursi obitelji proizvoda **Domovina**.

<p align="center">
  <img src="domovina_tv_logo_square.svg" width="160" alt="Domovina TV">
  &nbsp;&nbsp;&nbsp;
  <img src="domovina_ai_logo_square.svg" width="160" alt="Domovina AI">
  &nbsp;&nbsp;&nbsp;
  <img src="domovina_energy_logo_square.svg" width="160" alt="Domovina Energy">
</p>

## O repozitoriju

Repozitorij sadrži službene logotipe — u vektorskom (SVG) i rasterskom (PNG) formatu — za sve proizvode obitelji **Domovina**. Namijenjen je novinarima, partnerima, autorima sadržaja te svima koji žele referencirati ili prikazati Domovina brendove u izvornom, neizmijenjenom obliku.

## Brand sustav

Svi logotipi dijele jedinstveni vizualni okvir koji osigurava prepoznatljivost obitelji proizvoda:

- **Slovo „D"** ispunjeno horizontalnim prugama hrvatske zastave (crvena, bijela, plava) — vizualni temelj koji povezuje brend s hrvatskim identitetom.
- **Unutarnje bijelo „D"** — negativan prostor koji okružuje simbol proizvoda i osigurava čitljivost.
- **Središnji simbol** u tamnoplavoj boji (`#002F6C`) — jedinstven je za svaki proizvod i nosi semantičku poruku o njegovoj namjeni.
- **Bijela pozadina sa zaobljenim kutovima** — radijus zaobljenja iznosi 32 jedinice na platnu od 512 × 512.

### Paleta boja

| Naziv | HEX | Uloga |
|---|---|---|
| Crvena (HR zastava) | `#FF0000` | Gornja traka slova „D" |
| Bijela | `#FFFFFF` | Srednja traka i pozadina |
| Tamnoplava (HR zastava) | `#002F6C` | Donja traka i središnji simbol |

## Proizvodi

### Domovina TV
<img src="domovina_tv_logo_square.svg" width="110" align="left" hspace="20" vspace="4" alt="Domovina TV logotip">

Video platforma s domaćim sadržajem. Središnji simbol — trokut s vrhom udesno (play gumb) — univerzalno prepoznatljiv znak za reprodukciju multimedije.

<br clear="left">

### Domovina AI
<img src="domovina_ai_logo_square.svg" width="110" align="left" hspace="20" vspace="4" alt="Domovina AI logotip">

Platforma za AI-asistirane usluge nad medijskim sadržajem. Središnji simbol — povezani čvorovi oko zajedničkog središta — predstavlja neuronsku mrežu i graf znanja koji povezuje sadržaj, izvore i kontekst.

<br clear="left">

### Domovina Energy
<img src="domovina_energy_logo_square.svg" width="110" align="left" hspace="20" vspace="4" alt="Domovina Energy logotip">

Platforma za skupno financiranje (*crowdfunding*) obnovljivih izvora energije u Hrvatskoj — fotonaponskih elektrana, infrastrukture za električna vozila te vozila na vodik. Središnji simbol — munja — predstavlja električnu energiju kao zajednički nazivnik svih budućih energetskih vertikala.

<br clear="left">

## Datoteke

| Proizvod | Vektor (SVG) | Raster (PNG, 2048 × 2048) |
|---|---|---|
| Domovina TV | [`domovina_tv_logo_square.svg`](domovina_tv_logo_square.svg) | [`domovina_tv_logo_square.png`](domovina_tv_logo_square.png) |
| Domovina AI | [`domovina_ai_logo_square.svg`](domovina_ai_logo_square.svg) | [`domovina_ai_logo_square.png`](domovina_ai_logo_square.png) |
| Domovina Energy | [`domovina_energy_logo_square.svg`](domovina_energy_logo_square.svg) | [`domovina_energy_logo_square.png`](domovina_energy_logo_square.png) |

**Preporuka:** za sve digitalne i tiskane primjene koristite SVG kad god je to moguće — vektor ostaje oštar pri bilo kojoj veličini. PNG koristite isključivo ondje gdje SVG nije podržan (primjerice u nekim alatima za društvene mreže ili pri pripremi sažetaka u e-mailovima).

## Generiranje PNG-ova iz SVG-a

Sve PNG datoteke u repozitoriju generirane su iz pripadajućih SVG izvora pomoću alata [`rsvg-convert`](https://wiki.gnome.org/Projects/LibRsvg) (dio paketa `librsvg`):

```bash
# instalacija (macOS)
brew install librsvg

# generiranje sva tri logotipa na 2048 × 2048
for name in tv ai energy; do
  rsvg-convert -w 2048 -h 2048 \
    "domovina_${name}_logo_square.svg" \
    -o "domovina_${name}_logo_square.png"
done
```

Za drugačiju veličinu jednostavno zamijenite vrijednost parametra `-w` i `-h` (npr. `512`, `1024`, `4096`).

## Pravila korištenja

Brand resursi smiju se koristiti uz sljedeća pravila:

- **Bez izmjena.** Logotip se ne smije mijenjati — zabranjene su izmjene boja, proporcija, rotacija, dodavanje efekata, teksta ili drugih elemenata.
- **Bez izvedenih verzija** koje bi mogle izazvati zabunu s izvornim brendom ili sugerirati partnerstvo, sponzorstvo ili odobrenje koje ne postoji.
- **Sigurnosni prostor.** Oko logotipa ostavite slobodan prostor jednak najmanje 1/8 njegove ukupne visine.
- **Minimalna veličina.** Na zaslonu logotip ne koristite manji od 24 × 24 piksela jer središnji simbol ispod te veličine postaje nečitljiv.
- **Pozadina.** Logotip ima ugrađenu bijelu pozadinu sa zaobljenim kutovima. Ne postavljajte ga preko teksturiranih površina ni preko boja koje smanjuju kontrast s rubom.

## Licenca

Uvjeti korištenja navedeni su u datoteci [`LICENSE`](LICENSE).

## Kontakt

Za pitanja o korištenju brand resursa, suradnji ili partnerstvima obratite se timu projekta **Domovina**.
