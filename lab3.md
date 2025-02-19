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
The Julian date is how many days have passed since the start of the Julian period, which marks the alignment of the Indictment, Solar, and Lunas cycles.
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
This outputs the coordinates of an inputted location. However, when I initially tried to run this program, I kept getting a "certificate verification failed" error. After attempting multiple solutions, I decided to edit the code to fix the problem. With help from ChatGPT, I rewrote a part of the source code in order to implement SSL context verification. After that, the code ran successfully.

**coordinates.py output:**
![coordinates](https://github.com/kaitlynbjerke/Images/blob/main/lab3/coordinates.png)
**Original coordinates code:**
![coordinatesOG](https://github.com/kaitlynbjerke/Images/blob/main/lab3/coordinatesOG.png)
**Edited coordinates code:**
![coordinatesNew](https://github.com/kaitlynbjerke/Images/blob/main/lab3/coordinatesNew.png)

python3 address.py "40.74480675, -74.02532861159351"
---
This code outputs an address that corresponds to longitude/latitude coordinates. I faced a similar issue for this code, so, using what I learned from the coordinates code, I altered the address.py code accordingly. After revising the code, the function resulted in the expected output. 

**address.py output:**
![address](https://github.com/kaitlynbjerke/Images/blob/main/lab3/address.png)
**Edited address code:**
![addressNew](https://github.com/kaitlynbjerke/Images/blob/main/lab3/addressNew.png)

python3 cpu.py
---
This original code did not work on my computer. I kept getting an error about needing the "psutil" library. After two hours of unsuccessfully trying to download the library, I decided to alter the original code to not require the psutil library. I input the code into ChatGPT, and went through many iterations until it output a working program. The function output the number of physical cores, the number of logical cores, and the percentage of the cpu being utilized.

**cpu.py output:**
![cpu](https://github.com/kaitlynbjerke/Images/blob/main/lab3/cpu.png)
**Edited cpu code:**
![cpuNew](https://github.com/kaitlynbjerke/Images/blob/main/lab3/cpuNew.png)

python3 battery.py
---
This code shows the current battery information of your machine. Again, this code did not function properly due to the missing psutil library. Thus, I had ChatGPT alter the code to not include the psutil library. The resulting output was different than the expected output. Rather than simply outputting the battery information in the terminal, the new code resulted in the creation of an HTML file than includes a full Battery report.

**battery.py terminal output:** generates the battery report
![battery](https://github.com/kaitlynbjerke/Images/blob/main/lab3/battery.png)
**Battery report:** *Note: the entire battery report spans much longer, but this is just a snippet of it*
![batteryHTML](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-18%20194953.png)
**Edited battery code:**
![batteryNew](https://github.com/kaitlynbjerke/Images/blob/main/lab3/batteryNew.png)

python3 documentstats.py document.txt
---
This function shows information regarding the "document.txt" file, including word count and most used words.
![docstats](https://github.com/kaitlynbjerke/Images/blob/main/lab3/documentstats.png)
