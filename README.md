Moj merilnik bo izmeril hitrost in smer vetra z Hall senzorjem (zaznava magnetnega polja in pošilja pulz) in s prostovrteče vrtljivi enkoder (ta bo izmeril smer vetra).

Opis naprave:

Naprava bo imelo oglato pravokotno ohišje z zunanjem anemometer in kazalec smeri vetra. Na anemometer je pritrjen neodim magnet in na bazi (spodnji del) je Hall senzor.
Za vsak čas, ko Hall senzor zazna neodim magnet, pošilja teh pulzov do mikrokontrolerja in potem izračuna hitrost, ki je odvisen od število vrtljajev na sekundo.
Mikrokontroler nato pošlje podatke LCDju in se potem prikazuje na njej. Za vrtljivi enkoder sem izbral enega, ki je prosto vrteče. Zaradi tega sem napisal kodo tako,
da za vsak obrat (360°) bo vrednost na LCDju vračal nazaj na začetnem položaju, tako, da dobimo 0-360° meritev. Nato nastopajo tipke, ampak so samo dva. Eden je za
menjavo enoto hitrosti vetra (m/s, km/h, kt) in ta drugi pa zamenja med stopinje (°) in smeri neba (N, E, W, S ipd.).

KOSOVNICA:
- Arduino Uno R3,
- Hall senzor A3144,
- KY-040 vrtljivi enkoder,
- 3D modelirano anemometer in kazalec smeri,
- perfBoard,
- Baterija z USB pretvornikom (za napajanje Arduino) in
- 3D modelirano ohišje.
