# Komponenter som används

- ESP32 C6 https://www.electrokit.com/utvecklingskort-esp32-c6
- LD2420 (Microvågssensor) https://www.electrokit.com/rorelsesensor-mmwave-24ghz
- BME680/BME688 (Klimatsensor) https://www.amazon.se/gp/product/B0DGPS9KRZ/ref=ox_sc_act_image_1?smid=A2WSSX5YFMIMA4&psc=1
- BH1750 (Ljussensor) https://www.amazon.se/gp/product/B07NLL4SCB/ref=ox_sc_act_title_1?smid=A1X7QLRQH87QA3&th=1

# Kopplingsschema multisensor

## Neutral
ESP32 C6 GND  -->  Microvåg (Svart kabel)\
ESP32 C6 GND  -->  Ljussensor (Svart kabel)\
ESP32 C6 GND  -->  Klimat (Svart kabel)

## Positiv 3,3V
ESP32 C6 3V3  -->  Microvåg (Röd kabel)\
ESP32 C6 3V3  -->  Ljussensor (Röd kabel)\
ESP32 C6 3V3  -->  Klimat (Röd kabel)

## Rörelsesensor
ESP32 C6 GP0  -->  Microvåg (Grå kabel) TX\
ESP32 C6 GP1  -->  Microvåg (Lila kabel) RX

## i2c för ljus och klimat sensor
ESP32 C6 GP2  -->  Ljussensor (Orange kabel) SDA\
ESP32 C6 GP2  -->  Klimat (Orange kabel) SDA\
ESP32 C6 GP3  -->  Ljussensor (Gul kabel) SCL\
ESP32 C6 GP3  -->  Klimat (Gul kabel) SCL

