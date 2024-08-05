# MicroPython_weatherstation_clock_RPiW_i2c_LCD1602
based on project from https://how2electronics.com/raspberry-pi-pico-w-iot-weather-station-openweathermap/

used Thonny IDE as at https://randomnerdtutorials.com/getting-started-thonny-micropython-python-ide-esp32-esp8266/

installed firmware as at https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/3

for v1 version, you need change in main.py:
- line no.7: your Wi-Fi network name and password
- line no.8: your APIkey in openweathemap.orp 
- line 106: Craiova with your city

_Already I changed in main.py file line no.112 to solve local time issue (+3 in my case):  hours=(time.localtime()[3]+int(weather_data["timezone"] / 3600))%24 _
