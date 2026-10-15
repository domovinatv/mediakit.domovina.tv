# Znakovi srodnih brendova: kako su nastali (14.–15.10.2026.)

Pravila i datoteke su u [README](../README.md#srodni-brendovi-mpt-airkuna-i-paydomovinaai). Ovdje je ono što se iz datoteka ne vidi: što je odbačeno i zašto, zamke pri crtanju i gdje sve žive kopije.

## Odbačeno

| Varijanta | Razlog |
|---|---|
| Stari € u kovanici Domovina Pay (zaobljeni potezi) | „izgleda ko nekakav zec kojeg je generirao AI“: okrugle kapice i slobodne krivulje |
| MPT E (savijeni rep / strelica) | „izgleda ko vragov rep“: svaka Q-bezier krivulja ili savijeni završetak |
| MPT B, C, D, H, I | slabije čitljivo na 16 px ili bez veze s ostala dva znaka |
| MPT J (kovanica) | preblizu Pay kovanici, dva brenda bi se miješala |
| pay.domovina.ai kao „P“ pločica | korisnik je izabrao geometrijski € |
| airKUNA kao životinja kuna (clipart ili geometrijska) | ne veže se s M i € u isti sustav; zadržana samo ideja kovanice za token |

Zajednički nazivnik: **samo puni geometrijski oblici, ravno odrezani krajevi.** Veza između tri brenda je isti zlatni chevron (MPT M, airKUNA K), ista pločica i ista paleta.

## Zamke pri crtanju

- **Svaki dio znaka zaseban `<path>`.** Kad su bijeli i zlatni dijelovi ili preklapajući oblici u istom pathu, `fill-rule` izbuši rupe na preklopu. Dogodilo se, popravljeno razdvajanjem.
- **Provjera na 16 i 32 px**, ne samo na 512. Tanke crte i razmaci ispod ~1,5 jedinice na 32×32 platnu nestanu u faviconu.
- **Maskable PWA ikone** trebaju punu pozadinu do ruba i znak skaliran na ~0,82, inače Android odreže kutove.
- **macOS AppIcon** po Apple mreži: pločica 824 na platnu 1024, ne do ruba.
- **airKUNA `logo.svg`** ima viewBox `-5 -5 42 42` da zrake oko znaka ne budu odrezane.

## Kopije (promjena znaka = mediakit prvo, pa sve ovo)

- `pay.domovina.ai`: `docs/brand/`, `web/favicon.svg|png`, `web/icons/`, macOS AppIcon, admin `HEADER_LOGO_SVG` u `backend/src/admin/views.ts` (MPT M)
- `mpt-landing`: `public/favicon.svg`, `Logo()` u `src/components/site.tsx`, `docs/brand/og.svg` → `public/og.png`
- `airkuna-web`: `logo.svg` i `coin.svg` u 22 mape (oba sitea)

## Otvoreno

- Admin logo na mpt.domovina.ai deployan, ali vizualno neprovjeren (iza Cloudflare Access prijave).
- OMM: varijante A i B u mediakitu, konačan izbor čeka (vidi poglavlje OMM gore).

## OMM (dodano 15.10.2026.)

Druga sesija je po promptu iz ove napravila dvije varijante, obje s istim simbolom (prsten „O“ i munja, munja kao zaseban `<path>`, prsten jedan path s namjernom rupom preko evenodd):

- **B** `omm_logo_square`: pločica, bijeli prsten, zlatna munja. Aktivna na omm.domovina.ai; za tamnu temu web ima `logo-noc.svg` (bijela pločica, tamnoplavi prsten).
- **A** `domovina_omm_logo_square`: D okvir, prsten i munja tamnoplavi. Na webu s `?znak=a`. Munja je ista kao u Domovina Energy, pa se dva znaka razlikuju samo prstenom.

Odluka A vs. B još nije konačna (omm repo `CLAUDE.md`, „Izgled“). Kad se odluči, odbačenu varijantu u README označiti kao odbačenu, ali datoteku ostaviti.
