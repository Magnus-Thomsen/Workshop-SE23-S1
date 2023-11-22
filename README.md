# Workshop-SE23-S1
<span style="color:#FF0000">T</span><span style="color:#FF1900">h</span><span style="color:#FF3100">i</span><span style="color:#FF4A00">s</span> <span style="color:#FF6300">i</span><span style="color:#FF7B00">s</span> <span style="color:#FF9400">a</span> <span style="color:#FFAD00">p</span><span style="color:#FFC500">r</span><span style="color:#FFDE00">o</span><span style="color:#FFF700">j</span><span style="color:#EFFF00">e</span><span style="color:#D6FF00">c</span><span style="color:#BDFF00">t</span> <span style="color:#A5FF00">f</span><span style="color:#8CFF00">o</span><span style="color:#73FF00">r</span> <span style="color:#5AFF00">S</span><span style="color:#42FF00">D</span><span style="color:#29FF00">U</span> <span style="color:#10FF00">s</span><span style="color:#00FF08">o</span><span style="color:#00FF21">f</span><span style="color:#00FF3A">t</span><span style="color:#00FF52">w</span><span style="color:#00FF6B">a</span><span style="color:#00FF84">r</span><span style="color:#00FF9C">e</span> <span style="color:#00FFB5">e</span><span style="color:#00FFCE">n</span><span style="color:#00FFE6">g</span><span style="color:#00FFFF">e</span><span style="color:#00E6FF">n</span><span style="color:#00CEFF">e</span><span style="color:#00B5FF">e</span><span style="color:#009CFF">r</span><span style="color:#0084FF">i</span><span style="color:#006BFF">n</span><span style="color:#0052FF">g</span> <span style="color:#003AFF">2</span><span style="color:#0021FF">0</span><span style="color:#0008FF">2</span><span style="color:#1000FF">3</span> <span style="color:#2900FF">1</span><span style="color:#4200FF">.</span> <span style="color:#5A00FF">s</span><span style="color:#7300FF">e</span><span style="color:#8C00FF">m</span><span style="color:#A500FF">e</span><span style="color:#BD00FF">s</span><span style="color:#D600FF">t</span><span style="color:#EF00FF">e</span><span style="color:#FF00F7">r</span> <span style="color:#FF00DE">w</span><span style="color:#FF00C5">o</span><span style="color:#FF00AD">r</span><span style="color:#FF0094">k</span><span style="color:#FF007B">s</span><span style="color:#FF0063">h</span><span style="color:#FF004A">o</span><span style="color:#FF0031">p</span><span style="color:#FF0019">.</span> :boom::boom::boom::boom::boom::boom::boom::boom::boom::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo::man_playing_water_polo:

## Sprint 2

### Kravspecifikation
| Krav ID | Navn                     | Beskrivelse                                                                                                                                                                                                                                                                                   |
|---------|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| F01     | Tilføjelse af bygning    | Det skal være muligt at tilføje en bygning til systemet. En bygning er kendetegnet ved et unikt navn,                                                                                                                                                                                         |
| F02     | Fjernelse af bygning     | Det skal være muligt at fjerne en bygning fra systemet, hvorved sensorer og aktuatorer associeret med bygningen også fjernes.                                                                                                                                                                 |
| F03     | Tilføjelse af sensor     | Det skal være muligt at tilføje en sensor til systemet og associere denne med en bygning. En sensor er kendetegnet ved et unikt navn, en type (CO2/Temperatur) og dens nuværende værdi. Værdien er indtil videre bare en dummyværdi, da der i dette system ikke skal interfaces mod hardware. |
| F04     | Fjernelse af sensor      | Det skal være muligt at fjerne en given sensor fra systemet, hvorved den fjernes fra den bygning som den er associeret med.                                                                                                                                                                   |
| F05     | Tilføjelse af aktuator   | Det skal være muligt at tilføje en aktuator til systemet og associere denne med en bygning. En aktuator er kendetegnet ved et unikt navn, en type (kun ventilation indtil videre), og dens nuværende setpunkt.                                                                                |
| F06     | Ændring af aktuatorværdi | Det skal være muligt at ændre setpunkts-værdien for en aktuator.                                                                                                                                                                                                                              |
| F07     | Hent aktuatorværdi       | Det skal være muligt at udlæse setpunktsværdien for en given aktuator.                                                                                                                                                                                                                        |
| F08     | Hent sensorværdi         | Det skal være muligt at udlæse værdien for en given sensor.                                                                                                                                                                                                                                   |
| F09     | Liste over bygninger     | Det skal være muligt at hente en liste over bygninger der er tilføjet til systemet.                                                                                                                                                                                                           |
| F10     | Liste over aktuatorer    | Det skal være muligt at hente en liste over aktuatorer associeret med en given bygning.                                                                                                                                                                                                       |
| F11     | Liste over sensorer      | Det skal være muligt at hente en liste over sensorer associeret med en given bygning.                                                                                                                                                                                                         |
| F11     | Fjernelse af Aktuator    | Det skal være muligt at fjerne en given aktuator fra systemet, hvorved den fjernes fra den bygning som den er associeret med                                                                                                                                                                  |
### Noun/Verb Analyse

| Verb      | Noun       |
|-----------|------------|
| Move      | rooms      |
| Build     | player     |
| Generate  | village    |
| Repair    | town       |
| Wear Down | city       |
|           | road       |
|           | railway    |
|           | currency   |
|           | durability |
|           | ticks      |

### CRC Kort

| Bygning Handler                 |                        |
|---------------------------------|------------------------|
| **Ansvarsområde**               | **Samarbejdspartnere** |
| Lave en oversigt over bygninger | Bygning                |
| Tilføj Bygning                  |                        |
| Fjern Bygning                   |                        |

| Bygning                                                      |                        |
|--------------------------------------------------------------|------------------------|
| **Ansvarsområde**                                            | **Samarbejdspartnere** |
| Holde styr på hvilket sensorer der er tilknyttet bygningen   | Sensor                 |
| Holde styr på hvilket aktuatorer der er tilknyttet bygningen | Aktuator               |
| Tilføj sensorer og aktuatorer til bygning                    |                        |
| Fjern sensorer og aktuatorer fra bygning                     |                        |

| Sensor              |                        |
|---------------------|------------------------|
| **Ansvarsområde**   | **Samarbejdspartnere** |
| Læs data fra sensor |                        |

| Co2 Sensor              |                        |
|-------------------------|------------------------|
| **Ansvarsområde**       | **Samarbejdspartnere** |
| Opbevarer måling af Co2 |                        |

| Temperatur Sensor            |                        |
|------------------------------|------------------------|
| **Ansvarsområde**            | **Samarbejdspartnere** |
| Opbevar måling af Temperatur |                        |

| Aktuator               |                        |
|------------------------|------------------------|
| **Ansvarsområde**      | **Samarbejdspartnere** |
| Hent data fra aktuator |                        |
| Ændre aktuator værdi   |                        |

### UML Diagram
