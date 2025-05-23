# Lab 3 - Python
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** For this lab, we were tasked with utilizing Python packages via **bash** in order to test different functions.

**Prelab Tasks:** Before executing this lab, I had to install pip along with some Python packages (astral, jdcal, geopy). **Pip** is the package installer for Python.

cd ~/iot
---
This command changes the directory to the iot github.
![cd_iot](https://github.com/kaitlynbjerke/Images/blob/main/lab3/cd_iot%20(2).png)

cd *3
---
This changes the directory to the third file in the current directory, which is the lesson 3 file.
![cd3](https://github.com/kaitlynbjerke/Images/blob/main/lab3/cd3.png)

python3 julian.py
---
The Julian date is how many days have passed since the start of the Julian period, which marks the alignment of the Indictment, Solar, and Lunar cycles.
![julian](https://github.com/kaitlynbjerke/Images/blob/main/lab3/julian.png)

python3 date_example.py
---
The function marks the date, day of the week, time since the first day of class, and time until the last day of classes.
![date](https://github.com/kaitlynbjerke/Images/blob/main/lab3/date.png)

python3 datetime_example.py
---
This outputs the day, date, and current time.
![datetime](https://github.com/kaitlynbjerke/Images/blob/main/lab3/datetime.png)

python3 time_example.py
---
This function outputs the time in increments of 10 seconds.
![time](https://github.com/kaitlynbjerke/Images/blob/main/lab3/time.png)

python3 sun.py "New York"
---
When I initially tried to run this function, it outputed an error message that I was missing the **Pytz** library, which helps manage timezone calculations. Thus, I had to download the Pytz library, which then allowed me to run sun.py without any errors. This function shows the time of dawn, sunrise, noon, sunset, and dusk at your respective location.

**Initial error message:**
![sun_error](https://github.com/kaitlynbjerke/Images/blob/main/lab3/sun_error.png)
**Pytz installation:**
![pytz](https://github.com/kaitlynbjerke/Images/blob/main/lab3/pytz.png)
**Sun.py execution:**
![sun](https://github.com/kaitlynbjerke/Images/blob/main/lab3/sun.png)

python3 moon.py
---
This function outputs the phases of the moon for the next month. 27 indicates a new moon while 14 indicates a full moon.
![moon](https://github.com/kaitlynbjerke/Images/blob/main/lab3/moon.png)

python3 coordinates.py "Samuel C. Williams Library"
---
This outputs the coordinates of an inputted location in terms of town, county, state, zip code, country, and longitude/latitude.
![coordinates](https://github.com/kaitlynbjerke/Images/blob/main/coordinates.py.png)

python3 address.py "40.74480675, -74.02532861159351"
---
This code outputs an address that corresponds to longitude/latitude coordinates. In this case, we input the coordinates of the Samuel C Williams Library.

![address](https://github.com/kaitlynbjerke/Images/blob/main/address.py.png)

python3 cpu.py
---
This function outputs the number of physical cores, the number of logical cores, and the percentage of the cpu being utilized.
![cpu](https://github.com/kaitlynbjerke/Images/blob/main/cpu.py.png)

python3 battery.py
---
This code shows the current battery information of your machine, including pecerntage remaining and time left.
![battery](https://github.com/kaitlynbjerke/Images/blob/main/battery.py.png)

python3 documentstats.py document.txt
---
This function shows information regarding the "document.txt" file (The Declaration of Independence), including word count and most used words.
![docstats](https://github.com/kaitlynbjerke/Images/blob/main/lab3/documentstats.png)
