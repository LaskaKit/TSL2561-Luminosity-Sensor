# Modul s čidlem TSL2561 pro měření osvětlení

Moc světla? Zhasni! Málo světla? Rozsviť nebo vytáhni rolety! Jak pozná tvoje domácí automatizace zda má rozsvítit nebo zhasnout? Na to potřebuješ čidlo, třeba náš modul s čidlem TSL2561.

![Osazený modul](https://github.com/LaskaKit/TSL2561-Luminosity-Sensor/blob/main/img/4-10.jpg)

Čidlo TSL2561 je umístěno na našem modulu s už standarní velikostí a rozměry, kde najdeš dva [uŠup konektor](https://blog.laskakit.cz/predstavujeme-univerzalni-konektor-pro-propojeni-modulu-a-cidel-%CE%BCsup/)y a také místo pro zapájení standardního hřebínku s roztečí 2.54mm. Tento modul tak můžeš pohodlně propojit s dalšími moduly.

A jaké moduly to jsou? Třeba čidlo [SCD41 pro měření CO2, teploty a vlhkosti vzduchu](https://www.laskakit.cz/laskakit-scd41-senzor-co2--teploty-a-vlhkosti-vzduchu/), čidla SHT41 [teploty a vlhkosti vzduchu](https://www.laskakit.cz/laskakit-sht40-senzor-teploty-a-vlhkosti-vzduchu/) a [čidla tlaku, teploty a vlhkosti vzduchu BME280](https://www.laskakit.cz/arduino-senzor-tlaku--teploty-a-vlhkosti-bme280/), [RTC Hodiny reálného času](https://www.laskakit.cz/laskakit-ds3231-orig--rtc-hodiny-realneho-casu/) s DS3231 nebo [OLED displej o velikosti 1.3" a rozlišení 128x64px](https://www.laskakit.cz/laskakit-oled-displej-128x64-1-3--i2c/?variantId=11903).

Připojit to můžeš nejen do našich vývojových kitů jako jsou univerzální [Meteo Mini s možností připojení solárního panelu](https://www.laskakit.cz/laskakit-meteo-mini/?variantId=10473), jednoduše programovatelný [ESP32-DEVKit](https://www.laskakit.cz/laskakit-esp32-devkit/?variantId=11481), velmi [úsporný a malý kit ESP32-C3 LPKit](https://www.laskakit.cz/laskkit-esp-12-board/?variantId=10482), [ESPInk s ESP32 a velkým 4.2" ePaper](https://www.laskakit.cz/laskakit-espink-42-esp32-e-paper-pcb-antenna/?variantId=11400) nebo [populárním kitem s ESP32 a 3.5" TFT displejem](https://www.laskakit.cz/laskakit-espd-35-esp32-3-5-tft-ili9488-touch/?variantId=12158). 

Nakonec, není nutné používat pouze naše desky - použít [můžeš téměř kterékoliv Arduino](https://www.laskakit.cz/arduino-2/), jednodeskový počítač [Rock Pi nebo Raspberry Pi](https://www.laskakit.cz/mini-pc/) či jiné vývojové kity s I2C sběrnicí.

![Osazený modul](https://github.com/LaskaKit/TSL2561-Luminosity-Sensor/blob/main/img/3-11.jpg)

Napájecí napětí modulu a tedy i čidla je od 2.7V až do 3.6V. Adresa čidla je 0x29, 0x39 (výchozí) nebo 0x49 - to záleží na pájecím mostu umístěném na zadní straně modulu. Tím můžeš změnit adresu čidla a zapojit tak tři moduly s TSL2561 najednou, každý s nastavenou jinou I2C adresou. U jednoho čidla tedy ponecháš výchozí nastavení, u druhého čidla propájíš středový pad s pájecí mostu s jednou stranou, u třetího pak propájíš středový pad pájecího mostu s druhou stranou.

Další pájecí můstek určuje, zda budou pull-up rezistory připojeny ke sběrnici I2C, nebo ne. Ve výchozím nastavení jsou rezistory připojeny. Pokud je chcete odstranit, stačí přerušit cestu mezi pájecími můstky. 

Podporované knihovny v Arduino IDE jsou</br>
https://github.com/sparkfun/SparkFun_TSL2561_Arduino_Library</br>
https://github.com/adafruit/TSL2561-Arduino-Library</br>

Napsali jsme i vzorové kódy, které najdeš na https://github.com/LaskaKit/TSL2561-Luminosity-Sensor/tree/main/SW
