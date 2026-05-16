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

Sadržaj ovog repozitorija (logotipi, izvorne datoteke, dokumentacija i pripadajući materijali) licenciran je pod **[Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)](https://creativecommons.org/licenses/by-nd/4.0/deed.hr)**.

Slobodno smijete:

- **Dijeliti** — kopirati i redistribuirati materijal u bilo kojem mediju ili formatu, uključujući komercijalnu upotrebu

Pod sljedećim uvjetima:

- **Atribucija** — morate navesti odgovarajuće priznanje izvora (DOMOVINA.tv), poveznicu na licencu i naznačiti jesu li napravljene izmjene
- **Bez prerada** — ako preradite, transformirate ili nadograđujete materijal, ne smijete distribuirati izmijenjeni materijal

Puni pravni tekst dostupan je u datoteci [`LICENSE`](LICENSE) te na [creativecommons.org/licenses/by-nd/4.0/legalcode](https://creativecommons.org/licenses/by-nd/4.0/legalcode).

## Žigovi (Trademark)

Nazivi **„Domovina"**, **„Domovina TV"**, **„Domovina AI"**, **„Domovina Energy"**, stilizirano slovo „D" ispunjeno bojama hrvatske zastave te svi pripadajući logotipi, ikone i vizualni znakovi (zajednički „Žigovi") jesu žigovi društva **DOMOVINA.tv**.

CC BY-ND 4.0 licenca odnosi se isključivo na **autorska prava** na grafičkom djelu. Ne dodjeljuje nikakvo pravo, dopuštenje ni odobrenje za korištenje Žigova kao žigova. Posebno, **NIJE dopušteno**:

- Koristiti Žigove (ili zbunjujuće slične znakove) kao naziv, logotip ili identifikator vlastitog proizvoda, usluge, tvrtke ili projekta
- Koristiti Žigove na način koji sugerira sponzorstvo, odobrenje, partnerstvo ili povezanost s DOMOVINA.tv koja ne postoji
- Registrirati Žigove (ili zbunjujuće slične znakove) kao žigove, internetske domene, korisnička imena na društvenim mrežama ili nazive tvrtki
- Mijenjati Žigove na bilo koji način (neovisno zabranjeno i uvjetom *NoDerivatives* iz CC BY-ND 4.0)

**Dopuštena je** činjenična, opisna ili uredničko-novinarska upotreba Žigova radi referenciranja DOMOVINA.tv i njegovih proizvoda — primjerice u novinskim člancima, recenzijama, akademskim radovima ili tehničkoj dokumentaciji — uz uvjet da je takva upotreba poštena, ne dovodi u zabludu i ne implicira odnos koji ne postoji.

Sva prava na Žigove koja nisu izričito dodijeljena ovom napomenom ostaju pridržana.

## Kontakt

Za pitanja o korištenju brand resursa, licenciranju upotrebe Žigova izvan dopuštenog opsega, suradnji ili partnerstvima obratite se timu projekta **Domovina**.
