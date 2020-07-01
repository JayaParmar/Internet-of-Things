*For the product purchase details, please see “Bill of Materials” spreadsheet* here https://github.com/JayaParmar/Internet-of-Things/blob/master/images/Bill%20of%20materials.xlsx

**Floor Plan**

![](/images/Floor%20plan.jpg)

**Networking Hub**

![](/images/F1_Networking%20Hub.jpg)


Ubiquiti Unifi products are chosen for networking since I found them modular and scalable which is a good option for future expansion.

1.  > Gateway

<!-- end list -->

  - > 12V DC supply, power adapter included in the packet

  - > 500 MHz processor, dual core

  - > Supports voltage range from 9 to 24V DC

  - > Can carry packet size of 64 bytes at 1000000 pps and 512 bytes or more at 3 Gbps

Specifications Source:

[<span class="underline">https://dl.ubnt.com/qsg/USG/USG\_EN.html</span>](https://dl.ubnt.com/qsg/USG/USG_EN.html)

2.  > Switch

> The reason for selecting Switch 8-150W is it provides 8 PoE ports. We are using 1 PoE for input from gateway and 4 PoE connections for output to 4 floors. This provides a good option for scalability in the future. There is also 2 SFP ports for optical fiber cable connection, if needed.

  - > AC/DC power supply, internal, 150W DC

  - > Speed 1Gbps

  - > Networking PoE 10/100/1000 Mbps RJ45 ports

  - > PoE ports supply 24V DC

Specifications Source:

[<span class="underline">https://dl.ubnt.com/guides/UniFi\_Switch/US-8-150W\_QSG.pdf</span>](https://dl.ubnt.com/guides/UniFi_Switch/US-8-150W_QSG.pdf)

3.  > Controller

> Is connected to the PoE port in the Switch to access the LAN and the gateway. One can plug in a computer into another PoE port at switch and monitor the status of the network.
> 
> Controller/Cloud Key can also be accessed remotely.

  - > 5 W power consumption

Read below link to datasheet for further details

[<span class="underline">https://dl.ubnt.com/datasheets/unifi/UniFi\_Cloud\_Key\_DS.pdf</span>](https://dl.ubnt.com/datasheets/unifi/UniFi_Cloud_Key_DS.pdf)

With these three devices, we have the basic communication network setup to make our house a smart home. Later, we will provide an AC in wall unit on each floor (2,3 and 4) to provide ethernet and WiFi connection with basic PoE connection. Floor 1 will use the outdoor WiFi unit.

**Garage & Outdoor**

![](/images/F1_Garage%20%26%20Outdoor%20Area.jpg)

Devices here have wireless connectivity to gateway because outdoor has security issues.

1.  > Outdoor WiFi unit

<!-- end list -->

  - > Power Supply 24V, 0.5 A Gigabit Power Adapter included

  - > Max power consumption 8.5W

  - > Range 183 m

  - > Throughput Speed 300 Mbps at 2.4GHz and 866 Mbps at 5 GHz

  - > Supported voltage range is 44 to 57 V DC

WiFi unit is weatherproof and right now only security camera uses the 2.4GHz frequency and 1.2 Mbps bandwidth on a high quality resolution. Thus there is bandwidth to connect lawn sprinkler/small irrigation system for the outdoor area in summer/future.

Specification Source:

[<span class="underline">http://dl.ui.com/guides/UniFi/UniFi\_AP-AC-M\_QSG.pdf</span>](http://dl.ui.com/guides/UniFi/UniFi_AP-AC-M_QSG.pdf)

2.  > Security Camera

<!-- end list -->

  - > Can be connected to 230 V input directly

  - > Can be accessed from anywhere via Nest app

  - > Inbuilt motion detector

  - > 2 way sound to allow voice communication

  - > Weather-proof and can see in the dark

Specifications Source -

> [<span class="underline">https://support.google.com/googlenest/answer/9259110?hl=en</span>](https://support.google.com/googlenest/answer/9259110?hl=en)

3\. Outdoor Light

  - > Can be connected to 230 V input directly

  - > LED with motion sensor

> Light is activated by motion and is weatherproof. It does not need connectivity frequency hence this choice.

Specifications Source -

[<span class="underline">https://www.hornbach.se/data/shop/D04/001/780/491/145/730/6291540\_Doc\_02\_DE\_20180924094651.pdf</span>](https://www.hornbach.se/data/shop/D04/001/780/491/145/730/6291540_Doc_02_DE_20180924094651.pdf)

4\. Garage door sensor

> This is a simple magnet sensor with LED indication for the open/close status of the door. The status is shown on the smartphone so you can check of garage door sitting in the living room in case you think you forgot to close it.

Specification details

[<span class="underline">https://sensative.com/strips/guard/</span>](https://sensative.com/strips/guard/)

5\. Garage Indoor Light

> This is a light activated by motion. It can withstand temperature between -20 to +40C and can be used in garage. Chose this light since I did not find the need for it to be connected with the gateway.

**Kitchen**

![](/images/F2_Kitchen.jpg)

The network connectivity for floor 2 is provided by AC in wall unit installed in the kitchen (directly above the networking hub).

1.  > In-wall Unit (Floor 2 connectivity)

> This unit is placed towards the living room near the toilet wall. We assume that all indoor walls are softwalls and only outdoor walls are hardwalls. Thus the positioning of the in-wall unit will be close to the center of the floor.

It provides WiFi connectivity with two ethernet enabled ports

  - > Power Supply - UniFi Switch

  - > Max power consumption 7W (with PoE 19W)

  - > PoE Out 48V

  - > Range 100 m

  - > Data Speed 300 Mbps at 2.4GHz and 866 Mbps at 5 GHz

Specification Source:

[<span class="underline">https://dl.ui.com/guides/UniFi/UniFi\_UAP-AC-IW\_QSG.pdf</span>](https://dl.ui.com/guides/UniFi/UniFi_UAP-AC-IW_QSG.pdf)

2.  > Temperature Sensor

> This is a WiFi Socket with an integrated temperature sensor that enables to adjust the temperature of mechanical thermostat in the Millheat App from anywhere. It has a maximum capacity of 2300 W and uses the 2.4GHz frequency.

Specification Source:

[<span class="underline">https://www.millheat.com/mill-wifi/wifisocket-x4bkm</span>](https://www.millheat.com/mill-wifi/wifisocket-x4bkm)

3.  > Kitchen Light

> Here we use Philips Hue smart LED lights GU10. These can be WiFI controlled and have white to coloured lights in a spectrum. The dining table in the kitchen is used for study sometimes by the family and sometimes to set the mood when guests are home. Hence it is convenient to have the different shades of lights.

  - > Max power consumption 5.7 W

  - > Life 15 000 h

Specification Source:

[<span class="underline">https://www2.meethue.com/sv-se/p/hue-white-och-color-ambiance-startpaket-gu10/8718699629274</span>](https://www2.meethue.com/sv-se/p/hue-white-och-color-ambiance-startpaket-gu10/8718699629274)

4.  > Smoke Detector

We buy one pair of WiFi enabled interconnected smoke alarm to detect accidental smoke from the kitchen area. Alarm is kept at a reasonable distance to avoid false alarm trigger from cooking. The detector can be interconnected upto 12 units via WiFi for future scalability. On Blac Friday discount we got 2 units at a price of 1. We install one of them on Floor 2 and the other one can be used on Floor 3 but right now we keep it as a spare.

**Living Room**

![](/images/F2_Living%20Room.jpg)

1.  > Door Bell

> Although there is a security camera at the garage entrance, we prefer a security camera at the entrance to the building since a camera can miss a burglar outside its view scope. Later we will install one more camera on the top floor at the balcony door.
> 
> Nest Hello is a doorbell with a camera which can send you an alert when someone approaches even if they don’t ring the bell.

Specification Source:

[<span class="underline">https://store.google.com/us/product/nest\_hello\_doorbell\_specs?hl=en-US\&GoogleNest</span>](https://store.google.com/us/product/nest_hello_doorbell_specs?hl=en-US&GoogleNest)

2.  > Smart TV

> TV controlled with WiFi, voice and bluetooth; a7 processor with AI, 4K cinema HDR and 148 kW power consumption per year.

Specification Source:

[<span class="underline">https://www.lg.com/se/lgoled-tv/lineup.jsp?cmpid=2019HQSEM\_OLED-TV\_SW\_Google\_OLED\_Brand-Core\_Exact\_Model\_k4461\_pc\&gclid=Cj0KCQiAt\_PuBRDcARIsAMNlBdqZRZnrzMF9wO2vmwuRnr-5\_Gy18iM540-fiecszrutu4Af7Sm87ccaAuWcEALw\_wcB</span>](https://www.lg.com/se/lgoled-tv/lineup.jsp?cmpid=2019HQSEM_OLED-TV_SW_Google_OLED_Brand-Core_Exact_Model_k4461_pc&gclid=Cj0KCQiAt_PuBRDcARIsAMNlBdqZRZnrzMF9wO2vmwuRnr-5_Gy18iM540-fiecszrutu4Af7Sm87ccaAuWcEALw_wcB)

3.  > Temperature Controller

> This is a WiFi Socket with an integrated temperature sensor that enables to adjust the temperature of mechanical thermostat in the Millheat App from anywhere. It has a maximum capacity of 2300 W and uses the 2.4GHz frequency.

Specification Source:

[<span class="underline">https://www.millheat.com/mill-wifi/wifisocket-x4bkm</span>](https://www.millheat.com/mill-wifi/wifisocket-x4bkm)

4.  > Ceiling Light

> A 3000 lumen smart light above the seating area in the living room is good luminosity to light the area. Light has a life of 25 000 hours.

Specification Source:

[<span class="underline">https://www2.meethue.com/sv-se/p/hue-white-ambiance-cher-taklampa/4096730P7?origin=rcWEvjT6\&pcrid=341992782422|mckv|srcWEvjT6\_dc|plid||slid||\&gclid=Cj0KCQiAt\_PuBRDcARIsAMNlBdr-UlEhtUuRIkZRgLuyfYde9HIiO0DBaZKDfiSamFvZtOFxUM19TysaAp8wEALw\_wcB</span>](https://www2.meethue.com/sv-se/p/hue-white-ambiance-cher-taklampa/4096730P7?origin=rcWEvjT6&pcrid=341992782422%7Cmckv%7CsrcWEvjT6_dc%7Cplid%7C%7Cslid%7C%7C&gclid=Cj0KCQiAt_PuBRDcARIsAMNlBdr-UlEhtUuRIkZRgLuyfYde9HIiO0DBaZKDfiSamFvZtOFxUM19TysaAp8wEALw_wcB)

5.  > Entrance Lamp

> This is a lamp with a motion sensor and lights up as soon as the door is opened. 600 lumen is sufficient for the entrance.

6.  > Passage Spot Lights

> A set of three spot lights would cover the passage area from entrance to the living room. Details for the lights can be found below

Specification Source:

[<span class="underline">https://www2.meethue.com/sv-se/p/hue-white-ambiance-infalld-spot/3407511P7</span>](https://www2.meethue.com/sv-se/p/hue-white-ambiance-infalld-spot/3407511P7)

There could be devices like smartphones, laptops and computers on this floor using the WiFi capacity which are not shown in the Bill of Materials.

**Staircase F2**

We have a light with motion detector which turns on when someone climbs the stairs.

**Master Bedroom**

![](/images/F3_Master%20Bedroom.jpg)

1.  > In-wall Unit (Floor 2 connectivity)

> This unit is placed towards the master bedroom near the toilet wall. We assume that all indoor walls are softwalls and only outdoor walls are hardwalls. Thus the positioning of the in-wall unit will be close to the center of the floor.

It provides WiFi connectivity with two ethernet enabled ports

  - > Power Supply - UniFi Switch

  - > Max power consumption 7W (with PoE 19W)

  - > PoE Out 48V

  - > Range 100 m

  - > Data Speed 300 Mbps at 2.4GHz and 866 Mbps at 5 GHz

Specification Source:

[<span class="underline">https://dl.ui.com/guides/UniFi/UniFi\_UAP-AC-IW\_QSG.pdf</span>](https://dl.ui.com/guides/UniFi/UniFi_UAP-AC-IW_QSG.pdf)

2.  > Smart Vacuum Cleaner:

> We assume that there is a manual vacuum cleaner on Floor 2. The reason for this assumption is that most of the awake times family is on floor 2. Floor 3 is mostly used for sleeping and bathing. Hence it is easy to start cleaning this area while on Floor 2. We can ofcourse buy a smart vacuum cleaner for each floor in future.
> 
> For product details, please read below

Specification Source:

[<span class="underline">https://store.irobot.com/default/roomba-vacuuming-robot-vacuum-irobot-roomba-671/R671020.html</span>](https://store.irobot.com/default/roomba-vacuuming-robot-vacuum-irobot-roomba-671/R671020.html)

Other smart devices used in this room are already described above. For more details, please go to the ‘Bill of Materials’ sheet to read the product name, cost and link for where it is bought from the market.

**Kids Bedroom**

![](/images/F3_Kids%20Bedroom.jpg)

This room has two lights and a temperature sensor. The smart devices are similar to ones in the master bedroom. Read the ‘Bill of Materials’ for more details.

**Toilet + Bathroom**

Small kids in the house can forget to turn off the tap or lights after they use this area. Hence a water leak detector and light with motion sensor is used here. In case water on floor goes above 0.5 millimeter, there will be a message on phone warning leakage. The lights are turned off after the kids exit the bathroom.

There could be laptops, computers, smartphones or tablets on this floor but we have connectivity and bandwidth to support all these devices.

**Staircase F3**

Again, we have a light with motion detector which turns on when someone climbs the stairs.

**Guest Bedroom**

![](/images/F4_Guest%20Bedroom.jpg)

This room houses the last in-wall unit i.e. for floor 4. Like other bedrooms it has a ceiling light and a temperature controller. Details of the products can be found in the Bill of Materials.

**Study**

![](/images/F4_Study.jpg)

This is a room with three light sources and a temperature controller. Computers, music system or any other recreation devices can be connected in this room based on the mood. Connectivity both ethernet and wireless is available from Ubiquiti in-wall unit. Production details found in Bill of Materials.

**Balcony**

![](/images/F4_Balcony.jpg)

The balcony door at Floor 4 is one more entrance to the house. Since the family does not spend most time on this floor, we plan to install a security system here. Smart devices needed would be a security camera, a motion sensor, a door open sensor, a siren and connectivity to the smartphone.

We would have preferred to use the Google Nest security system like this one [<span class="underline">https://www.bigapplebuddy.com/product/8/nest-secure-alarm-system-white/14374?child\_sku=6080402\&utm-medium=pla\&utm-co=SE\&gclid=CjwKCAiA\_f3uBRAmEiwAzPuaM1tlnx5Rmbx6hAUAP7Z\_zMQzLrarA482vbE24pjNijx1jsoANvlymxoC8AsQAvD\_BwE</span>](https://www.bigapplebuddy.com/product/8/nest-secure-alarm-system-white/14374?child_sku=6080402&utm-medium=pla&utm-co=SE&gclid=CjwKCAiA_f3uBRAmEiwAzPuaM1tlnx5Rmbx6hAUAP7Z_zMQzLrarA482vbE24pjNijx1jsoANvlymxoC8AsQAvD_BwE) since Google Nest was used on Floor 1 and 2 but could not find it in Sweden yet. Alternatively one can try with the Google outdoor camera again and remaining devices from other suppliers.

I have chosen the Yale security system since the security devices are interconnected and can be connected to the Unifi in wall unit on Floor 4 for WiFi connectivity between all devices.

Specification Source:

[<span class="underline">https://www.yale.co.uk/en/yale/couk/products/smart-living/smart-home-alarms/smart-home-alarm-kit/</span>](https://www.yale.co.uk/en/yale/couk/products/smart-living/smart-home-alarms/smart-home-alarm-kit/)

**<span class="underline">My reflections during this assignment product research</span>**

Before looking into the market, I assumed of a house with all smart devices from one supplier so that with one application on my smartphone, I could control all the devices. But once I started looking into the market, I realised there were a limited number of smart products which worked with one single application.

Additionally the gateways had three problems -

1\. Some gateways were not compatible with many smart device brand providers. This meant I could not use a Google Nest camera with a Hornbach Smart Home Gateway, for example.

2\. There connectivity was limited for example 100 meters. This connectivity was not scalable for a multi storeyed building.

3\. Some gateways had only wireless connectivity. This means if I had to use ethernet or power a smart device via gateway, that was not possible.

The solution to gateway problem 2 & 3 was provided by Ubiquiti Unifi but the problem 1 is still unsolved in our practical home. There is a solution by using a Smart Hub connecting various smart devices that don’t talk to each other. For example, one could use Athom Homey [<span class="underline">https://homey.app/sv-se/</span>](https://homey.app/sv-se/) which is available in the market for around 3400 SEK today.

I have avoided the use of smart hub because of two reasons -

1.  > It might slow down the responsiveness of my smart devices

2.  > Presently, there are not huge amount of smart devices in the design.

But in the future, if we need more devices then hopefully we can install a Homey hub. Expect by that time there will be a wider range of smart products provided by the same supplier.

One more thing - I have not used any Google Home or Amazon Alexa like voice assistants out of personal choice. These devices listen to private conversations and can also be prone to false trigger by accidental use of name Google or Alexa.

GDPR issues have been filed reporting the breach of privacy data by the voice assistants for example this -

[<span class="underline">https://techcrunch.com/2019/08/02/google-ordered-to-halt-human-review-of-voice-ai-recordings-over-privacy-risks/</span>](https://techcrunch.com/2019/08/02/google-ordered-to-halt-human-review-of-voice-ai-recordings-over-privacy-risks/)

Overall, the house has networking for device scalability in future. Also, the networking hub being modular provides network scalability, if needed.


