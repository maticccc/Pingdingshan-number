# PINGDINGSHAN'S NUMBER

## UVOD
(kratka predstavitev problema, opis generiranja in zbiranja podatkov - nauty geng, glavna ideja)

V okviru najinega projekta, bova iskala tako imenovano Pingdingshanovo število poznano tudi kot 'subpath number'. To je število vseh poti v danem grafu, tudi trivialnih, torej poti dolžine 0. Tu je pot v grafu zaporedje vozlišč, kjer se ta ne smejo ponavljati. V jeziku Sage bova definirala algoritem PDS, ki bo izračunal Pingdingshanovo število. Iskala ga bova le na povezanih grafih, kjer bova ločila in posebej obravnavala različne skupine grafov. Na vozliščih $i = 1, ... , 8$ bova za skupine kubičnih, dvodelnih, grafov brez trikotnikov in nazadnje še vseh grafov izračunala maksimalne vrednosti PDS-ja na posameznem vozlišču in nato te vrednosti primerjala med skupinami grafov. Dalje bova postavila hipotezo, katera skupina grafov bo imela največji PDS, nato pa naredila stohastično analizo, s pomočjo katere bova videla, ali se rezultati le-te skladajo z najino hipotezo, ali pa ji nasprotujejo. Argumentirala bova rezultate stohastične analize in povzela ugotovitve.


## 1 ISKANJE PDS-JA NA GRAFIH Z i VOZLIŠČI i=1,2,...,8
(algoritem PDS, skupine grafov - lastnosti grafov)

### 1. 1 ALGORITEM PDS
Algoritem PDS(G) vrne Pingdingshanovo število grafa G. + psevdokoda PDS algoritma

### 1. 2 DVODELNI GRAFI

### 1. 3 KUBIČNI GRAFI

### 1. 4 GRAFI BREZ TRIKOTNIKOV


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
