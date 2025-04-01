# Lab 5 - Paho-MQTT
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** This lab utilizes Paho-MQTT, which is a type of protocol that allows publishing/subscribing between modules

**Prelab Tasks:** Before starting this lab, I had to install paho-mqtt and update the respository using `git pull`. These steps are shown below:
1. Paho Installation
![paho](https://github.com/kaitlynbjerke/Images/blob/main/paho.png)
2. git pull
![pull](https://github.com/kaitlynbjerke/Images/blob/main/git%20pull.png)

pubcpu and subcpu
---
These functions utilize Paho MQTT in order to send / receive messages. `pubcpu` publishes, or sends, information regarding the CPU to the subscriber. `subcpu` is the subscriber, and receives this information. The functions were run in different terminals simultaneously, so the timestamped information sent by the publisher immediately showed up in the subscriber terminal.
1. Publisher
![pubcpu](https://github.com/kaitlynbjerke/Images/blob/main/pubcpu.png)
2. Subscriber
![subcpu](https://github.com/kaitlynbjerke/Images/blob/main/subcpu.png)
