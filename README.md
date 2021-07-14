# BELA for Audiodesign

BELA for audiodesign handler om at give studerende på audiodesign kandidaten adgang til at anvende de muligheder BELA boardet giver adgang til, med de forudsætninger man som audiodesigner lære eller har lært gennem kurserne Digital Lyd og Lyd & Interaktion.

### Indhold

- [Hvorfor anvende BELA?](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#hvorfor-anvende-bela)
- [Hardware](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#hardware)
- [Projekter lavet med BELA](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#projekter-lavet-med-bela)
- [Kom igang med BELA](https://github.com/L4COUR/BELA_Aarhus_Audiodesign/tree/main#kom-igang-med-bela)

## Hvorfor anvende BELA?

Der findes mange microcontrollers der kan anvendes i en lydlig interaktiv sammenhæng. Fra [MakeyMakey](https://makeymakey.com/), [Arduino](https://www.arduino.cc/), [Teensy](https://www.pjrc.com/teensy/), [Raspberry Pi](https://www.raspberrypi.org/), [Axoloti](http://www.axoloti.com/), [Daisy](https://www.electro-smith.com/daisy), [BELA](https://bela.io/) og mange flere. Hvis du anvender BELA boardet fremfor de øvrige boards er det fordi du har brug for en robust og stabil platform der giver mulighed for "low-latency" interaktion.

![action-to-sound](./media/action-to-sound.png)

BELA beskriver latency som "Action-to-sound" og sammenligner deres latency på under 1 ms med andre platforme som arduino-to-Max eller Arduino-to-RaspberryPi, [her](https://www.nime.org/proceedings/2016/nime2016_paper0005.pdf) kan du læse mere om Latency og dets betydning i interaktive lyd konfigurationer

Den lave latency skyldes måde hvorpå BELA's software er opsat på. Den lydlige del af BELA er højest prioriteret gennem deres specialbyggede audioprocesserings miljø baseret på XenMai real-time Linux udvidelse, der kan læses mere om [her](https://bela.io/about)

![](https://bela.io/images/bela_software.png)

## Hardware

![](https://bela.io/images/bela_comparison.png)

BELA består af 8 kanaler af 16-bit analoge I/O, 16 digitale I/O, Stereo audio I/O, og 2 indbyggede højtaler forstærkere.

## Projekter lavet med BELA

- https://blog.bela.io/2021/05/27/morph-gestural-interface-kuntay-seferoglu/
  - ![](https://blog.bela.io/assets/images/morph/morph_t.jpg)
- https://blog.bela.io/2018/09/14/Giraf-Bela-Hjalte-Bested-Moller/
  - ![](https://blog.bela.io/assets/images/giraf/insides.jpg)
- https://blog.bela.io/2021/07/01/case-western-university-embedded-computing/
  - ![](https://blog.bela.io/assets/images/case-course/breadboard.jpeg)

## Kom igang med BELA



## sources

- https://puredata.info/docs/tutorials/PdForMaxUsers
- https://learn.bela.io/get-started-guide/quick-start/
- https://learn.bela.io/using-bela/languages/pure-data/
- https://forum.bela.io/d/101-compiling-puredata-externals/98
- https://github.com/jarmitage/bela.pd