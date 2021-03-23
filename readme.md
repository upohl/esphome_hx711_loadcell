![alt text](https://github.com/upohl/esphome_hx711_loadcell/blob/main/FritzingLoadcellSchematic_bb.png?raw=true)

# Parts 
HX711+LoadCell 20KG e.g. https://de.aliexpress.com/categories/hx711-load-cells.html
ESP01 
ESP01 Programmer

# Wiring
Power Supply 3.3V to ESP01 3.3V + ESP01 EN + HX711 VCC;
Power Supply GND to ESP01 GND + HX711 GND;
HX711 SDK to ESP 2;
HX711 DT to ESP 0;

# Framework
www.esphome.io

# Flash (Only via USB)
esphome config/loadcell.yaml run

# Logs (Over the Air)
esphome config/loadcell.yaml logs 

# Webserver
Enter IP Address of ESP01 as written in the config folder 

# Secrets 
add config\secrets.yaml                                                            
ssid: "YOUR_SSID"
password: "YOUR_PASSWORD"
fallback_password: "FALLBACK_PASSWORD"
static_ip: 192.168.1.300
api_password: "SECRET"
ota_password: "SECRET"
