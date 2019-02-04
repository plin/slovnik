# Český tvarotvorný slovník

Vzali sme 100 000 najčastejších slovných tvarov z korpusu, vytvorili vzory a polo-automaticky zaradili. Podrobnosti nájdete v diplomových prácach
 * M. Grác: Tvorba morfologické databáze z neoznačkovaného korpusu (https://is.muni.cz/th/d11gr/)
 * D. Husárová: Určování tvarotvorných vzorů neznámých slov (https://is.muni.cz/th/dxbz4/)
 * D. Ryšavá: Automatická tvorba imperativů z infinitivu (https://is.muni.cz/th/rq187/)
 
V adresári generated/ nájdete pripravené vygenerované dáta (tvar slova:základný tvar slova:gramatická značka) pre podstatné mená, 
prídavné mená a slovesá. Slovné druhy, ktoré sú najzaujímavejšie, čo sa týka ohýbania :) 

V adresári src/ nájdete zdrojové dáta a definície vzorov. Ak by ste ich chceli aplikovať na dáta, tak je možné použiť (zastaralý, málo dokumentovaný, ...) 
softvér Langusta (https://github.com/marxsk/langusta3) v ktorom je aj nástroj na pridávanie nových slov do slovníku. 

Licencia: Public Domain 

## Podpora

Ak nájdete chyby, či už systematické, alebo náhodné, tak nám prosím dajte o chybe vedieť. Buď na githube, alebo mailom na grac@mail.muni.cz. 

Ak by ste chceli náš slovník rozšíriť, tak nám len pošlite zmeny (ako pull request; alebo mailom). 

Ak neviete ako na to, ale ste ochotní zafinancovať to rozšírenie, tak sa ozvite. Budete prekvapení ako rýchlo a lacno sa to dá urobiť :)

## Autori

Na dátach a programoch pracovali (abecedne) M. Grác (@marxsk), D. Husárová, D. Ryšavá a N. Volková [obor Počítačová lingvistika, FF MU, Brno]

Konzultácie: doc. Klára Osolsobě, Dr.

Za finančnú podporu ďakujeme: Red Hat Czech, s.r.o.

## Popis značiek

Značky sú zapisovaná ako postupnosť dvojíc (atribút, hodnota), pričom každá informácia sa musí zmestiť do jedného znaku. 
Takže značka k1gFnSc4 je (k, 1), (g, F), (n, S), (c, 4). Vychádza sa z latinských názvov a čísiel pádov tak ako sa učia v škole.

Atribút | Hodnota
--------|--------
k       | Slovný druh; 1 - podstatné meno; 2 - prídavné meno; 5 - sloveso
g       | Gramatický rod; F - ženský, M - mužský životný, I - mužský neživotný, N - stredný
n       | Číslo; S - jednotné (singulár), P - množné (plurál)
c       | Pád; 1 - nominatív, 2 - genitív, 3 - datív, 4 - akuzatív, 5 - vokatív, 6 - lokál, 7 - inštrumentál
p       | Osoba
m       | "Druh slovesného tvaru"

## Citovanie
V prípade použitia v akademických článkoch sa prosím odkazujte na:

```
@inproceedings{866580,
   author = {Grác, Marek},
   address = {Brno},
   booktitle = {Proceedings of RASLAN 2009},
   keywords = {morphological paradigm nlp},
   language = {eng},
   location = {Brno},
   isbn = {978-80-210-5048-8},
   publisher = {Masaryk University},
   title = {Yet Another Formalism for Morphological Paradigm},
   year = {2009}
}
```
