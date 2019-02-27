# Project Title

This project is a part for my research project currently working on. We are using LifePo4wered(https://lifepo4wered.com/) a battery solution for raspberry pi,The LiFePO4wered/Pi3™ is a high performance battery power system for the Raspberry Pi.  It can power a Raspberry Pi for 1 to 9 hours from the battery (depending on Raspberry Pi model, attached peripherals and system load) and can be left plugged in continuously. The objective was to run raspberry pi with a bunch of sensors take readings and then send data to the server and go off to sleep. Now the LiFePO4wered/Pi3™ helps to sleep put the raspberry and wake it up the highlight is that we sleep mode consumes 4 Mirco Ohms. For surveillance of the raspberry power consumption and live data feed using pubnub.
Currently in this version we can track the wakeup time average power consumption of raspberry pi during its working cycle and wake up time for its next cycle
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
Required Software’s
```
Setting raspberry pi reference https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/3
Setting the LifePo4wered on raspberry pi use reference https://lifepo4wered.com/files/LiFePO4wered-Pi3-Product-Brief.pdf
Use the following commands for installing Python
sudo apt-get install python3.6

sudo pip install 'pubnub>=4.1.2' or sudo pip3 install 'pubnub>=4.1.2'  
(Depending on the version of pip you are using)

```
### Installing
Once all the Prerequisites are satisfied Follow this step to run on Raspberry Pi
```
Connect Raspberry pi to Network 

Copy the startup.py to in raspberry pi and run the file
sudo python startup.py
run the Reader.html on pc.
```
Once the file starts running it will send out data to the webpage.
## Running the tests

If you want to run the file at startup of the raspberry pi follow the following steps
Sudo nano /etc/profile
Once file is opten go to the file end and paste the below command 
Sudo python locationOf startup.py 
This will run the file each time you start the raspberry pi.
Uncommenting the last two line in the in the python code will shutdown the raspberry pi after the run is complete and then again wake up after 2 mins this process will be continuous and thus you won’t be able to interrupt it. 
If you want to interrupt this then opent he SD card in the computer and edit the lines in the etc/profile file or comment the lines in from the startup.py file from your computer.
### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With
* [LiFePO4wered/Pi3™]( https://lifepo4wered.com/) – API and Hardware
* [Python]( https://www.python.org/) - Python
* [Raspberry Pi]( https://www.raspberrypi.org/) – Raspberry Pi
* [PubNub]( https://www.pubnub.com/) - PubNub
* [Eon API]( https://www.pubnub.com/developers/eon/) – Eon API for graphs

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors
Pinak Kelkar

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
