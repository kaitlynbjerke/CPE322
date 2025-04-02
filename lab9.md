# Lab 9 - YANG
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** For this lab, we were tasked with utilizing PlantUML to create UML diagrams in the png format.

**Prelab Tasks:** The required installations for this lab included pyang and plantuml, which I installed with the following line of code: 
`pip install pyang plantuml`

Setting Up
---
- First, I had to copy over a program from lesson 9: `cp ~/iot/lesson9/instrusiondetection.yang`
- I am working in the "demo" directory, so I had to move there: `cd demo`
- Utilizing pyang, I transformed instrusiondetection.yang to yin and uml files:
```
pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
```
- Finally, using python, I ran `python3 -m plantuml -o /C/Users/bjerk/Downloads intrusiondetection.uml` to generate the png of the UML diagram in my Downloads directory

Result
---
I could not view the png file in my file manager, so I had to figure out another way to access it. My solution was to install eog, meaning [Eye of Gnome](https://en.wikipedia.org/wiki/Eye_of_GNOME), which is an image viewer for desktop environments. I ran `eog /home/bjerk/Downloads/intrusiondetection.png`, which opened the following png:
![uml](https://github.com/kaitlynbjerke/Images/blob/main/uml.png)
