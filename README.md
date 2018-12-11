### Build Instructions for using 'LSM9DS0 9-axis Accelerometer, Magnetometer, Gyroscope & Temperature Sensor' on a Raspberry Pi

In this Project, the aim is to give step by step instructions to build an hardware unit that measures the values coming from the LSM9DS0 <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a>. I will be discussing the components needed to build the unit, how much it might cost, various tools that we might need while building up a unit, how to use that tools, and the key factors that should be taken care of . We will start with the system diagram,

## System Diagram of the Hardware
![system diagram paint](https://user-images.githubusercontent.com/43181567/49611645-29ef4480-f970-11e8-9987-dfd604e5d199.png)
```
  The above diagram explaines how LSM9DS0 sensor can be used to build an hardware unit  which can be used to record the readings coming 
from the sensor using a Raspberry Pi. The sensor should be solderedd to an header pin and the header pin's other end should be soldered
to  a  PCB. The PCB  in trun is soldered to  another header pin  on the opposite side  where the sensor is attached.  The second header 
pin is then attached to  the I/O pins of the Raspberry Pi.  This whole unit is enclosed in an acrylic case for safety. The Raspberry Pi
needs  power  and should be connected to a Virtual  connection (wired/wireless) for operating  Raspberry Pi  remotely  by  which we can 
read the values coming from the sensor.
```
## The Components needed to make the Unit and its Cost

  If you are a student of a college or University, you most probably will have a Parts Kit which can be used here. You don't need to buy all those things, that you already have, which reduces the budget significantly. I am including all the components needed for the project, excluding items that are expected to be with students.
  
  All prices are in Canadian Dollars and include Taxes where ever applicable.
  
![budget for readme](https://user-images.githubusercontent.com/43181567/49680537-78314000-fa63-11e8-9830-149a1c6fbae9.PNG)

  You will also need a Laptop or a Desktop to set up the Virtual Connection and operate the Raspberry Pi remotely. Also for printing a 'PCB' and an enclosure(Hard case that holds the entire unit) you might need the help of a Prototype Lab, the cost of which I havent included here. You can get the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>, breadboard & Jumper Wires from Amazon.ca and the LSM9DS0 <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> from robotshop.com. There are several online portals that sell these items, you can shop around and find the cheapest one. This data is just for an overall idea about the budget.
  
#### You can see the pictures of the major components below,
### The Sensor
![sensor lsm9dso](https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg)
### The Raspberry Pi
![raspberrypi](https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png)

## Step by Step Instructions for building the Unit.

### Step-1
  The first step is to set up the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>. Raspbian is the Operating System for the Raspberry Pi. We will flash Raspbian OS on a 16 GB SD card and insert it into the Raspberry Pi. Raspbian OS is free and can be downloaded online. The flashing instructions can be found <a href="https://www.raspberrypi.org/documentation/installation/installing-images/">here</a> and if the flashing was successfull, when giving power to Raspberry Pi and connecting it to a display, will detect and boot the Raspbian OS automatically. For the first time, we need a mouse and a keyboard connected to Raspberry Pi to set up the Virtual Connection (using VNC Viewer) for Raspberry Pi, by giving input and Wi-Fi credentials. For setting up a virtual connection for remote operation of the unit we need to install VNC Viewer on Raspberry Pi and on the Desktop/Laptop which we use to remotely control Raspberry Pi. The details of how to install and setup VNC viewer can be found by clicking <a href="https://www.raspberrypi.org/documentation/remote-access/vnc/">here</a>.


### Step-2
  Second step is to check whether the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> is in working condition. First we should <a href="https://www.youtube.com/watch?v=3230nCz3XQA">solder</a> a <a href="https://www.aimagin.com/pin-header-long-single-row.html">9 pin header pin</a> on to the sensor, so that the sensor can be inserted into a breadboard. Before start soldering please read this <a href="https://safety.eng.cam.ac.uk/safe-working/copy_of_soldering-safety">document</a> for your own safety. We need to get the raw readings from the sensor on the specific I2C address of the Raspberry Pi. For that we need to find out the wiring diagram of the Sensor output to the specific pins on the Raspberry Pi. We are expected to get readings in two addresses after the wiring of sensor and <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> as shown below. The addresses where we get readings are '6a' and '1d' of the Raspberry Pi. To get the readings after connection open a terminal on the Raspberry Pi and give the command 'i2cdetect  -y 1'.
  
  ![wiring for readme](https://user-images.githubusercontent.com/43181567/49758374-c412fd80-fc8c-11e8-95a8-93683e93447f.PNG)
  
#### Sensor wired with Raspberry pi
  ![wired](https://user-images.githubusercontent.com/43181567/47402430-8590a600-d713-11e8-9d7d-0f8aa296ec67.png) 

#### Readings as Expected
  ![second1](https://user-images.githubusercontent.com/43181567/47402636-9988d780-d714-11e8-8801-65fb05d1cb4f.PNG)
  
### Step-3
  Once we make sure that our <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> and <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> is working, we can start the designing of PCB  and <a href="https://www.youtube.com/watch?v=3230nCz3XQA">soldering</a>(Please read <a href="https://safety.eng.cam.ac.uk/safe-working/copy_of_soldering-safety">safety measures</a>) of components. Designing a PCB can be done using fritzing software. Click <a href="http://fritzing.org/learning/">here</a> to get insructions on how to use fritzing. This is the image of the fritzing file generated specifically for this sensor and Raspberry Pi. You can download the below fritzing file from this <a href="https://github.com/HumberCampusNavigator/HumberCampusNavigation/blob/master/Fritzing.zip">link in zip format</a>.
  
  ![pcb design](https://user-images.githubusercontent.com/43181567/47764834-57740e80-dc9d-11e8-9220-53d7898e6b8d.png)

  Once you are done with the PCB design, you should take this file to a lab where PCB's can be printed out and get it printed out. Once you get the PCB board printed out, you should solder two header pins onto the PCB. One stack header pin of <a href="https://canada.newark.com/adafruit/2223/40-pin-pi-gpio-stacking-header/dp/31AC4582?gclid=EAIaIQobChMIo4ejjLOW3wIVQbjACh2MeQRJEAYYBCABEgISn_D_BwE&CAGPSPN=pla&CAWELAID=120185770002227709&CAAGID=23354969332&CMP=KNC-GCA-GEN-SHOPPING&CATCI=pla-294680686006">40 pins (two 20 pins in parallel)</a> to be soldered to PCB so that the PCB can be securely attached to the Raspberry Pi. Another single line 10 pin stack header pin to be soldered on the other side of the PCB where the sensor can be attached to the PCB securely. The following images will make the idea clear.
  ![blog3](https://user-images.githubusercontent.com/43181567/48283712-4d83a580-e42b-11e8-80e1-8e7a8995e9b7.jpeg)  
  ![blog1](https://user-images.githubusercontent.com/43181567/48283710-4ceb0f00-e42b-11e8-9058-3f58cf3142cd.jpeg)
  ![blog2](https://user-images.githubusercontent.com/43181567/48283711-4ceb0f00-e42b-11e8-811c-390f9df38c10.jpeg)

### Step-4
   After attaching the sensor on to the PCB and then the PCB on to the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> will take out all wirings and the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> is now connected to the Raspberry Pi with the help of PCB and header pins which are all soldered each other appropriately to make a single unit. Now in this step we need to install a python software specific for our sensor in the Raspberry Pi so that the software will process the raw signals coming from the sensor into human readable values. The measured values of Accelerometer, Gyroscope, Magnetometer and Temperature are expected. The python software for this is readily available from this <a href="http://ozzmaker.com/python-code-for-berryimu-accelerometer-gyroscope-magnetometer-pressure-sensor/">link</a>. All the necessary instructions for installing the software is given in this link. This software expects an output in the address '6b'. Since we are expecting the reading in '6a' address, a minor change need to be done before running the software. I changed the address from '6b' to '6a' in the file 'adafruit_lsm9ds0.py' and the software detected the readings and outputed the values as shown below.We need to do this because output of the sensor has been changed from '6b' to '6a' by making the SDO_G terminal of the sensor low. If SDO_G terminal of the sensor is not made low, we don't need to make this change to this software. The software file I changed is located at "usr/local/lib/python3.5/dist-packages/adafruit_lsm9ds0.py" on my <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>. The readings will come when running 'main.py' inside the software.
   ![whatsapp image 2018-11-19 at 1 35 15 pm 1](https://user-images.githubusercontent.com/43181567/48727577-a956e700-ec00-11e8-939c-4a5b10ac2c11.jpeg)
   
### Step-5
   Now the next step is the enclosure. It simply means to protect the working piece of your hardware get enclosed in a secure case to protect the unit from external damages. So to do that, you need to design an acrylic case for the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> which encloses the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> attched to the PCB. To design the case, you can use <a href="https://www.coreldraw.com/en/">CorelDraw</a> software. This is the link to download the <a href="https://www.coreldraw.com/en/">CorelDraw</a> codes for the below design.
https://github.com/HumberCampusNavigator/HumberCampusNavigation/blob/HumberCampusNavigator-CoralDraw/Pi2CaseX6.cdr
#### The design of the case using <a href="https://www.coreldraw.com/en/">CorelDraw</a> software
![whatsapp image 2018-11-20 at 5 41 26 pm 1](https://user-images.githubusercontent.com/43181567/48807494-ac7ad180-eceb-11e8-9a7a-947465b7f728.jpeg)
#### Images of the Hardware Unit built 
![whatsapp image 2018-11-20 at 5 41 24 pm](https://user-images.githubusercontent.com/43181567/48807491-abe23b00-eceb-11e8-8c7f-59baf00bae6f.jpeg)
![whatsapp image 2018-11-20 at 5 41 25 pm 1](https://user-images.githubusercontent.com/43181567/48807492-abe23b00-eceb-11e8-9f5a-143c627abe76.jpeg)
![whatsapp image 2018-11-20 at 5 41 25 pm](https://user-images.githubusercontent.com/43181567/48807493-ac7ad180-eceb-11e8-80ae-30af35c69a8d.jpeg)
![whatsapp image 2018-11-20 at 5 41 26 pm](https://user-images.githubusercontent.com/43181567/48807495-ac7ad180-eceb-11e8-970e-85bc3c8a9aef.jpeg)

  

  


  





    

