# ohbot for python

<a href="http://whoosh.co.uk/ohbothelp/images/eyes.gif" target="_blank"><img src="http://whoosh.co.uk/ohbothelp/images/eyes.gif" border="0" width = "30%"/></a>


This package is a starting point for people wanting to use Python 3 to control Ohbot. 

More information about Ohbot can be found on [ohbot.co.uk](http://www.ohbot.co.uk)

Dependencies
----------

If you don't have pip3 (the python 3 package manager) installed, open terminal and execute the following:

```
sudo apt-get install python3-pip
```

Ohbot requires the some libraries to be installed. 

To install libraries execute the corresponding terminal commands in your Raspberry Pi terminal:

| Library    | Use         | Terminal command to install  |Link |
| ---------- |-------------| -----------------------------|-----|
| ohbot   | Interface with Ohbot          | ```sudo pip3 install ohbot``` |[ohbot](https://github.com/ohbot/ohbot/) |
| festival    | Generate text to speech  | ```sudo apt-get install festival```  |- |
| espeak (optional)    | Generate text to speech  | ```sudo apt-get install espeak```  |[espeak](http://espeak.sourceforge.net/) |
| pico2wave (optional)    | Generate text to speech  | ```sudo apt-get install libttspico-utils```  |-|
| lxml    | Import settings file          | ```sudo apt-get install python3-lxml``` |[lxml](https://github.com/lxml/lxml) |
| serial    | Communicate with serial port | Included with Ohbot |[pyserial](https://github.com/pyserial/pyserial/) |
| threading    | Run multiple threads     | Included in Python 3  |- |
| os    | Send commands to festival       | Included in Python 3  |- |
| time    | Run timers                    | Included in Python 3  |- |


You only need to install ```ohbot```, ```lxml``` and ```festival```, ```serial``` should be installed automatically during the install of ohbot. 

Additonal voices can be used by installing ```espeak``` and ```pico2wave```

Ohbot is tested with Python 3 running on a Raspberry Pi 3 Model B. 

To upgrade to the latest version of the library run the following in the console:
```sudo pip3 install ohbot --upgrade```



Ohbot library files (these will be installed with the `pip3 install ohbot` command above):

| File    | Use         |
| ---------- |------------|
| ohbot.py   | Ohbot package |
| MotorDefinionsv21.omd    | Motor settings file |

_Note: The text to speech module Festival will generate an audio file, ‘ohbotspeech.wav’ and a text file ‘phonemes.txt’ inside your working folder._

---

Hardware
-----

Required:


* Raspberry Pi
* Ohbot
* USB Y Cable
* A 5 volt 1 amp USB power supply (for Ohbot)
* Speakers/headphones with 3.5mm headphone jack


Setup:



Plug the middle of USB Y cable into Raspberry Pi and the other large USB plug into the power adaptor. Then plug the mini USB into Ohbot. Finally plug your speakers into your Raspberry Pi. 

---

Writing Programs
--------

1. Open Python 3 (IDLE)
2. Click File → New File
3. Save your file as a python script (.py) in a new folder called Ohbot somewhere on your Pi.

Import
-------

Make sure you import ohbot at the start of your program. 
```python
from ohbot import ohbot
```

---