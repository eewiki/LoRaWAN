# Advantech WISE-4610 related code 

WiseParserV1_6_8_TTNmod.js is an Advantech Javascript payload decoder that has been modified for use in The Things Stack LoRaWAN server (TTN). 

Advantech provides a reference Javascript payload parser for raw data of WISE-2410 and WISE-4610 series. It is intended to be helpful for use with a 3rd party LoRaWAN gateway. Advantech's 1.6.8 version was used as a starting point for a decoder but needed to be modified to run as a payload decoder in The Things Stack (TTN). Advantech has an application note "IAG_FAQ WISE-2000 How to receive LoRa end node data payload and parse data on TTN_20200312.pdf" that goes into detail of the modifications needed. The app note can be found at below link:
https://advdownload.advantech.com/productfile/Downloadfile3/1-1VWSIJH/IAG_FAQ%20WISE-2000%20How%20to%20receive%20LoRa%20end%20node%20data%20payload%20and%20parse%20data%20on%20TTN_20200312.pdf 
Addititional changes made were to remove all code references to "console.log" since those references caused errors in the TTN payload decoder.

The latest version of Advantech's payload parser and associated documentation can be found at link https://www.advantech.com/en/support/details/utility?id=1-1UAZL7H .

note: the latest available version, 1.6.12, is too large to be easily used as a starting point for a TTN Javascript decoder since it exceeds the maximum size 
limit of 40 KB as specified by The Things Network at https://www.thethingsindustries.com/docs/integrations/payload-formatters/javascript/ .
