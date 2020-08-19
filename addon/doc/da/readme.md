# Ressourcemonitor #

* Authors: Alex Hall, Joseph Lee, beqa gozalishvili, Tuukka Ojala, Ethin
  Probst and other NVDA contributors
* Download [stable version][1]
* NVDA compatibility: 2019.3 to 2020.2

Dette tilføjelsesprogram giver information om CPU-belastning, brug af
hukommelse og andre oplysninger om forbrug af ressourcer.

# Genveje #

* NVDA+Shift+E: presents used ram, average processor load, and battery info
  if available.
* NVDA+Shift+1: presents the average processor load and if multicore CPU's
  are present the load of each core.
* NVDA+Shift+2/5: presents the used and total space for both physical and
  virtual ram.
* NVDA+Shift+3: presents the used and total space of the static and
  removable drives.
* NVDA+Shift+4: presents battery percentage, charging status, remaining time
  (if not charging), and a warning if the battery is low or critical.
* NVDA+Shift+6: presents CPU Architecture 32/64-bit and Windows version and
  service pack numbers.
* NVDA+Shift+7: presents the system's uptime.

If you have NvDA 2013.3 or later installed, you can change these shortcut
keys via input gestures dialog.

## Brugsanvisninger ##

Denne tilføjelse erstatter ikke Jobliste og andre
systeminformationsprogrammer til Windows. Bemærk også følgende:

* CPU-brug bliver angivet for logiske processorer, ikke fysiske
  kerner. Dette har betydning for processorer, som bruger
  hypertrådningsteknologi. Her er antallet af CPU'er er det dobbelte af
  CPU-kernerne.
* Hvis der er en stor mængde af diskaktivitet som f.eks. Kopiering af store
  filer, kan der være forsinkelser, når der hentes oplysninger om diskbrug.
* This add-on requires Windows 7 Service Pack 1 or later.

## Version 20.07

* Windows 10 Version 20H2 is properly recognized when obtaining Windows
  version information (NVDA+Shift+6).
* Simplified Windows 10 version message i.e. Windows 10 YYMM instead of
  Windows 10verYYMM when pressing NVDA+Shift+6.

## Version 20.06

* Resolved many coding style issues and potential bugs with Flake8.

## Version 20.04

* Updated psutil dependency to 5.7.0.

## Version 20.01

* NVDA 2019.3 or later is required due to extensive use of Python 3.

## Version 19.11

* Improved detection of Windows Insider Preview builds, especially for 20H1
  and beyond.

## Version 19.07

* Updated psutil dependency to 5.6.3.
* Internal changes to battery status announcement command.

## Version 18.12

* Internal changes to support future NVDA releases.

## Version 18.10

* Koden er blevet gjort mere kompatibel med Python 3.
* Opdateret psutil dependency til 5.4.7.
* Når der oplyses diskkapacitet og hukommelsesforbrug, vil NVDA ikke længere
  fejle, hvis du bruger en computer eller en tjeneste med mere end en
  petabyte RAM eller diskplads.
* Værdier for hukommelse og diskbrug vises med op til to decimaler (fx 4,00
  GB i stedet for 4,0 GB).
* Forbedret detektering af Windows Insider Preview builds.

## Version 18.04

Version 18.04.x er den sidste version, der understøtter udgaver af Windows
ældre end 7 SP1.

* Sidste version der understøtter Windows Server 2003, Vista og Server 2008.
* Forbedret detektion af udgaver af Windows 10 og bedre til at skelne mellem
  offentlige builds af Windows og Insider Preview.

## Version 17.12

* Tilføjet support til 64-bit ARM-processorer på Windows 10.

## Version 17.09

Vigtigt: Version 17.09.x er den sidste version, der understøtter Windows XP.

* Sidste version til at køre på Windows XP.
* Windows 10 build 16278 og senere er anerkendt som Version 1709. En mindre
  revision for denne tilføjelse frigives, når version 1709 stabil build er
  udgivet.

## Version 17.07.1

* Genindførte understøttelse for Windows XP (understøttelse har ikke virket
  siden version 17.02).

## Version 17.05

* Annoncering af systemopetid (tid gået siden sidste opstart, NVDA + Shift
  +7).

## Version 17.02

* Opdateret psutil afhængighed til 5.0.1.
* Når du kontrollerer diskbrug, vil NVDA ikke længere præsentere en
  fejldialog på nogle systemer, hvor et flytbart medie ikke er korrekt
  genkendt (f.eks. Når et kort ikke er indsat i en kortlæser).

## Version 16.08

Begyndende med version 16.08 vises tilføjelsespakkens fremtidige udgivelser
som år.måned.revision.

* Forskellige revisioner af Windows 10 er nu korrekt genkendt (f.eks. 1607
  til build 14393).
* Windows 10 build revisions (efter installation af kumulative opdateringer)
  er korrekt genkendt (såsom 14393.51).
* Hvis du bruger Insider-preview-builds, genkendes dette.

## Ændringer i 4.5 ##

* Tilføjelsespakkens udviklingssted er flyttet til GitHub (kan findes på
  https://github.com/josephsl/resourcemonitor).
* Windows Server 2016 er korrekt genkendt.

## Ændringer i4.0  ##

* Opdateret psutil dependency til 2.2.1.
* Stor forbedring af performance, under opsamlingen af oplysninger om
  CPU-belastning.
* Tilføjet understøttelse af genkendelse af Windows 10.
* I Windows 10 vil build-nummeret også blive annonceret.
* Du kan bruge Styring af tilføjelsesprogrammer til at få hjælp til
  tilføjelsesprogrammet.

## Ændringer i 3.1 ##

* Resource Monitor understøtter officielt Windows 8.1.
* Opdaterede oversættelser.

## Ændringer i 3.0 ##

* Opdateret psutil dependency til 1.2.1.
* Annoncering af Windows-version, CPU-arkitektur og service pack hvis nogen
  (NVDA+Shift+6).
* Mulighed for at ændre genvejstaster (NVDA 2013.3 eller senere).
* Muligt at kopiere individuelle ressourceoplysninger til udklipsholderen
  ved at ved at trykke på genvejstasten to gange.

## Ændringer i 2.4 ##

* Nye sprog: Kinesisk (simplificeret), ukrainsk.
* Opdaterede oversættelser.

## Ændringer i 2.3 ##

* Tilføjet bulgarsk oversættelse.

## Ændringer i 2.2 ##

* Tilføjet følgende oversættelser: Arabisk, aragonesisk, croatisk,
  hollandsk, finsk, fransk, galicisk, tysk, ungarsk, italiensk, japansk,
  koreansk, nepalesisk, polsk, portugisisk (Brasilien), russisk, slovakisk,
  slovensk, spansk, tamilsk og tyrkisk.

## Ændringer i 2.1 ##

* opdated psutil dependency til version 0.6.1.
* Rettet lang forsinkelse, når man bad om informationer om drev.
* Oprydning i koden.

## Ændringer i 2.0 ##

* Tilføjet understøttelse af oversættelse og oversættelseskommentarer.

## Ændringer i 1.0 ##

* Første udgivelse

[[!tag dev stable]]

[1]: https://addons.nvda-project.org/files/get.php?file=rm
