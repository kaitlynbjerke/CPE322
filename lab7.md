# Lab 7 - ThingSpeak and Google Sheets 
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** For this lab, we were tasked with using ThingSpeak and Google sheets as methods of representing our data.

**Required Installations:** For this lab, we had to install `gspread` and `oauth2client`, which were useful in the second half of our lab.

ThingSpeak
---
1. Create a project in ThingSpeak
![cpu](https://github.com/kaitlynbjerke/Images/blob/main/thingspeakProject.png)
2. Copy over necessary python files
```
cp ~/iot/lesson7/thingspeak_cpu_loop.py .
cp ~/iot/lesson7/thingspeak_feed.py .
```
3. Edit `thingspeak_feed.py` to include your **Write API Key**
4. Run `python3 thingspeak_feed.py`, and let it run to collect data
5. Check graphs in ThingSpeak to observe data collected
![cpu_loop](https://github.com/kaitlynbjerke/Images/blob/main/cpu_pc.png)
![mem_avail](https://github.com/kaitlynbjerke/Images/blob/main/mem_avail.png)

*Note: this computer was off during some of the data collection, hence the straight line*

Google Sheets
---
1. Copy necessary python files to current working directory
```
cp ~/iot/lesson3/system_info.py .
cp ~/iot/lesson7/cpu_spreadsheet.py .
```
2. Log into Google Cloud, create JSON key and corresponding email adress in order to connect the python code to the Google Sheets
3. Add .json file into same directory as cpu_spreadsheet
`mv /mnt/c/Users/bjerk/Downloads/cpudata-xxxxx.json .`
4. Create a sheet in Google Sheets, delete rows 2-1000, add column titles: "Date/Time", "CPU Usage", and "Memory Available"
5. Share sheet with email address associated with .json key
![share](https://github.com/kaitlynbjerke/Images/blob/main/share.png)
6. Use `nano` to edit cpu_spreadsheet.py in order to add the JSON key, run program `python cpu_spreadsheet.py`
![spreadsheet.py](https://github.com/kaitlynbjerke/Images/blob/main/spreadsheet.py.png)
7. View resultant output in spreadsheet
![spreadsheet](https://github.com/kaitlynbjerke/Images/blob/main/googleSheets.png)
