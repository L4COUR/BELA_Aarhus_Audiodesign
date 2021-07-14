# BELA for Audiodesign

BELA for audiodesign handler om at give studerende på audiodesign kandidaten adgang til at anvende de muligheder BELA boardet giver adgang til, med de forudsætninger man som audiodesigner lære eller har lært gennem kurserne Digital Lyd og Lyd & Interaktion.

### Indhold

- [Hvorfor anvende BELA?](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#hvorfor-anvende-bela)
- [Hardware](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#hardware)
- [Projekter lavet med BELA](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#projekter-lavet-med-bela)
- [Setup BELA](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#kom-igang-med-bela)

## Hvorfor anvende BELA?

Der findes mange microcontrollers der kan anvendes i en lydlig interaktiv sammenhæng. Fra [MakeyMakey](https://makeymakey.com/), [Arduino](https://www.arduino.cc/), [Teensy](https://www.pjrc.com/teensy/), [Raspberry Pi](https://www.raspberrypi.org/), [Axoloti](http://www.axoloti.com/), [Daisy](https://www.electro-smith.com/daisy), [BELA](https://bela.io/) og mange flere. Hvis du anvender BELA boardet fremfor de øvrige boards er det fordi du har brug for en robust og stabil platform der giver mulighed for "low-latency" interaktion.

![action-to-sound](./media/action-to-sound.png)

BELA beskriver latency som "Action-to-sound" og sammenligner deres latency på under 1 ms med andre platforme som arduino-to-Max eller Arduino-to-RaspberryPi, [her](https://www.nime.org/proceedings/2016/nime2016_paper0005.pdf) kan du læse mere om Latency og dets betydning i interaktive lyd konfigurationer

Den lave latency skyldes måde hvorpå BELA's software er opsat på. Den lydlige del af BELA er højest prioriteret gennem deres specialbyggede audioprocesserings miljø baseret på XenMai real-time Linux udvidelse, der kan læses mere om [her](https://bela.io/about)

![](https://bela.io/images/bela_software.png)

## Hardware

![](https://bela.io/images/bela_comparison.png)

BELA består af 8 kanaler af 16-bit analoge I/O, 16 digitale I/O, Stereo audio I/O, og 2 indbyggede højtaler forstærkere.

![](https://bela.io/images/products/bela.png)

## Projekter lavet med BELA

- https://blog.bela.io/2021/05/27/morph-gestural-interface-kuntay-seferoglu/
  - ![](https://blog.bela.io/assets/images/morph/morph_t.jpg)
  
- https://blog.bela.io/2018/09/14/Giraf-Bela-Hjalte-Bested-Moller/

  - ![](https://blog.bela.io/assets/images/giraf/insides.jpg)

- https://blog.bela.io/2021/07/01/case-western-university-embedded-computing/

  - ![](https://blog.bela.io/assets/images/case-course/breadboard.jpeg)

- BELA har indtil videre været anvendt til at bygge

  - musik instrumenter
  - kinetiske skulpture
  - wearable devices
  - interactive lyd installationer
  - effekt bokse
  - sensor eksperimenter
  -  papir kredsløb
  - e-tekstiler

  ... og meget meget mere

## Setup BELA

følg BELA's egen guide til at komme igang [her](https://learn.bela.io/get-started-guide/quick-start/)

### Step 1: Assemble and Plug in your hardware

- Når du har forbundet BELA med computer med USB kabel skal du vente ca. 40 sekunder mens BELA boomer op. Når BELA er klar vil dens blå LED blinke i et hjerteslagsbanken.
- Forbind headphones eller højtaler til BELA's Stereo out connecter med et audio adapter kabel.

### Step 2: Load BELA IDE

Audiodesigneren vil måske fra tidligere forløb på kurserne kende til arduino's IDE hvori arduino kode skrives og compiles. BELA's IDE køre gennem webbrowseren (anbefalet chrome) idet BELA genkendes af computeren som en USB netværks device.

- tjek om BELA's IDE er klar ved at åbne en webbrowser, og gå til "Http://bela.local" hvis systemet er klar vil du se denne side.
  - ![](https://learn.bela.io/assets/images/get-started-guide/ide_screenshot.png)
- Hvis siden ikke loader skal du installere en driver se instruktioner for dit styresystem
  - [Max OS X](https://learn.bela.io/using-bela/bela-techniques/network-setup/#mac-os-x)
  - [Linux](https://learn.bela.io/using-bela/bela-techniques/network-setup/#linux)
  - [Windows](https://learn.bela.io/using-bela/bela-techniques/network-setup/#windows)

### Step 3: Build an example project

Når IDE er ladet i browser, åben eksempler ved at trykke på el-pæren. klik på eksemplet kaldet [sinetone](https://learn.bela.io/tutorials/c-plus-plus/fundamentals/sinetone/). Når eksemplet compiles vil det producere en 440Hz sinus tone. Koden kan ses i editoren, såvel som i projekts filer.

I toolbaren i den nederste del af skærmen, klik "Run". Hvis det er første gang du kører et projekt gennem BELA kan der godt gå et minuts tid hvor boardet skal opsætte nogle folder etc forend sinus tonen høres.

![](https://learn.bela.io/assets/images/get-started-guide/ide_runbutton.gif)

Når Run-knappen er grøn og drejer rundt så virker systemet korrekt og du bør høre en tone komme ud af audio outputet fra BELA.

Hvis du kan køre sinetone eksempel projektet og du høre en tone komme fra boardet, virker boardet som det skal,

### Step 4: turning off BELA

Det er vigtigt at man [slukker for BELA boardet](https://learn.bela.io/using-bela/bela-techniques/shutting-down-bela/) på den rigtige måde for ikke at ødelægge boardet.

på boardet er en dedikeret sluk knap for boardet

![](https://learn.bela.io/assets/images/using-bela/bela-techniques/shutdown-button-cape.jpg)

Boardet kan også slukkes fra BELA's IDE

![](https://learn.bela.io/assets/images/using-bela/bela-techniques/shutdown-button.png)



## sources

- https://puredata.info/docs/tutorials/PdForMaxUsers
- https://learn.bela.io/get-started-guide/quick-start/
- https://learn.bela.io/using-bela/languages/pure-data/
- https://forum.bela.io/d/101-compiling-puredata-externals/98
- https://github.com/jarmitage/bela.pd