4G Phone with ESP32-S3-SIM7670G

Description: A custom-built 4G LTE smartphone powered by the ESP32-S3. This device is designed to function as a regular phone.

Why I made it: Regular Smartphones are a distraction from our daily life and routine, we tend to keep watching it for the dopamine aspect, additionally, the software and OS not being open source leaves us vulnerable to trackers, etc. With an open source OS and code, we have complete freedom and privacy, and are aware of where our data is being used.

Features:

4G LTE connectivity (SIM7670G)

2.8" Capacitive Touch Display

Camera and audio

Custom 3D printed chassis

Architecture: Two ESP32-S3s are used(Dual MCU architecture). Both are integrated into their respective boards. One on the SIM7670G and one on the 2.8" screen. They communicate via Serial(UART). The ESP32-S3 on the display handles graphics and UI, while the ESP32-S3 on the SIM7670G handles the calling logic.

Assembly Instructions:

3D Print: Print the chassis using any material with gyroid infill. Material suggested: ASA or PLA+(I suggest ASA for the better heat tolerance specs, but haven't used it since i use an ELEGOO Neptune 4)

Wiring: Built to be modular, just connect the 18650 battery to both boards and connect the two boards through UART( wire included with screen I chose).

Software: Flash the respective codes in /src(coming soon) to the two ESP32-S3s using the Arduino IDE.

Bill of Materials:

Component Cost(AED) Cost(USD) Link Hosyond 2.8'' Screen 79.29 21.60490463 https://amzn.eu/d/0iEEv7Ig ESP32-S3 SIM7670G 179.79 48.99 https://www.waveshare.com/esp32-s3-sim7670g-4g.htm 32GB Storage SD Card 16 4.359673025 https://amzn.eu/d/0a1YgC0N 3.7V 3200mAH Battery 80.92 22.04904632 https://www.amazon.in/dp/B0F3XHNRPT?psc=1&ref_=cm_sw_r_cp_ud_ct_RA1AZJE9ZNZMSNYY2FQ9_6 Capacitative Stylus 2.00 0.5449591281 https://www.amazon.in/dp/B0FHW2K49G?psc=1&ref_=cm_sw_r_cp_ud_ct_RA1AZJE9ZNZMSNYY2FQ9_8 Delivery & Tax 50.1689 13.67 NA Total 408.17 111.2185831 NA

(If you are trying to replicate this project, you can definitely change the parts as long as they are functional and good enough for the project.) (I have made two variants of this project, one uses a PCB and one doesn't, at first I will be using the version without a PCB. If you find the version with the PCB better, you can definitely use it. Just remember to replace the SIM7670G with this(as it uses EC200U rather than SIM7670G:

https://evelta.com/7semi-esp32-s3-ec200u-4g-lte-cat-1-wifi-bluetooth-gnss-iot-smart-modem/?sku=004-DC-10120&utm_campaign=PMax_7Semi_Brand&utm_source=google&utm_medium=cpc&utm_matchtype=&utm_term=&adgroupid=&gc_id=21448253640&h_ad_id=&gad_source=1&gad_campaignid=21448255362&gbraid=0AAAAADwtsXniiHdx4kQmTVuiIV6Tp6DU1&gclid=CjwKCAjwyuDTBhB-EiwANCQhLGBQXLIfmObVwrfRuaRKQDc5tHNnd7hCKBzqb87wfotB9UMXs5gdgRoCigwQAvD_BwE)

