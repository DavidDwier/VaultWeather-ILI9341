# VaultWeather-ILI9341

This project is a fork from SplinterJawLab/VaultWeather. I changed the Display from an 2-inch ST7789 SPI TFT to ILI9341 display.
I also changed the Timezone to Europe/Berlin/Germany. Everything else stayed the same.
A little weather station inspired by Fallout’s green terminals, now with its own weather artwork. It fetches local weather over WiFi and displays ten different scenes, with animated weather effects including rain, snow, fog and lightning.

The character’s pose matches the weather, from sipping Sun Cola in the sunshine to warming up with tea in the snow. The display also shows the local clock, temperature, feels like, humidity and wind speed. Weather data comes from Open-Meteo, with no API key needed.

This was only my second build like this, so it’s a bit rough around the edges. I mostly figured out where everything would go as I went. The round brass rod forms the exposed frame and carries some of the electrical connections. I ended up rerouting a few connections with copper wires after running into some shorts 😅

## Hardware

- ESP32-C3 SuperMini
- 2-inch ILI9341 SPI TFT (240 × 320, used in landscape)
- 3.7 V LiPo battery
- USB-C LiPo charging module with 5 V boost
- Power switch
- Round brass rod
- Copper wires

## WiFi setup

On first boot, connect to the **VaultWeather** network using the password **vaultweather**. Open **http://192.168.4.1** in your browser and enter your home 2.4 GHz WiFi details. The station saves them and reconnects automatically next time.

Set your city, coordinates and time zone in **config.h** before uploading. All artwork is included in the firmware—no SD card or separate image upload is needed.
