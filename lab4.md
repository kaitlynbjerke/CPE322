# Lab 4 - Django and Flask
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** In this lab, we were tasked with utilizing Django, which is a framework that supports the development of web aplications. Additionally, we utilized Flask, another python-based web framework.

**Pre-Lab Steps:** In order to execute some steps in this lab, I had to create a virtual environment. In order to do this, I executed the following code:
``` python
python -m venv myenv
source myenv/bin/activate
```
Additionally, I had to install some additional packages, including `django`, `djangorestframework`, `setuptools`, `django-filter`, `markdown`, `requests`, and `flask`

Weather Station
---
This part of the lab utilized Django in order to create a web application that shows the current temperature. In order to accomplish this task, I had to edit the necessary files, including settings.py and index.html, using the `nano` function. Additionally, I copied python files into the appropriate directory, created an API key for the map on the website, created a django superuser, and ran the web app at [127.0.0.1:8000](http://127.0.0.1:8000)
![weather](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-04-01%20095552.png)

mycpu
---
This is a Django REST project, which is an extension of Django that utilizes APIs to simplify projects. For this project, I underwent many of the same steps as for the weather station project. For this, I also needed to download `psutil`, which accesses CPU information. Additionally, I simultaneously ran the `controller.py` program in order to collect data regarding cpu usage and memory on my device. The resulting website showed that cpu information, updating periodically.
![cpu](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-04-01%20095922.png)

hello_world
---
This project utillizes Flask, which is similar to Django, but used for simpler applications. For this project, I ran `python3 hello_world.py`, and then went to [127.0.0.1:5000](http://127.0.0.1:5000/). The resulting output was a website that just printed "hello, world."
![flask](https://github.com/kaitlynbjerke/Images/blob/main/hello%20world.png)
