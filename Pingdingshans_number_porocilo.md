# PINGDINGSHAN'S NUMBER

## UVOD
(kratka predstavitev problema, opis generiranja in zbiranja podatkov - nauty geng, glavna ideja)
### Kratka predstavitev/opis problema
V okviru najinega projekta, sva iskala tako imenovano Pingdingshanovo število poznano tudi kot 'subpath number'. To je število vseh poti v danem grafu, tudi trivialnih, torej poti dolžine 0. Tu je pot v grafu zaporedje vozlišč, kjer se ta ne smejo ponavljati. V jeziku Sage sva definirala algoritem PDS, ki  izračunava Pingdingshanovo število. Iskala sva ga le na povezanih grafih, kjer sva ločila in posebej obravnavala različne skupine grafov. Na vozliščih $i = 1, ... , 8$ sva za skupine kubičnih, dvodelnih, grafov brez trikotnikov in nazadnje še vseh grafov izračunala maksimalne vrednosti PDS-ja na posameznem vozlišču in nato te vrednosti primerjala med skupinami grafov. Dalje sva postavila hipotezo, katera skupina grafov bo imela največji PDS, nato pa naredila stohastično analizo, s pomočjo katere bova videla, ali se rezultati le-te skladajo z najino hipotezo, ali pa ji nasprotujejo. Argumentirala sva  rezultate stohastične analize in povzela ugotovitve.

### Generacija in zbiranje podatkov
#### Generacija
Za generacijo podatkov sva izbrala nauty.geng okolje, saj se nama je zdelo najbolj primerno iz večih razlogov. Funkcija nauty.geng ne zgenenrira bseh grafov, temveč zgolj generatorje za izbrane grafe na i vozliščih. To je bilo za najin program bolj učinkovito, saj si razen določenih grafov (tistih, ki so imeli največje pds število v posamezni skupini) nisva želela shraniti vseh grafov. To bi bilo za najin računalnik in program veliko prezahtevno, za občutek na 8 vozliščih je 268 435 456 možnih grafov. Poleg prezahtevnosti, pa je v prid ne shranjevanju potegnilo tudi dejstvo, da teh grafov za analizo Pingdingshanovega števila nisva potrebovala. Nauty.geng nama je torej omogočil, da si za vsako skupino pripraviva generatorje grafov na željenih vozliščih, nato pa z uporabo for zanke inzračunava pds števila za vsako skupino in si zapomniva zgolj največja pds števila v posameznih skupinah za pimerno število vozlišč. Nauty.geng kot argumente sprejme število vozlišč in poebne argumente za vsako od skupin grafov. Ti so navedeni pri posameznih skupinah. Funkcije za generacijo generatorjev grafov so med seboj zelo simetrične (vse kar se bistveno spremeni so argumenti v nauty.geng funkciji in določene specifike glede na skupino grafov) zato bova kot psavdo kodo navedla zgoraj omenjene funkcije zgolj za vse grafe.

#### Zbiranje oziroma shranjevanje


## 1 ISKANJE PDS-JA NA GRAFIH Z i VOZLIŠČI i=1,2,...,8
(algoritem PDS, skupine grafov - lastnosti grafov)

### 1. 1 ALGORITEM PDS
Algoritem PDS(G) vrne Pingdingshanovo število grafa G. + psevdokoda PDS algoritma

### 1. 2 DVODELNI GRAFI

### 1. 3 KUBIČNI GRAFI
Za kubične grafe velja, da imajo vsa vozlišča v takem grafu stopnjo natanko 3 (pravimo jim tudi 3-regularni grafi). Lastnost kubičnih grafov je tudi, da jih lahko dobimo le na sodo mnogo vozliščih. Kubične grafe sva tako kot vse ostale zgenerirala pomočjo nauty.geng paketa v Sageu. Argument, ki ga moramo podati za generacijo kubičnih grafo s pomočjo nauty.geng je "-d3 -D3", kjer nam številka poleg -d pove najnižjo stopnjo za vsa vozlišča v grafu, številka poleg -D pa najvišjo. Ker so vsi kubični grafi 3 regularni moramo obe številki postaviti na 3.
### 1. 4 GRAFI BREZ TRIKOTNIKOV
Grafi brez trikotnikov oziroma grafi brez ciklov dolžine so definirani za vse možne i=1,2,...,8. Tudi te sva genenirala s pomočjo nauty.geng. Če želimo s nauty.geng zgenenrirati grafe brez ciklov dolžine tri potrebujemo argument -t.

## 2 PRIMERJAVA PDS MED SKUPINAMI GRAFOV 
(graf, navedba hipoteze)

Za vsako skupino grafov sva napisala funkcijo, ki za vsakega od vozlišč $i = 1, ..., 8$ izračuna maksimalno Pingdingshanovo število grafov znotraj te skupine. Vrednosti sva shranjevala v slovarje, kjer so ključi števila vozlišč, vrednosti pa maksimalna PDS. Slovar je oblike: ...

## 3 STOHASTIČNA ANALIZA
(algoritem, primerjava pdsja orignalnih grafov z pdsjem novih)

## 4 POLNI GRAFI 
(podatki v prid hipoteze)

## ZAKLJUČEK



Pomožne točke:
• Približno 5 strani (fleksibilno).
• Vsebuje jasen opis problema.
• Vsebuje glavne ideje programa ali psevdokodo.
• Vsebuje jasen opis generiranja ali izbiranja podatkov.
• Prikaže grafe, tabele ali drugaˇcen opis eksperimentov (npr. kako se poveˇca ˇcas izvajanja z
velikostjo problema).
