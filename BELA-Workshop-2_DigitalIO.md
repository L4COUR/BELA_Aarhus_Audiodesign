# BELA Workshop 1: Digital I/O
I denne workshop skal de studerende prøve kræfter med Digitale inputs og outputs (i/o) på [BELA boardet](https://learn.bela.io/pin-diagram/).

### BOM
- 1 x LED
- 1 x button
- 1 x Breadboard
- 2 x resistors
- 10 x jumper wires
- 1 x BELA board

![](https://static.wixstatic.com/media/7736d7_ec5d8a00c01a4f3aae53403cfb69f072~mv2.jpg/v1/fill/w_600,h_400,al_c,q_90/7736d7_ec5d8a00c01a4f3aae53403cfb69f072~mv2.jpg)


## Digital Output
![](https://cdn-learn.adafruit.com/assets/assets/000/035/419/medium800thumb/components_halfbb.jpg?1472966532)

- lav kredsløb med LED og resistor
- find ud af hvor på BELA boardet den positive udgang af LED skal placeres.

### koden
- Først skal den digitale pin initialiseres

![](https://learn.bela.io/assets/images/tutorials/pd/digital-output-1.png)

- For at få LED'en til at blinke

![](https://learn.bela.io/assets/images/tutorials/pd/digital-output-2.png)

## Digital Input
En stor forskel til BELA's analoge pins er at de digitale pins i sig selv kan initieres som enden input eller output.

![](https://learn.bela.io/assets/images/fritzing/pd//digital-input.png)

I følgende eksempel anvendes en knap, men der findes naturligvis andre former for digitale inputs componenter

- kontakt
- relay
- PIR sensor
- rotary encoder
- proximity sensor
- IR sensor
- ...

![](https://components101.com/sites/default/files/component_pin/Push-button-Pinout.gif)

### kode
- de digital pins initialiseres som hhv. input og output

![](https://learn.bela.io/assets/images/tutorials/pd/digital-input-1.png)

- herefter anvendes [s] & [r] objekter for hhv. at sende og modtage det digitale signal.

![](https://learn.bela.io/assets/images/tutorials/pd/digital-input-2.png)


## Installering af Externals
- [Cyclone Install guide](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#cyclone-on-bela)

## Opgave
Kombiner Det i har lært om digitale og analoge I/O i et system hvori der i pure data anvendes [cyclone objekter](http://suita.chopin.edu.pl/~czaja/miXed/externs/cyclone.html) samt afvikling af en lydfil efter eget ønske. Systemet må nødvendigvis indeholde;

- Analoge input (pot eller LDR)
- Analoge/Digitale output (LED)
- Digital input (button)
- Puredata kode med cyclone objekter