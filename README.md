# pin-led
A small RGB LED board that can be mounted on pinball playfields.
The board uses neopixel LEDs (WS2812B), which can be chained using only three
wires: power (5V), ground, and data.

<img src="/images/pin-led_pcbs.jpg">

The boards are panelized into 100mm x 100mm pcbs for easy and inexpensive 
ordering from JLCPCB.com (or other fabs).  I recommend using their SMT
assembly to populate the LEDs and the capacitors during manufacturing.

There are two pcb options: a stamp hole panel that easily breaks apart, and a
nocut layout that must be cut manually later on.

## Nocut board
The uncut pcb has a dense layout yielding 27 boards (3x9).  This is the most
economical option, but it requires cutting the pcb manually later on, which is
surprisingly difficult.  The total cost, including the cheapest shipping option
at jlcpcb was about $25 for five populated panels, for a total of 135 
boards.

<img src="/images/pin-led_pcb.jpg">

I tried a bunch of different options to cut the boards apart.  The best one was
using a mini tablesaw with a thin 4 inch diamond blade (Amazon carries these 
for ~$70, Harbor Freight has one for ~$40). 

Scoring the pcb with a knife or scoring tool kind of works, but it takes a 
lot of work and a lot of long time.  It's also easy to slip and mess up and
the resulting breaks are not very clean.

I also tried using a scroll saw, but the boards are so snmall that the blade
guard was often not able to hold them down.  

<img src="/images/pin-led_glass.jpg">

A more convenient option is the stamp hole layout, where the boards are cut 
during manufacturing and can be broken apart easily.  

## Stamp Hole
The stamp hole panel yields only 21 led boards (3x7) due to the need for
edge rails and a minimum cut width of 1.6mm.  

Another drawback is that jlcpcb contacted me after reviewing my order to
charge an additional $12 because the panel requires too much cutting time.
This brings the total cost including shipping to $35 for 105 populated boards.
Still a great deal overall and no mess cutting the boards yourself.

## V-cut
My actual preferred option would have been a v-cut panel, but jlcpcb does not
offer SMT assembly for v-cut panels, as they may warp during the reflow 
soldering.

# PCB design software
I used EasyEDA v6.4.7 to design these pcbs.  It's a free software offered by 
jlcpcb that can be used online or downloaded and installed.  Major benefits 
were support for the jlcpcb parts catalog to build the BOM and excellent 
support for panelizing (something that I couldn't figure out in KiCad).
