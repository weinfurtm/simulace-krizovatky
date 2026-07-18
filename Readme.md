# Simulace krizovatky

Interaktivni lokalni simulace dvou aut v pravouhle krizovatce.

## Spusteni

Otevrete `index.html` v prohlizeci. Aplikace nepotrebuje instalaci zavislosti ani build krok.

## Co model pocita

- rychlosti se zadavaji v metrech za sekundu,
- startovni vzdalenosti a bod vyboceni se zadavaji v metrech od referencniho mista stretu,
- referencni misto stretu lze korigovat vodorovne a svisle v metrech,
- modre auto jede zleva doprava konstantni rychlosti,
- cervene auto jede zespodu nahoru ve ctyrpruhovem smeru,
- cervene auto muze jet rovne nebo diagonalne vybocit doprava,
- uhel diagonalniho vyboceni cerveneho auta je nastavitelny,
- kolize se pocita jako prunik obdelniku aut,
- porovnani rovne jizdy pouziva stejne rychlosti a stejne vychozi body jako diagonalni scenar.
- pokud zvolena trasa vede ke kolizi, prehravani se zastavi v case prvniho kontaktu.

## Meritko

Vypocet pracuje v metrech a sekundach. Canvas pouze prevadi polohy pro zobrazeni v meritku `10 px = 1 m`.

Referencni misto stretu je uprostred 3. pruhu zprava ve viceproude silnici. Vzdalenost modreho auta se meri doleva od tohoto bodu, vzdalenost cerveneho auta dolu od tohoto bodu. Korekce mista stretu posouva tento referencni bod; kladna vodorovna korekce jde doprava a kladna svisla korekce dolu v pohledu shora.

## Omezeni

Model neresi brzdeni, akceleraci, reakci ridice, presnou dynamiku zataceni ani znaleckou rekonstrukci podle presneho zamereni mista
