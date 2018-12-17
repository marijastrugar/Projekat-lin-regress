**Linearna regresija**

Da ilustrujemo ovaj primjer, koristili smo CalCOFI okeanografske podatke, preuzete sa: https://www.kaggle.com/sohier/calcofi#bottle.csv

Koristeći fajl bottle.csv, napravili smo bottle.xlsx, koji je zatim korišćen u primjeru. Originalni bottle.csv je redukovan, izbacujući nepotrebne kolone, tako da ostanu samo dvije relevantne kolone: salinitet vode i temperatura vode.

Zatim, kolone su skraćene na ~10000 redova, jer originalni bottle.csv sadrži ~814000 redova i veličine je ~49MB, šro predstavlja problem za softverski paket koji smo koristili u rješavanju problema.

**Python skripta**

Podatke učitavamo koristeći _pandas_ paket i zatim isfiltriramo, izbacujući (djelimično) prazne redove. Pošto su podaci predstavljeni u 2 kolone, matricu podataka transponujemo i ta dva reda razdvojimo u dvije promjenljive.

Linearna regresija se postiže korišćenjem _stats_-a, a rezultujući podaci su iskorišćeni da iscrtamo linearnu funkciju kroz originalnu grupu podataka.

Korišćenjem _R-vrijednosti_ ograničavamo moguće granice i pokušavamo da iscrtamo nekoliko različitih podataka.

**Prilozi**

Repozitorijum sadrži bottle.xlsx fajl i rezultujuću sliku koju iscrtava  _matplotlib_ na kraju izvršavanja koda linearne regresije.
