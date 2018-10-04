# Tuntiharjoitus 2

Tuntiharjoituksessa kaksi tavoitteennamme on tehdä saadusta datasta johtopäätöksiä ja tehdä ennustava puumalli.

Tehtävässä käytämme SPSS-modeler työkalua, joka on osa Watson Studiota.

## Vaihe 1.

### Luo Modeler flow

Watson Studiossa valitse ensin projektisi ja projektin asset-välilehdellä etsi kohta **Modeler Flows** paina **New flow** painiketta


![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.12.13.png "New flow Text 1")

Anna flowlesi nimi **Tuntiharjoitus 2_Omanimi** ja varmista että kohdat Modeler flow type on **Modeler Flow** ja Modeler Runtime on **IBM SPSS Modeler**



![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.18.01.png "New flow Text 2")

Paina **Create**

## Vaihe 2


### Työkalun ominaisuudet

Edessäsi on tyhjä kanvas, SPSS Modeler on graafinen analytiikan työkalu, jolla voidaan tehdä analyyttisiä päätelmiä, sekä kouluttaa erilaisia malleja

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.20.46.png "New flow Text 3")
## kanvas

Keskellä oleva tyhjä tila on flown kanvas, tähän tuodaan nodeja, jotka yhdistettynä toisiinsa luovat halutun flown, eli työn ja sen järjestyksen


### Nodes

Vasemmalla on nodes valikko, sieltä löytyy kaikki tarvittavat työkalut. Ne on jaettu toiminnallisuuden mukaan eri kategorioihin.

Tässä harjoituksessa tulemme käyttämään kaikkien muiden kategorioiden nodeja, paitsi exportin. Export noden tehtävänä on tallentaa data uutena data tiedostona takaisin projektiin.

### Toolbar

Kanvaksen yläpuolella on toolbar. Toolbarista löytyy napit tarvittaviin toimintoihin, joilla kanvakseen tehtyä flowta ajetaan. Ensimmäisenä vasemmalla on node-valikon nappi, josta nodet saa esiin. Toisena on Stop and Run napit, joista varsinkin Run on tärkeä. Tällä napilla saadaan ajettua flow, ja halutut toiminnat saadaan suoritettua.

Keskeltä löytyy copy ja paste napit, joilla saa kopioitua käyttämiään nodeja ja viimeisessä osiossa on delete ja settings napit. Nodeja saa kopioitua ja poistettua myös hiiren oikealla napilla.


## Vaihe 3

### Datan tuominen flowhun.

Valitse Node valikosta **Import** osio ja sieltä raahaa **Data Asset** node kanvakselle. Nodejen raahaaminen toimii perinteisellä drag and drop menetelmällä.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.31.31.png "New flow Text 5")



Tämän jälkeen tuplaklikkaa kanvakselle siirrettyä **Data Asset** nodea ja valitse oikealle avautuvasta valikosta **Change data asset**. Klikkaa valikosta **Dementtiapart2.csv** Tiedostoa ja valitse sivun oikeasta alalaidasta **OK**. Palattuasi takasin kanvakselle muista painaa **Save**-nappia tallentaaksesi nodeen tekemät muutokset.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.35.46.png "New flow Text 4")

## Vaihe 4

### Datan preparointi

#### Type node

Seuraavaksi lisää node-valikosta **Field Operations** alta **Type**-node kanvakselle. Type nodessa pystymme konfiguroimaan datan tyypit.
![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.41.44.png "New flow Text 6")

Jotta nodit toimivat yhteen on ne yhdistettävä. Nodet yhdistetään vetämällä viiva nodeissa olevasta pallosta toisen noden palloon.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.48.50.png "New flow Text 7")

Seuraavaksi konfiguroidaan nodet. Datasta tiedämme että ainut muutos joka on tehtävä on vuoden vaihtaminen kategoriseksi muuttujaksi.

Jotta saamme tämän tehtyä avaa type-node kaksoisklikkaamalla, oikealle avautuvasta valikosta valitse **configure Types** ja uudesta aukeavasta valikosta paina **Read Values**.

Muuttujan **Year** kohdalla vaihda **Continuous** **Categorical** tyyppiin.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.54.12.png "New flow Text 8")

Paina **OK**

Tämän jälkeen muista vielä painaa **Save** type noden valikosta, jotta tehdyt muutokset tallentuvat.

#### Data Audit

Tarkastellaan datan laatua, **Node valikosta** avaa **Output** valinta ja raahaa sieltä **Data Audit** node kavakselle. ja yhdistä nodet.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%207.57.19.png "New flow Text 9")

Nodejen yhdistämisen jälkeen paina toolbarista **RUN** nappia, eli play-ikonia.

Oikealle avautuu **Output list**, josta näet jatkossakin kaikki tuottamasi outputit. pääset listaan aina takaisin painamalla toolbarista nappia, jossa on piste, jonka yläpuolelta kiertää nuoli.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.00.25.png "New flow Text 10")

Tupla klikkaa Output valikosta Data audit outputtia

Avautuvasta raportista saamme hyvän yleiskäsityksen datasta ja sen ominaisuuksista.

#### Välitehtävä

Kuvaa lyhyesti esim wordissä yleisiä havaintoja datasta, mille ajanjaksolle data sijoittuu, keskiarvoja eri havainnoista, sekä datan laadusta.

#### Ensimmäiset havainnot

Tavoitteenamme on tehdä ennustava malli nOfIncidents kentästä. Lähdemmekin selvittämään ensimmäisenä onko meillä suoria selittäviä tekijöitä. Tähän tarkoitukseen hyvä työkalu on **Statistics**-Node, joka löytyy **Output** osiosta node-valikosta

Raahaa **Statistics**-node kanvakselle ja avaa sen asetukset tuplaklikkaamalla.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.09.40.png "New flow Text 11")


Paina **Examine** osion vierestä **add columns** nappia ja avautuvasta valikosta valitse kaikki kolumnit.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.10.51.png "New flow Text 12")

Paina **OK**

Paina **Correlate** osion vierestä **add columns** nappia ja avautuvasta valikosta valitse nOfIncidents kolumnni.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.14.16.png "New flow Text 13")

Paina **OK**

Muista jälleen tallentaa nodeen tehdyt muutokset **Save** painikkeella.

Kun olet tallentanut noden muutokset paina jälleen **Run** nappia.

Avautuvassa output ikkunassa huomaat että flow näyttää aina edellisienkin ajojen outputit. Tästä syystä työn selkeyden kannalta kannattaa harkita edellisten outputtien poistamista ennen seuraavaa ajoa. Outputit poistetaan painamalla kolmea pistettä, jotka sijaitsevat outputin oikealla puolella ja valitsemalla **delete**. Joudut vielä vahvistamaan poistamisen uudestaan.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.22.02.png "New flow Text 13")

Seuraavaksi avaa luomasi **Statistics** output.

#### Välitehtävä

Mitkä kentät selittävät nOfIncidents kolumnia?

#### Havaintojen tarkentaminen.

Huomasimme edellisessä kohdassa että esimerkiksi nukuttujen tuntien määrällä on suuri vaikutus nOfIncidents kolumniin. Piirrämme tästä kuvaajan, josta havainto on helpompi nähdä.

Valitse Node valikon **Graphs** Osiosta **Plot** node ja raahaa se kanvakselle. Avaa sen jälkeen noden asetukset tuplaklikkaamalla nodea.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.26.39%201.png "New flow Text 14")

Valitse **X**-muuttujaksi **Ssleepinghours** muuttuja ja **Y**-muuttujaksi **nOfIncidents** muuttuja.

Seuraavaksi avaa alavalikko **Overlay** ja laita raksi **Smoother** kohtaan, jotta saamme keskiarvo-viivan graafiin. Tämän jälkeen paina **Save**

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.27.01.png "New flow Text 15")

Paina jälleen **Run** nappia ja avaa tarkasteluun luotu graafi.

Graafin tarkastelu vahvistaa korrelaatio havainnon. Kaikki graafin pallot ovat selkeissä ryhmissä, ja niin sanottuja outliereita ei esiinny. Keskiarvoviiva on johdonmukainen ja menee suoraan alaspäin.


![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.35.11.png "New flow Text 16")

#### Uusien muuttujien luominen

Saavuttaaksemme vielä parempaa ymmärrystä käsiteltävästä keissistä luomme muuttujat **kuukausi** ja **period**. Näiden muuttujien avulla saamme paremman käsityksen siitä miten datan kohdehenkilön käyttäytyminen on muuttunut datan keruu aikana.

#### Month

**Field Operators** valikosta raahaa **derive** node kanvakselle. Yhdistä **Derive** node **Type** nodeen ja avaa **Derive** node.
![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%208.56.45.png "New flow Text 17")

Muuta noden nimi month nimiseksi. Saat muutettua noden nimeä Derive-tekstin oikealta puolelta löytyvästä kynästä.

Tämän jälkeen **Derived Field Name** kohtaan kirjoita **month** ja **Expression** kohtaan kirjoita kaava **datetime_month(date)**. Vaihda vielä **Measurement Categorial** muotoon.

![alt text](https://github.com/LasseHuotari/Analyticsbasic/blob/master/images/Näyttökuva%202018-10-4%20kello%209.00.04.png "New flow Text 18")





