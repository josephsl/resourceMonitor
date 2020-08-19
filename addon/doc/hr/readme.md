# Prati stanje resursa (Resource Monitor) #

* Autori: Alex Hall, Joseph Lee, Beqa Gozalishvili, Tuukka Ojala, Ethin
  Probst i drugi NVDA doprinositelji
* Preuzmi [stabilnu verziju][1]
* NVDA kompatibilnost: 2019.3 do 2020.2

Ovaj dodatak daje informacije o opterećenosti procesora, korištenju memorije
i druge informacije o korištenju resursa.

# Prečaci #

* NVDA+šift+E: Prikazuje korištenje ram memorije, prosječno opterećenje
  procesora i informacije o stanju baterije, ako su dostupne.
* NVDA+šift+1: Prikazuje prosječnu opterećenost procesora i ako postoje
  višejezgreni procesori, prikazuje opterećenje svake jezgre.
* NVDA+šift+2/5: Prikazuje iskorišten i ukupni kapacitet fizičke I virtualne
  ram memorije.
* NVDA+šift+3: Prikazuje iskorišten i ukupni prostor na statičnim i
  prenosivim diskovima.
* NVDA+šift+4: Prikazuje postotak baterije, status punjenja, preostalo
  vrijeme (ako se ne puni), te upozorenje, ako je baterija slaba ili skoro
  prazna.
* NVDA+šift+6: Prikazuje strukturu procesora (32-64-bitni), verziju Windowsa
  i broj service paketa.
* NVDA+šift+7: Prikazuje trajanje pokretanja sustava.

Ako je instalirana NVDA verzija 2013.3 ili novija, tipkovničke prečace je
moguće mijenjati putem dijaloškog okvira za ulazne geste.

## Upute za primjenu ##

Ovaj dodatak ne zamjenjuje upravljača zadataka i druge programe za
informacije o sustavu Windows. Važno je znati i sljedeće:

* Informacije o korištenju procesora dane su za logičke procesore, ne za
  fizičke jezgre. To se može primijetiti kod procesora koji koriste
  Hyper-Threading gdje je broj procesora dvostruko veći od broja jezgri.
* Ako je u tijeku velika aktivnost diska, kao što je kopiranje velikih
  datoteka, moguća su kašnjenja prilikom dobivanja informacija o korištenju
  diska.
* Ovaj dodatak zahtijeva Windows 7 Service Pack 1 ili kasniji.

## Verzija 20.07

* Windows 10 verzija 20H2 pravilno se prepoznaje prilikom dohvaćanja
  podataka o Windows verziji (NVDA+šift+6).
* Pojednostavljena poruka verzije sustava Windows 10, tj. Windows 10 YYMM
  umjesto Windows 10verYYMM kad se pritisne NVDA+šift+6.

## Verzija 20.06

* Riješeni su mnogi problemi sa stilom kodiranja i potencijalnih grešaka sa
  Flake8.

## Verzija 20.04

* Ažurirana je psutil zavisnost na 5.7.0.

## Verzija 20.01

* Potrebna je verzija NVDA 2019.3 zbog iskorištavanja mogućnosti Pythona 3.

## Verzija 19.11

* Poboljšano otkrivanje za Windows Insider Preview gradnje, posebice za 20H1
  i nadalje.

## Verzija 19.07

* Ažurirana je psutil zavisnost na 5.6.3.
* Interna promjena za naredbu najavljivanja stanja baterija.

## Verzija 18.12

* Unutarnje promjene, kako bi se podržala buduća NVDA izdanja.

## Verzija 18.10

* Kod je sada kompatibilniji s Python 3.
* Ažurirana je psutil zavisnost na 5.4.7.
* Prilikom dobivanja kapaciteta diska i upotrebe memorije, NVDA više neće
  pogriješiti, ako koristi računalo ili uslugu s više od petabajta RAM-a ili
  veličine diska.
* Vrijednosti za memoriju i upotrebu diska prikazuju se s najviše dva
  decimalna mjesta (npr. 4,00 GB umjesto 4,0 GB).
* Poboljšano otkrivanje za Windows Insider Preview gradnje.

## Verzija 18.04

Verzija 18.04.x je posljednje izdanje koje će podržavati verzije Windowsa
starije od Windowsa 7 SP1.

* Posljednje izdanje koje podržava Windows Server 2003, Vistu i Server 2008.
* Poboljšano otkrivanje za Windowsa 10 izdanja i bolje razlikovanje između
  javnih i Insider Preview izdanja.

## Verzija 17.12

* Dodana podrška za 64-bitne ARM procesore na Windowsima 10.

## Verzija 17.09

Važno: Verzija 17.09 je posljednje izdanje koje podržava Windows XP.

* Zadnja verzija koja radi na Windowsima XP.
* Windows 10 verzija 16278 i novija prepoznata je kao Verzija 17.09. Manje
  izdanje ovog dodatka bit će objavljeno nakon objave stabilne verzije
  2017.9.

## Verzija 17.07.1

* Ponovo uvedena podrška za Windows XP (prekinuta od verzije 17.02).

## Verzija 17.05

* Najava trajanja pokretanja sustava (vrijeme proteklo od zadnjeg pokretanja
  računala); NVDA+Shift+7).

## Verzija 17.02

* Ažurirana je psutil zavisnost na 5.0.1.
* Tijekom provjere upotrebljivosti diska, NVDA više neće prikazivati
  dijaloški okvir pogreške na nekim sustavima gdje izmjenjivi medij nije
  ispravno prepoznat (primjerice kada kartica nije umetnuta u čitač
  kartica.)

## Verzija 16.08

Počevši od verzije 16.08, izdanja ovog dodatka prikazivat će se u formatu
godina.mjesec.izdanje.

* Različite verzije Windowsa 10 se sada ispravno prepoznaju (kao što je 1607
  za verziju 14393).
* Revizije Windows 10 gradnji (nakon instalacije kumulativnih ažuriranja)
  ispravno se prepoznaju (kao što je 14.393.51).
* Ako koristite Insider Preview gradnje, ta se činjenica prepoznaje.

## Promjene u verziji 4.5 ##

* Repozitorij dodatka premješten je na GitHub (možete ga pronaći na
  https://github.com/josephsl/resourcemonitor).
* Windows Server 2016. se ispravno prepoznaje.

## Promjene u verziji 4.0 ##

* Ažurirana je opsutil zavisnost na 2.2.1.
* Izrazito poboljšana učinkovitost pri dobivanju informacija o opterećenosti
  procesora.
* Dodana podrška za prepoznavanje Windowsa 10.
* U Windowsima 10, broj verzije Windowsa također će biti izgovoren.
* Moguće je koristiti Upravljač za dodatke za pristup pomoći.

## Promjene u verziji 3.1 ##

* „Prati stanje resursa” službeno podržava Windows 8.1.
* Ažurirani prijevodi.

## Promjene u verziji 3.0 ##

* Ažurirana psutil zavisnost na 1.2.1.
* Izgovor trenutne verzije Windowsa, arhitekture procesora i servisnog
  paketa ako postoji (NVDA+Shift+6).
* Mogućnost promjene tipkovnih prečica (NVDA verzija 2013.3 ili novija).
* Mogućnost kopiranja pojedinačnih informacija o resursima u međuspremnik
  pritiskom naredbi resursa dva puta.

## Promjene u verziji 2.4 ##

* Novi jezici: kineski (pojednostavljeni), ukrajinski.
* Ažurirani prijevodi.

## Promjene u verziji 2.3 ##

* Dodan prijevod na bugarski jezik.

## Promjene u verziji 2.2 ##

* Dodani prijevodi na sljedeće jezike: arapski, aragonski, hrvatski,
  nizozemski, finski, francuski, galicijski, njemački, mađarski, talijanski,
  japanski, korejski, nepaljski, poljski, portugalski (Brazil), ruski,
  slovački, slovenski, španjolski, tamilski i turski.

## Promjene u verziji 2.1 ##

* Ažurirana psutil zavisnost na verziju 0.6.1.
* Riješen problem velikog kašnjenja pri dobivanju informacija o particijama.
* Čišćenje koda.

## Promjene u verziji 2.0 ##

* Dodana podrška za prijevode i komentare prijevoda.

## Promjene u verziji 1.0 ##

* Prvo izdanje

[[!tag dev stable]]

[1]: https://addons.nvda-project.org/files/get.php?file=rm
