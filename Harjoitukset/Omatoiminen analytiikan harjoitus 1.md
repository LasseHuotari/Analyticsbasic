# Omatoiminen analytiikan harjoitus 1


Omatoimisessa analytiikan harjoitus 1:ssä tarkastellaan ihmisen nukkumisen ja käyttäytymisen suhdetta. Harjoituksessa käytetöön Data kansiosta löytyvää SportClock.csv tiedostoa, joka on hypoteettinen datasetti älyrannekkeesta saaduista dementtia potilaiden tiedoista.

Käytä harjoitusta tehdessäsi hyväksi jo ennalta opittuja taitoja ja koita näitä hyödyntäen kuvata, sekä numeerisesti, että visualisoinnin kautta datasta tehtyjä havaintoja mahdollisimman kattavasti. Tutki myös datan laatua.

Apunasi voit käyttää Analyticsbasic repositoryn päänäkymästä löytyvää pandas ja python cheat sheet ohjeita.

Vinkki: Visualisoinnissa helppo koodi on df['Awakenings'].value_counts().plot(kind="bar",figsize=(10,10))

Jossa df on dataframen nimi, määritelty solussa jossa datan tuot sisään, ellet ole sitä muuttanut.
['Awakenings'] kolumnin nimi, tässä esimerkissä Awakenings
.value_counts() laskee yhteen montakokertaa havaintoja esiintyy datassa
.plot() piirtää graafin
kind="bar" on graaffin tyyppi, tässä tapauksessa pylväs. (Koita esim line ja scatter)
figsize=(19,10) kuvaajan koko

Palauta tekemäsi analyysi Omaan ipynb formaatissa, jonka saat Watson Studiosta ladattua.


Tietokuvaus:

Date: päivämäärä YYYY-MM-DD muodossa <br/>
nOfIncidents - Asiakkaan huonon käytöksen lukumäärä hoitajien havaintojen perusteella <br/>
SleepingHours - nukutut tunnit <br/>
Awakenings - Heräämiset yön aikana <br/>
RHR - leposykkeen keskiarvo <br/>
ActiveTime - Aktiivisuusaika <br/>
Steps - Askelmäärä
