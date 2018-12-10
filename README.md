### Build Instructions for using 'LSM9DS0 9-axis Accelerometer, Magnetometer, Gyroscope & Temperature Sensor' on a Raspberry Pi

In this Project, the aim is to give step by step instructions to build an hardware unit that measures the values coming from the LSM9DS0 sensor. I will be discussing the components needed to build the unit, how much it might cost, various tools that we might need while building up a unit, how to use that tools, and the key factors that should be taken care of . We will start with the system diagram,

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

  If you are a student of a college or University, you most probably will have a Parts Kit which can be used here. You don't need to buy all those things, that you already have which reduces the budget significantly. I am including all the components needed for the project excluding items that are expected to be with students.
  
  All prices are in Canadian Dollars and include Taxes where ever applicable.
  
![budget for readme](https://user-images.githubusercontent.com/43181567/49680537-78314000-fa63-11e8-9830-149a1c6fbae9.PNG)

  You can also expect some shipping charges for the components if you are ordering online. You will also need a Laptop or a Desktop to set up the Virtual Connection and operate the Raspberry Pi. Also for printing a 'PCB' and an enclosure(Hard case that holds the entire unit) you might need the help of a Prototype Lab, the cost of which I havent included here. You can get the Raspberry Pi, breadboad & Jumper Wires from Amazon.ca and the LSM9DS0 sensor from robotshop.com. There are several online portals that sell these items, you can shop around and find the cheapest one. This data is just for an overall idea about the budget.
  
#### You can see the pictures of the major components below,
### The Sensor
![sensor lsm9dso](https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg)
### The Raspberry Pi
![raspberrypi](https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png)

## Step by Step Instructions for building the Unit.

### Step-1
  The first step is to set up the Raspberry Pi. Raspbian is the Operating System for the Raspberry Pi. We will flash Raspbian OS on a 16 GB SD card and insert it into the Raspberry Pi. Raspbian OS is free and can be downloaded online. The flashing instructions can be found <a href="https://www.raspberrypi.org/documentation/installation/installing-images/">here</a> and if the flashing was successfull, when giving power to Raspberry Pi and connecting it to a display, will detect and boot the Raspbian OS automatically. For the first time, we need a mouse and a keyboard connected to Raspberry Pi to set up the Virtual Connection (using VNC Viewer) for Raspberry Pi, by giving input and Wi-Fi credentials. For setting up a virtual connection for remote operation of the unit we need to install VNC Viewer on Raspberry Pi and on the Desktop/Laptop which we use to remotely control Raspberry Pi. The details of how to install and setup VNC viewer can be found by clicking <a href="https://www.raspberrypi.org/documentation/remote-access/vnc/">here</a>.


### Step-2
  Second step is to check whether the sensor is in working condition. First we should <a href="https://www.youtube.com/watch?v=3230nCz3XQA">solder</a> an header pin on to the sensor, so that the sensor can be inserted into a breadboard. Before start soldering please read this <a href="https://safety.eng.cam.ac.uk/safe-working/copy_of_soldering-safety">document</a> for your own safety. We need to get the raw readings from the sensor on the specific I2C address of the Raspberry Pi. For that we need to find out the wiring diagram of the Sensor output to the specific pins on the Raspberry Pi. We are expected to get readings in two addresses after the wiring of sensor and Raspberry Pi as shown below. The addresses where we get readings are '6a' and '1d' of the Raspberry Pi. To get the readings after connection open a terminal on the Raspberry Pi and give the command 'i2cdetect  -y 1'.
  
  ![wiring for readme](https://user-images.githubusercontent.com/43181567/49758374-c412fd80-fc8c-11e8-95a8-93683e93447f.PNG)
  
#### Sensor wired with Raspberry pi
  ![wired](https://user-images.githubusercontent.com/43181567/47402430-8590a600-d713-11e8-9d7d-0f8aa296ec67.png) 

#### Readings as Expected
  ![second1](https://user-images.githubusercontent.com/43181567/47402636-9988d780-d714-11e8-8801-65fb05d1cb4f.PNG)
  
### Step-3
  Once we make sure that our Raspberry Pi and sensor is working, we can start the designing of PCB  and <a href="https://www.youtube.com/watch?v=3230nCz3XQA">soldering</a>(Please read <a href="https://safety.eng.cam.ac.uk/safe-working/copy_of_soldering-safety">safety measures</a>) of components. Designing a PCB can be done using fritzing software. Click <a href="http://fritzing.org/learning/">here</a> to get insructions on how to use fritzing. 




  

  


  





    

