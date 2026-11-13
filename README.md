VaultWeather

A little weather station inspired by Fallout. It fetches local weather over WiFi and plays different animations throughout the day, like drinking coffee in the morning and yawning at night.

This was only my second build like this, so it’s a bit rough around the edges. I mostly figured out where everything would go as I went. The round brass rod forms the exposed frame and carries some of the electrical connections. I ended up rerouting a few connections with copper wires after running into some shorts 😅

Hardware

ESP32 C3 SuperMini
2 inch ST7789 SPI TFT (240 × 320)
3.7 V LiPo battery
USB C LiPo charging module with 5 V boost
Power switch
Round brass rod
Copper wires

WiFi setup

On first boot, connect to the "VaultWeather" network using the password "vaultweather". Open "http://192.168.4.1" in your browser and enter your WiFi details. The station saves them and reconnects automatically next time.
