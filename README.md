# Sensing Ball 
## FabAcademy Microchallenge 4
[Borka](https://borbalamoravcsik.github.io/mdef-borka/),
[Dídac](https://didac-torrent.github.io/mdef/),
[Pippa](https://philippa-formosa.github.io/mdefweb/)



### Our Sensing Ball will achieve these goals 
**CAPTURING HEIGHTENED SENSIVITY OF OUR ENVIRONMENT**
**Tactility**
-Capturing with different metrics, the effect of artificial and natural materials. To understand the partisipents hightened sensitivity through tactics and what is the difference between their perceptions and ours connected in the natural and built environment.
**Imaginations**
-Capturing how do we experience our built and natural environment through movements and bodies, with drawings generated by our movements.
To be able and imagine what we need in the spaces based on the generated drawings.

### Concept

An gamified audiovisual system, to capture different perception of different environments.
Capturing movements, sounds and sensing of materials. Visualizing the movements of the body in a space, the connection
with different materials in the natural or builr environment.

![concept-04](https://user-images.githubusercontent.com/92103034/171836534-033ea76d-cec9-4615-a418-924802a4c84b.png)



### Why?

### To understand our environment with a higher sensibility
![sensinf-01](https://user-images.githubusercontent.com/92103034/171842441-b733ba03-4375-4731-8f8c-22322b14651b.png)


### To help to sense our environment when there is limitations with our senses
![p030bb1t](https://user-images.githubusercontent.com/92103034/171842448-46180065-6d80-4e45-ab45-94af429a37d2.jpeg) 

### Purpose

To help to understand how kids with heightened sensivities (the ones who are actually affected by the built and natural environment around us) understand the environment around them, how they move around in spaces and what kind of materials are they connected to the most in different environments. And turn the data back to create better spaces which would support their tactile and imaginative development. 

To help people to understand more their surroundings and how they move around in spaces, to connect them to different materialities and understand their heightened sensivities and create and audiovisual experience from their perceptions. 


### Plan And Execution

### Gamified tactility game:
![tactility 26](https://user-images.githubusercontent.com/92103034/171842500-6a25c299-9b43-45ae-b595-6eb8a82f5078.png)

### Device for environmental sensing:

To connect them together into one artefact and to connect it to different sensivities we teamed up with Dídac and we created an artefact that can be carried around with wearing on our bodies and can create a gamified fun experience fow it's users.
![Untitled 19](https://user-images.githubusercontent.com/92103006/171863666-cc4b443f-a763-41e0-9bc7-c0e879132b8d.jpg)




### Fabrication Process and Materials

![fabrication_proccess-01](https://user-images.githubusercontent.com/92103034/171836492-4b694cf9-20f5-4d6a-afc1-36be91839017.png)

#### 3D printing:
- the ball - Semi transparent PETG
- 1 tactility element - white PLA (painted with spray paint)
- Positive shape for silicone mold

For the production of the ball, we decided to use 3D printing as a fabrication method since it was the one that offered us the most adaptability to all the electronic components and the functionalities we wanted it to have. We used Fusion 360 to make the 3D model of the ball and some other parts that would keep materials and everything in place. We designed it also in a modular way, creating some attachment points that would allow us to screw more components or structures inside if needed in the future.

For the printing part, we used Ultimaker Cura to slice each part in a way to reduce support structures and as a consequence also printing time. At the same time, this helped use less material and have less waste. We used PETG as the primary material for the ball because of its properties and considering that the ball would get some hit from time to time. The aim of using transparent PETG was also to be able to project light through the material from inside and give the ball a bit more life.

After printing, we added some inserts to the ball in order to use screws to join the different parts of the device.

![3d mdoel](https://user-images.githubusercontent.com/92103006/171870773-c2ba1572-3d58-4521-b229-4162c4d5125b.jpg)

![ezgif com-gif-maker](https://user-images.githubusercontent.com/92103006/171864562-d38142ba-029e-4990-816c-98c31acee472.gif)

![printed ball](https://user-images.githubusercontent.com/92103006/171866957-7913f788-bb8a-4126-a440-0cd0a98db166.jpg)

#### molding and casting:
- 1 tactility element: Hydrocal white (colored with black ink)
- 1 tactility element: Agar-agar biomaterial (colored with spirulina)

#### CNC milling:
- 1 tactility element: Birch wood 

#### Felting:
- 1 tactility element: Wool 

![fabrication_proccess-02](https://user-images.githubusercontent.com/92103034/171836513-2070d818-d162-4066-89fb-6c11f3f628d1.png)


#### Electronics
  - 1 huzzah feather ESP32
  - 1 Giroscop GY-61 accelrometer 
  - Microphoto 
  - 4 Piezo sensor with 10k resistor
  - 1 Battery 
  - LED lights 
 
References used 
- [1 Gyroscope GY-61 accelrometer](https://forum.arduino.cc/t/how-to-use-the-adxl355-or-gy-61-accelrometer/331047)
- [1 Microphone Analog Sound Sensor V2.2](https://www.e-tinkers.com/2019/10/using-a-thermistor-with-arduino-and-unexpected-esp32-adc-non-linearity/)
- [4 Piezo sensor with 10k resistor](https://www.arduino.cc/reference/en/libraries/thermistorlibrary/)
- [1 Battery ](https://www.arduino.cc/reference/en/libraries/thermistorlibrary/)
- [LED lights](https://www.arduino.cc/reference/en/libraries/thermistorlibrary/)
- [P5](https://p5js.org/reference/#/p5/line)
- [P5](https://p5js.org/reference/#/p5/strokeWeight)
- 4 1M Resistors 

#### Fabrication of Electronics 
For the Electronics part of the design we used The ESP32 Feather microcontroller. For this design we used different analog and transferred information through BlueTooth. The links of the tutorials we used are below, just some helpful tips with P5 Serial Controller on a window is that the select port is for both ports and BlueTooth so if you aren't seeing it show up don’t panic it is there. 
 
We connected all the different sensors slowly to make sure each worked with the code that was found in the links below. We had 6 different inputs. We had 4 Piezo Sensors that worked with the same code, we used these sensors to detect popularity in different materials, with using P5 we could see the date that is collected from each material. Each Piezo Sensor had a 1M Resistor attached to both the ground and the different pins. For the Mocrophone we connected the pins to V3, ground and an analog pin, we used a basic Arduino Code which will be collecting data.
The final sensor we used was the Giroscop this senor was the hardest to collect data from as we needed to figure out how to transform with p5 the direction if was going into to a data collected drawing. The pins we used was V3, ground and 3 different analogs.

Trying to understand such a complex code for the first time all 3 of us where doing was a bit challenging, but this didnt fase us to ge the out come we wanted. 


- [Analog Pins](https://learn.adafruit.com/adafruit-huzzah32-esp32-feather/pinouts)
- [Bluetooth](https://www.prometec.net/esp32-serial-bluetooth/)
- [Bluetooth with P5](https://itp.nyu.edu/physcomp/labs/labs-serial-communication/lab-serial-input-to-the-p5-js-ide/)
- [P5 with Gyroscope](https://p5js.org/reference/#/p5/strokeWeight)
- [P5 with Gyroscope](https://p5js.org/reference/#/p5/stroke)

#### System Diagram


![systemdiagramm-01](https://user-images.githubusercontent.com/92103034/171836607-36adfc45-8fe4-43bd-9fdb-fe8dce31ff39.png)


#### Integrated Design
![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/92103006/171867668-4d497e07-db03-4473-bf7c-b042d23ff174.gif)
![WhatsApp Image 2022-06-03 at 15 22 07](https://user-images.githubusercontent.com/92103006/171864777-0902cb98-bf31-4e92-886b-c081f213c51f.jpeg)
![WhatsApp Image 2022-06-03 at 15 22 57](https://user-images.githubusercontent.com/92103006/171864781-82359838-1649-4748-8da5-231993c31406.jpeg)



#### Future Development Opportunities

- Modular structure for the electronics inside the ball
- A shield for the esp feather
- Change of materials (matt material or a light in the ball) - for more friendly aesthetics
- Develope the interface of P5 for better understendable graphics


#### Hiccups
 
- A lots of lots of hiccups with the code, it was a platform for study for all of us as we were always in group with had people who knew more about coding then we did. But the fablab team helped us and showed us how eahc system worked on its own.
- The behaviour of the biomateriel, next time mold a bigger one than the exact shape and be aware of the shrink
- Some hiccups with the inside sturcture of the object
- Coming to the last 20min of thes eproject we had a fault in the electronics this made us not manage to take the ball with all the sensors to the workshop, never the less are good reserch designers we are we had some other tools up our sleave to see how to make this workshop still create the data we wanted. 


#### Open-source design and fabrication files

#### Stl files for 3D printing (PLA and PETG)
- Tactility element 1:

#### Rhino file for CNC milling: 


#### Recipe for the biomaterial (@Anna Mestres): 
- Agar agar: 4 gr
- Glicerin 10-15 ml
- Water 80 ml
- Microwave until it has a fom and bolis: 1,20 min

#### Hydrocal white: 
- 1:5 water and hydrocal

#### Codes:

- [P5](https://editor.p5js.org/philippa-Formosa/sketches/NT09r6K3H)
- [Arduino](https://www.notion.so/Fab-Challenge-4-a55f90cbd074407a86a914ada8ca7fbb)


