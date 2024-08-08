# MicroPython_weatherstation_clock_RPiW_i2c_LCD1602
based on project from https://how2electronics.com/raspberry-pi-pico-w-iot-weather-station-openweathermap/

used Thonny IDE as at https://randomnerdtutorials.com/getting-started-thonny-micropython-python-ide-esp32-esp8266/

installed firmware as at https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/3

other useful info: https://randomnerdtutorials.com/projects-raspberry-pi-pico/

![schematic](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEil5gJXyv9T17ok5rb63Mfo6C1IBHG_IsvHhO8xzbZy_chHft5jRu0zATV-FepKYvg5JqyE9GqgMcJTwAQfToS2WuQ_8T8dbeLVi_MMS0GfuyPGjYdEODjpoZY6wgXEQASJIqIjQDVOPidBwOjn8Z2Mdrp-EtEm13SVdClQd4swbeTyMZ2nplezY8j658pe/s320/Raspberry-Pi-Pico-W-I2C-LCD.jpg)

1st article: http://nicuflorica.blogspot.com/2024/08/ceas-cu-date-meteo-rpi-pico-w-si-afisaj.html

for v1 version or v2 version, you need change in main.py:
- line no.7: your Wi-Fi network name and password
- line no.8: your APIkey in openweathemap.org 
- line 106: Craiova with your city

Already I changed in main.py file line no.112 to solve local time issue (+3 in my case):  hours=(time.localtime()[3]+int(weather_data["timezone"] / 3600))%24

For version no.2 I used librar from https://github.com/Guitarman9119/Raspberry-Pi-Pico- !
