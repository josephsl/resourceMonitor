# Resurssienvalvonta #

* Tekijät: Alex Hall, Joseph Lee, beqa gozalishvili, Tuukka Ojala, Ethin
  Probst sekä muut NVDA:n tekijät
* Lataa [vakaa versio][1]
* Yhteensopivuus: NVDA 2019.3-2020.2

Tämä lisäosa antaa tietoja suorittimen kuormituksesta sekä muistin ja muiden
resurssien käytöstä.

# Pikanäppäimet #

* NVDA+Vaihto+E: Lukee käytetyn RAM-muistin määrän, suorittimen
  keskimääräisen kuormituksen sekä akun tiedot, mikäli sellainen on
  käytettävissä.
* NVDA+Vaihto+1: Lukee suorittimen keskimääräisen kuormituksen, ja mikäli
  käytössä on moniydinsuoritin, myös ytimien kuormituksen.
* NVDA+Vaihto+2/5: Lukee sekä fyysisen että näennäisen RAM-muistin käytetyn
  ja kokonaismäärän.
* NVDA+Vaihto+3: Lukee kiintolevyjen ja siirrettävien asemien käytetyn ja
  kokonaistilan.
* NVDA+Vaihto+4: Lukee akun varauksen prosentteina, latauksen tilan,
  jäljellä olevan ajan (jos ei latauksessa) sekä varoituksen, mikäli
  varauksen taso on alhainen tai kriittinen.
* NVDA+Vaihto+6: Ilmoittaa suorittimen arkkitehtuurin (32- tai 64-bittinen)
  sekä Windowsin ja Service Packin version.
* NVDA+Vaihto+7 ilmoittaa järjestelmän käynnissäoloajan.

Jos käytössäsi on NVDA 2013.3 tai uudempi, voit muuttaa näitä pikanäppäimiä
Syötekomennot-valintaikkunasta.

## Huomautuksia käytöstä ##

Tämä lisäosa ei korvaa Windowsin tehtävienhallintaa tai muita
järjestelmätietoja näyttäviä ohjelmia. Huomaa lisäksi seuraavat seikat:

* Suorittimen käyttö ilmoitetaan loogisille suorittimille, ei fyysisille
  ytimille. Tällä on merkitystä Hyper Threading -teknologiaa käyttävissä
  suorittimissa, joissa suorittimien määrä on kaksi kertaa ydinten määrä.
* Levynkäyttötietoja haettaessa saattaa olla viivettä, mikäli levytoimintaa,
  kuten suurten tiedostojen kopiointia, on runsaasti.
* Tämä lisäosa edellyttää Windows 7 Service Pack 1:tä tai uudempaa.

## Versio 20.07

* Windows 10:n versio 20H2 tunnistetaan oikein Windowsin versiotietoja
  haettaessa (NVDA+Vaihto+6).
* Yksinkertaistettu Windows 10:n versioviestiä painettaessa NVDA+Vaihto+6,
  esim. Windows 10verVVKK:n:n asemesta Windows 10 VVKK.

## Versio 20.06

* Ratkaistu useita koodaustyylin ongelmia sekä mahdollisia bugeja Flake8:n
  kanssa.

## Versio 20.04

* Päivitetty psutil-riippuvuus versioksi 5.7.0.

## Versio 20.01

* NVDA 2019.3 tai uudempi vaaditaan laajamittaisen Python 3:n käytön takia.

## Versio 19.11

* Windows Insider -esiversioiden tunnistusta paranneltu, erityisesti
  20H1:ssä ja uudemmissa.

## Versio 19.07

* Päivitetty psutil-riippuvuus versioksi 5.6.3.
* Sisäisiä muutoksia akun tilan ilmoittavaan komentoon.

## Versio 18.12

* Sisäisiä muutoksia tulevien NVDA-versioiden tukemiseksi.

## Versio 18.10

* Koodista on tehty yhteensopivampaa Python 3:n kanssa.
* Päivitetty psutil-riippuvuus versioksi 5.4.7.
* NVDA ei enää ilmoita virheistä haettaessa tietoa levyn kapasiteetista ja
  muistin käytöstä , mikäli käytetään  tietokonetta tai palvelua, jossa
  RAM-muistin määrä tai levyn koko ylittää yhden petatavun.
* Muistin ja levyn käytön arvot näytetään enintään kahdella desimaalilla
  (esim. 4.00 Gt aiemman 4.0 Gt sijaan).
* Windows Insider -esiversioiden tunnistusta paranneltu.

## Versio 18.04

Versio 18.04.x on viimeinen julkaisu, joka tukee 7 SP1:tä vanhempia
Windows-versioita.

* Viimeinen Windows Server 2003:a, Vistaa ja Server 2008:aa tukeva versio.
* Parempi Windows 10 -versioiden tunnistaminen sekä julkisten ja
  Insider-esiversioiden erottaminen toisistaan.

## Versio 17.12

* Lisätty tuki 64-bittisille ARM-suorittimille Windows 10:ssä.

## Versio 17.09

Tärkeää: 17.09.x on viimeinen Windows XP:tä tukeva versio.

* Viimeinen Windows XP:ssä ajettava versio.
* Windows 10:n koontiversio 16278 ja uudemmat tunnistetaan versioksi
  1709. Tästä lisäosasta julkaistaan pieni päivitys, kun version 1709 vakaa
  koontiversio on julkistettu.

## Versio 17.07.1

* Palautettu Windows XP:n tuki (ollut rikki versiosta 17.02 lähtien).

## Versio 17.05

* Järjestelmän käynnissäoloajan ilmoittaminen (edellisestä käynnistyksestä
  kulunut aika; NVDA+Shift+7).

## Versio 17.02

* Päivitetty psutil-riippuvuus versioksi 5.0.1.
* NVDA ei näytä enää virheilmoitusta levynkäyttötietoja tarkistettaessa
  järjestelmissä, joissa siirrettävää tietovälinettä ei tunnistettu oikein
  (esim. kun muistikorttia ei ole asetettu kortinlukijaan).

## Versio 16.08

Lisäosan versionumerot ovat Versiosta 16.08 alkaen muotoa
vuosi.kuukausi.tarkistusversio.

* Windows 10:n eri versiot tunnistetaan nyt oikein (kuten 1607
  koontiversiossa 14393).
* Windows 10:n koontiversiot tunnistetaan oikein kumulatiivisten päivitysten
  asentamisen jälkeen (kuten 14393.51).
* Insider-esiversiot tunnistetaan oikein.

## Muutokset versiossa 4.5 ##

* Lisäosan koodivarasto on muuttanut GitHubiin (löytyy osoitteesta
  https://github.com/josephsl/resourcemonitor).
* Windows Server 2016 tunnistetaan asianmukaisesti.

## Muutokset versiossa 4.0 ##

* Päivitetty psutil-riippuvuus versioksi 2.2.1.
* Suorituskykyä paranneltu huomattavasti suorittimen kuormituksen tietoja
  haettaessa.
* Lisätty tuki Windows 10:n tunnistamiselle.
* Windows 10:n versiota ilmoitettaessa kerrotaan myös koontiversio.
* Ohje on käytettävissä Lisäosien hallinnasta.

## Muutokset versiossa 3.1 ##

* Resurssienvalvonta tukee virallisesti Windows 8.1:tä.
* Käännöksiä päivitetty.

## Muutokset versiossa 3.0 ##

* Päivitetty psutil-riippuvuus versioksi 1.2.1.
* Suorittimen arkkitehtuurin sekä Windowsin ja Service Packin version
  ilmoittaminen (NVDA+Shift+6).
* Mahdollisuus vaihtaa lisäosan pikanäppäimiä (NVDA:n 2013.3-versiossa tai
  uudemmassa).
* Mahdollisuus kopioida yksittäisen resurssin tiedot leikepöydälle
  painamalla komentoja kahdesti.

## Muutokset versiossa 2.4 ##

* Uusia kieliä: kiina (yksinkertaistettu), ukraina
* Käännöksiä päivitetty.

## Muutokset versiossa 2.3 ##

* Lisätty bulgariankielinen käännös.

## Muutokset versiossa 2.2 ##

* Lisätty seuraavat käännökset: arabia, aragonia, brasilianportugali,
  espanja, galego, hollanti, italia, japani, korea, kroatia, nepali, puola,
  ranska, saksa, slovakki, slovenia, suomi, tamili, turkki, unkari ja
  venäjä.

## Muutokset versiossa 2.1 ##

* Päivitetty psutil-riippuvuus versioksi 0.6.1.
* Korjattu pitkä viive asemien tietoja haettaessa.
* Koodia siivottu.

## Muutokset versiossa 2.0 ##

* Lisätty käännösten tuki ja käännöskommentteja.

## Muutokset versiossa 1.0 ##

* Ensimmäinen versio

[[!tag dev stable]]

[1]: https://addons.nvda-project.org/files/get.php?file=rm
