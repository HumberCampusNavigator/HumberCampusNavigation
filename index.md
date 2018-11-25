# HUMBER CAMPUS NAVIGATOR

# Week-12 - Nov-20
 This week I am supposed to do my enclosure. It simply means to protect the working piece of my hardware enclosed in a secure case to protect the unit from external damages. So to do that, I need to design an acrylic case for my <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> which encloses the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> attched to the PCB. To design the case, I used <a href="https://www.coreldraw.com/en/">CorelDraw</a> software provided by the college. Staff of the prototype lab helped to understand the software and were great support. The case design was a good challenge and I now know to design something for 2D printing using the <a href="https://www.coreldraw.com/en/">CorelDraw</a> software. It was a good experience and it was not difficult as expected. I got my case printed on the acrylic material and, I now just need to put the whole unit into the case and lock it. It was an easy job. The board of the Raspberry Pi was screwed to the base of the case to make the unit immovable and intact with the case. The screws were provided by the prototype lab of the college. Now my hardware piece with the case looks beautiful as are in the pictures below.  
 # Images of the Hardware Unit built 
![whatsapp image 2018-11-20 at 5 41 24 pm](https://user-images.githubusercontent.com/43181567/48807491-abe23b00-eceb-11e8-8c7f-59baf00bae6f.jpeg)
![whatsapp image 2018-11-20 at 5 41 25 pm 1](https://user-images.githubusercontent.com/43181567/48807492-abe23b00-eceb-11e8-9f5a-143c627abe76.jpeg)
![whatsapp image 2018-11-20 at 5 41 25 pm](https://user-images.githubusercontent.com/43181567/48807493-ac7ad180-eceb-11e8-80ae-30af35c69a8d.jpeg)
![whatsapp image 2018-11-20 at 5 41 26 pm](https://user-images.githubusercontent.com/43181567/48807495-ac7ad180-eceb-11e8-970e-85bc3c8a9aef.jpeg)
 # Follow this link to download the <a href="https://www.coreldraw.com/en/">CorelDraw</a> codes for the below design.
https://github.com/HumberCampusNavigator/HumberCampusNavigation/blob/HumberCampusNavigator-CoralDraw/Pi2CaseX6.cdr
 # The design of the case using <a href="https://www.coreldraw.com/en/">CorelDraw</a> software
![whatsapp image 2018-11-20 at 5 41 26 pm 1](https://user-images.githubusercontent.com/43181567/48807494-ac7ad180-eceb-11e8-9a7a-947465b7f728.jpeg)
# Week-11 - Nov-19
 Hurray, I could finally get the real values out of the readings from my <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> successfully using a <a href="http://ozzmaker.com/python-code-for-berryimu-accelerometer-gyroscope-magnetometer-pressure-sensor/">software</a>. The readings were got using 'main.py' inside the software. I changed the address from 6B to 6A in the file 'adafruit_lsm9ds0.py' and the software detected the readings and outputed the values as shown below. I needed to do this because in Week-8 of my project, I changed the output of the sensor from 6B to 6A by making the SDO_G terminal low. The software file I changed is located at "usr/local/lib/python3.5/dist-packages/adafruit_lsm9ds0.py" on my <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>. But it took really long time to figure out what was the error. I am back on my <a href="https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG">schedule</a> now. The link of the place from where I downloaded my software is http://ozzmaker.com/python-code-for-berryimu-accelerometer-gyroscope-magnetometer-pressure-sensor/ . Next week, that is tomorrow I need to finish my enclosure.
 ![whatsapp image 2018-11-19 at 1 35 15 pm 1](https://user-images.githubusercontent.com/43181567/48727577-a956e700-ec00-11e8-939c-4a5b10ac2c11.jpeg)  
# Week-11 - Nov-13
 As number 13 is considered unlucky, this Nov-13th turned out to be unlucky for me. This week was the power up of the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> due, unfortunately, I could not get the <a href="http://ozzmaker.com/python-code-for-berryimu-accelerometer-gyroscope-magnetometer-pressure-sensor/">software</a> correctly installed on the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> to process the readings from the sensor. Since the specific software could not be installed, I could not complete this week's due. So my project is getting late now. I hope to fix the error in the software and get it working, so that I could be back on <a href="https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG">track</a>. The error is displayed below.
 ![whatsapp image 2018-11-19 at 1 35 14 pm](https://user-images.githubusercontent.com/43181567/48727576-a956e700-ec00-11e8-901d-3673781aa9c6.jpeg)
  I was successfull in getting readings from the sensor, means the raw data. Now I need to try getting the readings using a <a href="http://ozzmaker.com/python-code-for-berryimu-accelerometer-gyroscope-magnetometer-pressure-sensor/">software</a>, and processing the data coming in, and display the values of the readings in decimal values.
  ![whatsapp image 2018-11-19 at 1 35 15 pm](https://user-images.githubusercontent.com/43181567/48727578-a9ef7d80-ec00-11e8-869a-e022aeb3b57c.jpeg)
 # Week-10 - Nov-06
 This week I got the PCB that I <a href="https://user-images.githubusercontent.com/43181567/47764834-57740e80-dc9d-11e8-9220-53d7898e6b8d.png">designed</a> actually built. It was my very first experience like this and was really amazing to have a PCB designed by me itself. After getting the PCB, I soldered my <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> with the PCB, but not directly. I used an header which I soldered on top part of the PCB directly and then I inserted my sensor to the header. Again I soldered another header to the other part of the PCB and connected the header to the pins of <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>.
 
 ![blog2](https://user-images.githubusercontent.com/43181567/48283711-4ceb0f00-e42b-11e8-811c-390f9df38c10.jpeg)
 ![blog1](https://user-images.githubusercontent.com/43181567/48283710-4ceb0f00-e42b-11e8-9058-3f58cf3142cd.jpeg)

 Since there need a connection between the third and eighth pin of the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a>, I needed to connect it on the PCB with a small wire. Actually it is to make the SDO_G pin of the <a href="![sensor lsm9dso](https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg)">sensor</a> low which will give the readings on 6a insted of 6b. Eventhough I made this connection on the PCB, since there was no actual 'VIA' connection, I needed to do this, otherwise need to redesign and make a brand new one. This was a good experience for me which I think will be helpfull in solving real world problems too.
 ![blog3](https://user-images.githubusercontent.com/43181567/48283712-4d83a580-e42b-11e8-80e1-8e7a8995e9b7.jpeg)
# Week-9 - Oct-30
 This week I finished the <a href="https://github.com/HumberCampusNavigator/HumberCampusNavigation/blob/master/Fritzing.fzz">PCB design</a>and send it to Prototype Lab of Humber College for its making. I used the <a href="http://fritzing.org/home/">Fritzing</a> Software to design the PCB. The PCB design can be downloaded by clicking this <a href="https://github.com/HumberCampusNavigator/HumberCampusNavigation/blob/master/Fritzing.fzz">link</a>. One PCB will be attched on to the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> and my sensor will be attached to the PCB. The image below is the PCB designed. In the image below, the Orange wires shows wiring under the PCB, that will not be visible after attaching to the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>. The Yellow lines are wiring on the top portion of the PCB. The <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> will come on top of the PCB. You could also see the round images with black core, which connects orange lines and yellow lines, which are called 'VIA', are used to connect the wiring from down side of PCB to the top side of PCB.
 
  This week, when I reviewed the <a href="https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG">progress</a> of the project, it is a good feeling that the project is progressing as expected. All <a href="https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG">milestones</a> are being covered on time. <a href="https://user-images.githubusercontent.com/43181567/47050517-a9ca1100-d16e-11e8-802e-e4492f145e6d.png">The Budget</a> of the project is also as expected. No extra expenses incurred yet.
  
![pcb design](https://user-images.githubusercontent.com/43181567/47764834-57740e80-dc9d-11e8-9220-53d7898e6b8d.png)

# Week-8 - Oct-23
 This week I finished the breadboarding of the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a>, wiring it to the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a> and connecting the raspberry pi to a screen using HDMI/VGA cables & also through VCN. 
 
 ![breadboard](https://user-images.githubusercontent.com/43181567/47765308-c0f51c80-dc9f-11e8-91ae-60b8e82cea00.png)
 
 After connecting the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> with the <a href="https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png">Raspberry Pi</a>, I was successfull in getting the readings from the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a>. But the reading that was supposed to be at the location 6A was coming at 6B. This error was rectified by making the terminal SDO_G on the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> low, ie, by connecting terminal SDO_G to Ground. I also assigned static ip for the raspberry pi because, each time when I connect through VCN, it is easy in future to set up the connection, no need to find the ip address assigned.
 
 # Readings as Expected
![second1](https://user-images.githubusercontent.com/43181567/47402636-9988d780-d714-11e8-8801-65fb05d1cb4f.PNG)
 # Readings from Sensor with Unexpected Results
![first](https://user-images.githubusercontent.com/43181567/47402425-845f7900-d713-11e8-99f1-5df29760bdd8.png)
 # Sensor wired with Raspberry pi
![wired](https://user-images.githubusercontent.com/43181567/47402430-8590a600-d713-11e8-9d7d-0f8aa296ec67.png) 

# Week-7 - Oct-16

I setup the raspberry pi with the Raspbian Operating System installed on a 16 GB memory card which is  inserted into the memory card slot of the raspberry pi. Further, I recieved all other hardwares ordered during the Week-5 and started to research on the assembly of the breadboard.

# Week-6 - Oct-9

This week I worked on the pseudo codes and UML diagram of the project. There was no class this week as it was our reading week.

# Week-5 - Oct-2

I purchased Raspberry pi from Amazon.ca

![amazonbill](https://user-images.githubusercontent.com/43181567/47049698-11329180-d16c-11e8-81d5-18eb4ec82cfb.png)

I purchased the <a href="https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg">sensor</a> from robotshop.com

![robotshopbill](https://user-images.githubusercontent.com/43181567/47049705-14c61880-d16c-11e8-8cce-6dd2eb901e12.png)

# Week-4 - Sept-25

Here is the Budget for my Project

![budget](https://user-images.githubusercontent.com/43181567/47050517-a9ca1100-d16e-11e8-802e-e4492f145e6d.png)

# Week-3 - Sept-18

Here is the Project Schedule/Gantt Chart for the project

![gantt chart](https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG)

# Week-2 - Sept-11

The Proposal of the project is given below. In this project, the android application will get readings from a sensor and will display it to the users while using the application. The sensor that I am using is <a href="https://www.adafruit.com/product/2021">LSM9DSO</a>. Details about the sensor can be found in https://www.adafruit.com/product/2021 .In this project I am building an hardware unit which reads the data from the sensors and tranfer it to a database so that the application can read from the database. For this I need a Raspberry pi and the sensor as the main components and then some wires and a PCB to power up the unit and to connect the components together.
 # The Sensor
![sensor lsm9dso](https://user-images.githubusercontent.com/43181567/48284781-778a9700-e42e-11e8-9d20-d70dc913a38f.jpg)
 # The Raspberry Pi
![raspberrypi](https://user-images.githubusercontent.com/43181567/48285231-f46a4080-e42f-11e8-9b14-ac0aec60a713.png)
 # The Proposal
![proposal](https://user-images.githubusercontent.com/43181567/47050519-a9ca1100-d16e-11e8-94a1-91569708e7a5.png)

# Week-1 - Sept-04

The idea of the project was discussed with the professor and group members were finalised. 
The name of the project was decided as, 
# HUMBER CAMPUS NAVIGATOR
