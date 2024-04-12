# nfc_business_card
Create and build your own business card on a PCB with NFC capability

## Step 1: Design your PCB
you would need to design your PCB to include your contact details, graphics and also select the dimensions of the card.
You can use my example by opening it using [EasyEDA Standard](https://easyeda.com/) to import the schematic and PCB json files or clone it from [this project on OSHWLAB] (https://oshwlab.com/info_4904/nfc-business-card)
I have also cloned the project at first from this one: https://oshwlab.com/shuchirj/nfc-business-card

## Step 2: Manufacture your PCB
I have used JLCPCB to manufacture the PCBs, it was easy to do and the results look great (they even remade part of the batch because they found scratches on some of the boards, so I got more boards eventually).

Here are the parameters I've used
#TODO: add jlcpcb parameters

One thing that I would like to think about for the next order is to also order a stencil since it makes the boards easier to assemble. A thing to note is, that if you've designed visible copper traces such as your name, they would be exposed in the stencil. In ordr to avoid that you'd need to review or design the stencil yourself. 

Here are the manufactured PCBs:
![alt text](https://github.com/barcesat/nfc_business_card/raw/master/pcb.jpg "Manufactured PCBs")

## Step 3: Order parts
To assemble the board, you would need these parts (Digikey links):
1. [1K memory NFC chip with I2C Interface](https://www.digikey.com/en/products/detail/nxp-usa-inc/NT3H2111W0FTTJ/5872979)
2. [0.22 uF Capacitor](https://www.digikey.co.il/he/products/detail/samsung-electro-mechanics/CL10B224KA8NNNC/3886769)
3. [47 Ohm Resistor](https://www.digikey.co.il/he/products/detail/yageo/RC0603FR-0747RL/727252)
4. [Red LED](https://www.digikey.co.il/he/products/detail/w%C3%BCrth-elektronik/150080RS75000/4489918)

To assemble the board you would need some kind of a solder paste like [this one](https://www.digikey.co.il/he/products/detail/chip-quik-inc/SMDLTLFP/2682721)

## Step 4: Assemble your board
![pcb](https://github.com/barcesat/nfc_business_card/assets/9979719/3b095e2d-df43-4225-813c-9dbabc531038)

The required tools are:
1. A hot plate or a hot air gun
2. A soldering Iron
3. A solder wick
4. tweezers to place tiny parts on the board
5. Some kind of a magnifying lens or microscope

Here are the assembled PCBs:
![alt text](https://github.com/barcesat/nfc_business_card/raw/master/assembled_pcb.jpg "Assembled PCBs")

#TODO: add assembly guide, cleaning and visual checkup

## Step 5: Program your board

![alt text](https://github.com/barcesat/nfc_business_card/raw/master/programmed_pcb.jpg "Programmed PCBs")

#TODO: add code

## Step 6: Write NFC records
I have used [NFC Tools](https://play.google.com/store/apps/details?id=com.wakdev.wdnfc&hl=en&gl=US&pli=1) to read the tag, create a contact URI record, and write it to the tag.![programmed_pcb](https://github.com/barcesat/nfc_business_card/assets/9979719/4d5683f2-a22c-467a-b51c-4314655f3536)
![programmed_pcb](https://github.com/barcesat/nfc_business_card/assets/9979719/100d1378-8614-402d-b954-b2a368212507)

#TODO: add screenshots
