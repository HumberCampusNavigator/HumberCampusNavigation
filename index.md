# Week-10 - Nov-06
 This week I got the PCB that I designed actually built. It was my very first experience like this and was really amazing to have a PCB designed by me itself. After getting the PCB, I soldered my sensor with the PCB, but not directly. I used an header which I soldered on top part of the PCB directly and then I inserted my sensor to the header. Again I soldered another header to the other part of the PCB and connected the header to the pins of Raspberry pi.
 
 ![blog2](https://user-images.githubusercontent.com/43181567/48283711-4ceb0f00-e42b-11e8-811c-390f9df38c10.jpeg)
 ![blog1](https://user-images.githubusercontent.com/43181567/48283710-4ceb0f00-e42b-11e8-9058-3f58cf3142cd.jpeg)

 Since there need a connection between the third and eighth pin of the sensor, I needed to connect it on the PCB with a small wire. Actually it is to make the SDO_G pin low which will give the readings on 6a insted of 6b. Eventhough I made this connection on the PCB, since there was no actual 'VIA' connection, I needed to do this, otherwise need to redesign and make a brand new one. This was a good experience for me which I think will be helpfull in solving real world problems too.
 ![blog3](https://user-images.githubusercontent.com/43181567/48283712-4d83a580-e42b-11e8-80e1-8e7a8995e9b7.jpeg)
# Week-9 - Oct-30
 This week I finished the PCB design and send it to Prototype Lab of Humber College for its making. One PCB will be attched on to the Raspberry pi and my sensor will be attached to the PCB. The image below is the PCB designed. In the image below, the Orange wires shows wiring under the PCB, that will not be visible after attaching to the raspberry pi. The Yellow lines are wiring on the top portion of the PCB. The sensor will come on top of the PCB. You could also see the round images with black core, which connects orange lines and yellow lines, which are called 'VIA', are used to connect the wiring from down side of PCB to the top side of PCB.
 
  This week, when I reviewed the progress of the project, it is a good feeling that the project is progressing as expected. All milestones are being covered on time. Budget of the project is also as expected. No extra expenses incurred yet.
  
![pcb design](https://user-images.githubusercontent.com/43181567/47764834-57740e80-dc9d-11e8-9220-53d7898e6b8d.png)

# Week-8 - Oct-23
 This week I finished the breadboarding of the sensor, wiring it to the Raspberry pi and connecting the raspberry pi to a screen using HDMI/VGA cables & also through VCN. 
 
 ![breadboard](https://user-images.githubusercontent.com/43181567/47765308-c0f51c80-dc9f-11e8-91ae-60b8e82cea00.png)
 
 After connecting the sensor with the raspberry pi, I was successfull in getting the readings from the sensor. But the reading that was supposed to be at the location 6A was coming at 6B. This error was rectified by making the terminal SDO_G on the sensor low, ie, by connecting terminal SDO_G to Ground. I also assigned static ip for the raspberry pi because, each time when I connect through VCN, it is easy in future to set up the connection, no need to find the ip address assigned.
 
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

I purchased the sensor from robotshop.com

![robotshopbill](https://user-images.githubusercontent.com/43181567/47049705-14c61880-d16c-11e8-8cce-6dd2eb901e12.png)

# Week-4 - Sept-25

Here is the Budget for my Project

![budget](https://user-images.githubusercontent.com/43181567/47050517-a9ca1100-d16e-11e8-802e-e4492f145e6d.png)

# Week-3 - Sept-18

Here is the Project Schedule/Gantt Chart for the project

![gantt chart](https://user-images.githubusercontent.com/43181567/47050518-a9ca1100-d16e-11e8-99f8-abb6f7a2d0af.PNG)

# Week-2 - Sept-11

The Proposal of the project is given below

![proposal](https://user-images.githubusercontent.com/43181567/47050519-a9ca1100-d16e-11e8-94a1-91569708e7a5.png)

# Week-1 - Sept-04

The idea of the project was discussed with the professor and group members were finalised. 
The name of the project was decided as 
# HUMBER CAMPUS NAVIGATOR
