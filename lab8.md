# Lab 8 - Data Analysis
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** For this lab, we want to investigate how python can be used for data analysis. Specifically, we used our previously generated data from lab 7, and used python functions to generate graphs / plots.

**Prelab tasks:** Before starting this lab, we had to install some libraries. I used pip to install these libraries, and I executed this line of code: `pip install numpy scipy scikit-learn matplotlib pandas tensorflow keras`

Additionally, I downloaded VcXsrv, which permits graphical output on WSL.

![install](https://github.com/kaitlynbjerke/Images/blob/main/installation.png)

A final set-up step was downloading the previously collected cpu data (CPU Usage and Memory Available) as a .csv file, and moving the file into the working directory.

plt_///.py Functions
---
*Note: this part of the lab requires WSL2 rather than WSL, as WSL2 is functional with GUI applications when used in conjunction with X servers*

First, I altered the `plt_final.py` and `plt_cv2.py` functions, allowing them to source data from my cpudata file. Additionally, I changed the "Temperature" information to "Memory Available", as the cpudata file does not include the former. Below, I have attached the editted `plt_cv2.py` script, however similar alterations were made to `plt_final.py`.

![plt_cv2](https://github.com/kaitlynbjerke/Images/blob/main/plt_cv2_script.png)

**plt_final.py:** This function output six different plots, all showing the distribution of data in different ways.

Box Plots:

![memBox](https://github.com/kaitlynbjerke/Images/blob/main/memBoxPlot.png)
![cpuBox](https://github.com/kaitlynbjerke/Images/blob/main/memBoxPlot%20(2).png)

Probability Bar Charts:

![memProb](https://github.com/kaitlynbjerke/Images/blob/main/memProb.png)
![cpuProb](https://github.com/kaitlynbjerke/Images/blob/main/cpuProb.png)

Scatterplot:

![scatter](https://github.com/kaitlynbjerke/Images/blob/main/cpuUsageVsMem.png)

Time-Series Plot:

![line](https://github.com/kaitlynbjerke/Images/blob/main/cpuMemTime.png)

**plt_cv2.py:** This function output one single plot: Memory Available vs. Predicted Value

![predicted](https://github.com/kaitlynbjerke/Images/blob/main/predicted_cv2.png)
