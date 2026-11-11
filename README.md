# Elektro chart

Preprost interaktivni prikaz časovnih blokov in njihovih cen skozi dan. Urnik je razdeljen po sezonah ter na delovne in dela proste dni, tako da lahko na enem mestu primerjate razporeditev blokov za vseh 24 ur.

**Aplikacija:** [elektrika-blok-cene.vercel.app](https://elektrika-blok-cene.vercel.app/)

## Kaj omogoča

- prikaz urnika blokov po urah za zimsko in poletno sezono;
- ločen prikaz delovnih dni in dela prostih dni;
- urejanje prikazanih cen za bloke 1–5;
- tiskanje oziroma shranjevanje prikaza v PDF z gumbom **Shrani PDF**.

Cene so v aplikaciji začetne informativne vrednosti, ki jih lahko prilagodite. Prikaz ni uradni obračun in ne predstavlja nujno cene, ki vam jo zaračuna vaš dobavitelj. Za podatke, veljavne za vašo lokacijo, se obrnite na dobavitelja ali obiščite [mojelektro.si](https://mojelektro.si/).

## Lokalni zagon

Potrebujete Node.js in pnpm. Namestite odvisnosti in zaženite razvojni strežnik:

```bash
pnpm install
pnpm dev
```

Zaženite `pnpm dev -- --open`, če želite aplikacijo po zagonu odpreti v brskalniku.

## Ukazi

```bash
pnpm dev       # razvojni strežnik
pnpm build     # produkcijska gradnja
pnpm preview   # predogled produkcijske gradnje
pnpm lint      # preverjanje oblikovanja s Prettierjem
pnpm format    # samodejno oblikovanje datotek
```

Projekt uporablja SvelteKit, Svelte, Vite in Tailwind CSS. Za produkcijsko objavo lahko glede na izbrano okolje potrebujete ustrezen SvelteKit adapter.
