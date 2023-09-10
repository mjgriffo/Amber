# Amber + SolarEdge Export limiting
Solaredge export limit during low or negative Feed in Tarrif (FiT) 

This is a blueprint that automates the exporting of solarpower to the grid when using Amber as a power provider in Australia that offer real time enrgy market rates.
This means that duing periouds of high renewable energy generation that the price of the grid is negative. Meaning that you would "pay" to export power to the grid

This automation is based on several items 
# 1) SolarEdge HD Wave with consumption monitoring 
You will need to ensure that your solar system has the consumtion monitor option. This is so that the solar system knows how much power to 
generate to match your housees power demand. 
# 2) Amber as your power provider 
This is required to take advantage of the veriable rate that is on offer in the energy market leading to periods of low prices and also high prices 
# 3) Home assistant 
This is the software brain that is required to being the information to gether and drive action when conditions are met 
# 4) SolarEdge Modbus add on for Home assistant  - https://github.com/binsentsu/home-assistant-solaredge-modbus
This is the interface between home assistant and the SolarEdge inverter. This specific add-on is required as it privuides local control over your inverter 
It is critical that you have this module running before installing this blueprint as it will not be able to make any changes at all without it. 
The instructions on how to get this working are in the link above. you will know its off an running when you are able to see the details of your inverter in the 
Home assistant device and service page.
# 5) Amber integration for home assistant - https://www.home-assistant.io/integrations/amberelectric/
The Amber integration provides the pricing information about the grid to determin when you should be limiting production 
# 6) Import the  blueprint 
Once you have met all the above rewuirement import the blueprint with this link


      


