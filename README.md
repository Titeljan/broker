# Broker Nekretnine Pancevo — sajt

Statican sajt. Nema servera, nema build koraka: dovoljno je da fajlovi iz ovog foldera budu u repozitorijumu.

## Hostovanje na GitHub Pages

1. Napravi novi repozitorijum na GitHubu (npr. `broker-nekretnine`).
2. Ubaci sve fajlove iz ovog foldera u koren repozitorijuma (index.html mora biti u korenu).
3. Settings > Pages > Build and deployment > Source: **Deploy from a branch**, Branch: **main**, folder: **/ (root)**, Save.
4. Sajt je za minut-dva dostupan na `https://<korisnicko-ime>.github.io/<repo>/`.
5. Za svoj domen: Settings > Pages > Custom domain.

## Fajlovi

- `index.html` — ceo sajt (sve strane su u ovom fajlu, meni radi bez ponovnog ucitavanja)
- `stanovi.json` — lista oglasa, ovde dodajes i uklanjas stanove (uputstvo je na vrhu fajla)
- `slike/` — fotografije (imena su fiksna, vidi slike/UPUTSTVO.txt)
- `logo.jpg` — logo
- `support.js` — pogon sajta, ne diraj

## Vazno

- Fotografije se ucitavaju iz foldera `slike/` po tacnim imenima. Gde slika ne postoji, mesto ostaje prazno (sajt se ne kvari).
- `stanovi.json` i slike se ucitavaju preko mreze, pa sajt treba otvarati preko GitHub Pages adrese (ili lokalnog servera), a ne duplim klikom na index.html.
- React se ucitava sa interneta (unpkg.com), zato je potrebna internet konekcija posetiocu, sto je uvek slucaj.

## Sta jos treba dopuniti

- mail adresa i radno vreme (strana Kontakt)
- PIB i maticni broj (futer)
- godine rada i broj zavrsenih transakcija (stoji XXX)
- imena i pozicije clanova tima (strana O nama)
- naslovi tekstova na strani Vodici
