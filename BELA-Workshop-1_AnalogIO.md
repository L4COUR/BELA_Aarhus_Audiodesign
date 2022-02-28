# BELA Workshop 1: Analog I/O
I denne workshop skal de studerende prøve kræfter med analoge inputs og outputs (i/o) på BELA boardet.

![](./media/BELA_AnalogIO.png)

### BOM
- 1 x Pot
- 1 x LED
- 1 x LDR
- 1 x Breadboard
- 2 x resistors
- 10 x jumper wires
- 1 x BELA board
- (electrical tape)
![](./media/BELAWorkshop1BOM.jpg)
## Analog Input
Der findes mange forskellige analoge input sensorer. Eksempler på disse er

- accelerometre
- pressure sensor
- light sensor
- sound sensors
- temperature sensors
- ...

I denne workshop anvendes potentiometre og LDR som analoge inputs.

![Potentiometer](https://www.digikey.dk/-/media/Images/Article%20Library/TechZone%20Articles/2021/May/The%20Fundamentals%20of%20Digital%20Potentiometers%20and%20How%20to%20Use%20Them/article-2021may-the-fundamentals-of-digital-fig1.jpg?la=en&ts=7103c327-388b-4a84-8620-851590a9ec9f)

![LDR-breadboard](./media/LDRBreadboardCircuit.png)

Alle de kredsløb vi skal bygge sker vha. breadboards
![](https://components101.com/sites/default/files/component_pin/Breadboard-Pinout.png)

### Potentiometer til BELA
![](https://learn.bela.io/assets/images/fritzing/pd//analog-input.png)

- Byg et simpelt kredsløb med potentiometeret i forbindelse med BELA boardet
	- Identificer potentiometrets pinouts
	- Identificer hvor på boardet de forskellige pins fra potentiometret skal tilsluttes
- [Creating a Pd Project](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#creating-a-pd-project)
- download _main.pd og rediger i Pure Data
- overwrite filen på boardet med din egen fil

- [adc~ 3 4 5 6 7 8 9 10] = Bela's 8 analoge inputs.

![](./media/BELA_debuggerTool.png)

- Anvend ovenstående objekter i pd for at logge værdier fra potentiometret til BELA's consol.
- Lav et system med BELA hvor et potentiometer bestemmer lydstyrken af en 440 hz sinus tone.

## Analog Output
Der findes mange forskellige analoge outputs sensorer. Eksempler på disse er

- LED
- motorer (servo, stepper etc.)
- solenoid
- DAC
- relay
- graphic displays (OLED, LCD etc.)
- ...

I denne workshop anvendes LED som det analoge output.

![](./media/BELAAnalogOut.png)

- Byg et simpelt kredsløb med LED i forbindelse med BELA boardet
- [Creating a Pd Project](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#creating-a-pd-project)
- download _main.pd og rediger i Pure Data
- overwrite filen på boardet med din egen fil
- [dac~ 3 4 5 6 7 8 9 10] = Bela's 8 analoge outputs.

## Vactroler
![](https://content.instructables.com/ORIG/FDN/1TFH/K0R1JGKR/FDN1TFHK0R1JGKR.jpg?auto=webp&frame=1&crop=3:2&width=320&md=a4660a600323ac2d0d3102e7c6d855f1)

- En vactrol er en kombination af Light Dependent Resistors (LDR) og en lys kilde i en beskyttet lys-resistent kasse.
- Vactroler er anvendt i filtre, forstærkere, phaser, trigger delays, slew limiters, envelope generators, LFO'er og oscillatorer der eksempelvis i eurorack skal kunne kontrolleres gennem control voltage (CV) se [Doepfers side om vactroler](https://doepfer.de/a100_man/Vactrol.htm)
- Jeres erfaring fra hvordan man tilslutter BELA med dets analoge inputs og outputs kan bruges til at eksperimentere med vactroler.

### Vactrol oscillator
![](./media/BELAsimpelVactrolCircuit.png)

- Byg et kredsløb med LED og LDR koblet til BELA.
- [Creating a Pd Project](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#creating-a-pd-project)
- download _main.pd og rediger i Pure Data
- overwrite filen på boardet med din egen fil

![](./media/LDRLEDBELA.png)

- Overvej hvordan disse værdier kan bruges i forhold til at lave en oscillator, voice der skal komme ud af BELA's stereo output

![](./BELA-VactrolOSC/BELAVactrolOSCcircuit.png)

![](./BELA-VactrolOSC/VactrolCircuit.png)

- [andre workshops](./README.md)