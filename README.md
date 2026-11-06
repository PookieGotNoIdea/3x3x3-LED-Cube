# 3×3×3 LED Cube using Arduino Uno

This repository includes the code, hardware, assembly and documentation of my 3x3x3 LED Cube using the Arduino Uno.
The overall aim of this project was to create a 3D LED display. This consists of LEDs that can be programmed to show different lighting patterns. I wanted the LEDs to be set up in 3 layers rather than just being laid out flat.

The Arduino Uno is used to control the LEDs. The cube includes 27 LEDs, split into 3 layers with 9 LEDs per layer. This was connected together into horizontal layers and vertical columns so different lighting patterns could be shown.

The project was based around a tutorial, but some changes were made to suit the components I had. I used white LEDs rather than RGB, an Arduino Uno instead of an Arduino Nano and a cycle rim as part of the structure.

Throughout the project I have learnt how to set up LEDs, solder, wire up circuits and programme the Arduino. I have also learnt how challenging it can be to create a physical electronic structure.

The project involved learning about LED arrangements, soldering, circuit connections, Arduino programming, and the challenges of building a physical electronic structure.

<img width="1512" height="982" alt="image" src="https://github.com/user-attachments/assets/d778dc7d-c8b8-4527-963b-d627491b50bd" />

## Features

-LED Cube 3x3x3
-27 white LEDs
-Main controller: Arduino Uno
-3 horizontal LED layers
-9 vertical LED columns
-Horizontal layers are connected together via common cathodes.
-Each column is connected via individual anodes.
-LEDs can be programmed to light up in different patterns and animations.
-Arduino Uno powered via USB.
-Supporting frame made from whatever was available.
-Extra supporting base designed using Autodesk Fusion 360.

## BOM – Bill of Materials

| Component | Quantity | Purpose |
|---|---:|---|
| Arduino Uno | 1 | Main controller for the LED cube |
| White LEDs | 27 | Light-emitting elements |
| 220 Ω resistors | 3 | Current limiting |
| Cycle rim | As required | Supporting structure |
| Cardboard | 1 piece | Template for arranging LEDs |
| Thermocol | As required | Used during the structural build |
| Connecting wires | As required | Electrical connections |
| Soldering wire | As required | Joining LED terminals |
| USB cable | 1 | Programming and powering the Arduino |
| Supporting base | 1 | Base design for supporting the cube |

The components and materials were selected based on availability. I used white LEDs because I could not find the same RGB LEDs shown in the tutorial. I also used a cycle rim instead of an iron rod for the supporting structure.

## Circuit Diagram

The LED cube is wired using a row/column configuration. The rows (horizontal) of LEDs are all connected together to a common cathode connection. The positive legs of the LEDs are connected together into 9 columns.

This means that we can use the Arduino Uno to control the rows and columns to create a variety of lighting patterns.

### Main Connections

![LED Cube Circuit Diagram](images/circuit-diagram.png)

### LED Layer Connections

There are 9 LED's per horizontal layer. The negative leads are then bent and soldered to create a shared cathode connection.

Each horizontal layer has its own connection to the Arduino.

### LED Column Connections

The positive leads are then connected vertically for each of the 3 layers. This gives us 9 vertical columns.

We now have our main connections for controlling the cube.

### Arduino Connections

The Arduino Uno connects to the 3 horizontal and 9 vertical connections. We also need 3 220 Ω resistors in the circuit as shown in the tutorial.

**Important:** Make sure that the pins on the Arduino match those in the uploaded Arduino sketch. Once confirmed add the pin mapping below.

| LED Cube Connection | Arduino Uno Pin |
|---|---|
| Column 1 | Add pin number |
| Column 2 | Add pin number |
| Column 3 | Add pin number |
| Column 4 | Add pin number |
| Column 5 | Add pin number |
| Column 6 | Add pin number |
| Column 7 | Add pin number |
| Column 8 | Add pin number |
| Column 9 | Add pin number |
| Layer 1 | Add pin number |
| Layer 2 | Add pin number |
| Layer 3 | Add pin number |

The Arduino Uno can be powered via a USB connection to your computer. Before powering the cube, make sure all connections are made correctly.

## How to Build This

### Step 1 – Collect the Parts

Arduino Uno

27 LEDs

Three 220 Ω resistors

Connecting wires

Structure parts

I used white LEDs as I couldn’t find the exact RGB LEDs that were used in the tutorial.

### Step 2 – Make Template for LEDs

I made a template out of cardboard to keep the LEDs spaced out. The size of mine was roughly 5 x 5cm.

Nine holes were made in the cardboard to fit LEDs into. This helped me place them in a 3x3 formation.

![Cardboard LED Template]
<img width="1958" height="1524" alt="cardboard-template" src="https://github.com/user-attachments/assets/aae62288-d62a-45bd-a70d-938580b3ed92" />


### Step 3 – Build the LED Layers

Place nine LEDs into the template.

Solder the negative leads of the LEDs together after bending. This will provide a common cathode.

Repeat this to make three layers of LEDs (27 total).

![LED Layers]
![led-layers](https://github.com/user-attachments/assets/e2b2d662-6233-4208-91de-be1bd179d727)


### Step 4 – Assemble the 3D Structure

Once you have your three layers, stack them on top of each other.

The positive leads of the LEDs will be connected vertically making nine columns.

Instead of using an iron rod I used a cycle rim as I couldn’t get the material shown in the tutorial.

During the construction I also used some thermocol. However this caused problems as it began to melt when the soldering iron got close.

![LED Cube Structure]
<img width="1005" height="685" alt="cube-structure" src="https://github.com/user-attachments/assets/a7e8cc9d-1256-4c08-9555-598675466ff9" />


### Step 5 – Make Connections

Connect the three horizontal connections. Connect the nine vertical connections. Connect these to the Arduino Uno.

Use the three 220 Ω resistors. Connect them as shown in the wiring diagram.

Make sure the soldering and connections are correct.

![LED Cube Wiring]
<img width="1512" height="982" alt="cube-wiring-1" src="https://github.com/user-attachments/assets/bfd71469-0024-4441-84ad-15f73203d69a" />
![cube-wiring-2](https://github.com/user-attachments/assets/705940d2-93ed-4c44-9abc-9bb21efd188f)


### Step 6 – Connect Arduino

Connect the Arduino Uno to your computer.

I powered my Arduino using my MacBook so an external battery was not required.

### Step 7 – Upload Code

Open the sketch for the project in the Arduino IDE.

I used the code from the video description of the tutorial. I did not change any of the code.

Select the correct board type and port. Upload your sketch.

### Step 8 – Test LEDs

Upload your code and see if the LEDs light up as they should.

If some of your LEDs aren’t working, check the soldering points, connections between layers and column connections.

### Step 9 – Final Testing

Once your connections are working, test the different lighting patterns.

My final cube had several attempts. I fixed any wiring and soldering issues.

## LED Cube Structure

There are 27 individual LEDs.

There are 3 layers of 9 LEDs each. The layers are joined together via 9 columns.

The cardboard template ensured that there were gaps between the LEDs. The supporting structure also helped keep the layers together.

## Programming

The project uses the Arduino platform.

The main purpose of the code was to control the different layers and columns of LEDs.

The code was copied straight from the video description of the reference tutorial.

Key ideas used within the project were:
- Digital input/output using Arduino
- Controlling LEDs
- Connecting layers and columns
- Multiplexing the layers of LEDs
- Timing LED patterns
- Basic programming of embedded systems

### Code

The code can be found here in this repository.

**Main file:** `LED_Cube_3x3x3.ino`

Before uploading the code to the Arduino Uno you need to make sure the pins match up to what is in the code.


## CAD Models
I also created a supporting structure to be attached to the LED cube using **Autodesk Fusion 360**.

This helped provide a base for the structure.

By creating a CAD model I could create the supporting structure.

### Fusion 360 Model

![LED Cube Base - Fusion 360 Isometric View](images/cad-base-isometric.png)

### Sketch and Dimensions

![LED Cube Base - Fusion 360 Sketch](images/cad-base-sketch.png)

### Additional CAD Views

![LED Cube Base - Fusion 360 Additional View](images/cad-base-detail.png)

*The images in this section show the CAD design. They should not be interpreted as proof of physical fabrication unless the base was actually manufactured.*

## Working Principle

The main concept behind the LED cube is arranging the LEDs into 3 horizontal layers and 9 vertical lines.

Using the Arduino Uno we can control the connections between the layers and lines to create various lighting effects.

The 3 horizontal layers have common cathode connections. The nine vertical lines are formed using the positive connections of the LEDs.

By controlling the layers and lines in order the Arduino can create various patterns and animations.

This can be shown below:

```text
                  Arduino Uno
                      |
             +--------+--------+
             |                 |
        Layer Control     Column Control
             |                 |
       +-----+-----+           |
       |     |     |           |
     Layer Layer Layer         |
       1     2     3           |
       |     |     |           |
       +-----+-----+-----------+
                      |
                27 LED Cube
                      |
             Lighting Patterns
                 and Animations
```

It enabled the 3D set-up to be controlled using a small amount of connections.

## Challenges and Known Issues

During the construction and testing process, I faced a few practical challenges.

- **LED availability:** I could not find the same RGB LEDs shown in the tutorial, so I used white LEDs instead.
- **Structural material:** I used a cycle rim instead of an iron rod because the original material was not available.
- **Thermocol melting:** The thermocol started melting when the soldering iron came too close to it. I had to be careful while working around the structure.
- **LED alignment:** Keeping all nine LEDs evenly spaced in each layer required careful placement using the cardboard template.
- **Soldering:** Joining the LED legs and maintaining the correct layer and column connections required multiple attempts.
- **Circuit debugging:** Some wiring and soldering issues had to be corrected before all the LEDs worked properly.

These challenges helped me understand that building an electronic project involves more than just connecting components. Mechanical alignment, material selection, soldering, and circuit testing are equally important.

## Final Result

A fully functioning 3x3x3 cube was created with 27 white LEDs.

After several attempts and fixes to the soldering and wiring, all 27 LEDs were working and displaying the programmed lighting patterns and animations.

This helped with my understanding of how to program using Arduino, multiplexing LEDs, soldering, putting circuits together and how to create a 3D electronic object.

I had also got to use my mechanical design skills to create the base supporting model in Autodesk Fusion 360.

Despite a few material swaps and difficulties when building the cube I was able to complete the project successfully.

![Completed 3x3x3 LED Cube]
![final-cube](https://github.com/user-attachments/assets/61d5dc5f-27a1-43da-9e70-20aadb5786b4)


## Demo Video

Here is a video of how the LED cube works.

[**Watch the LED Cube Demo on YouTube**](ADDING_VIDEO_LINK_HERE)

## Reference
I followed the tutorial below to build and program my LED cube.

[**Original LED Cube Tutorial – YouTube**](ADDING_ORIGINAL_TUTORIAL_LINK_HERE)

This github includes details of how I have implemented the LED cube project. Including component replacements, assembly, wiring, CAD and testing.

## Future Improvements

Possible improvements to this project could include:

- Use RGB LEDs to allow more colour variation.
- Create a smaller and sturdier support structure.
- Create the base model from Fusion 360.
- Include more light patterns and effects.
- Improve the look of the project by having a proper housing/base.

---

**Project Status:** Completed
**Controller:** Arduino Uno
**LED Configuration:** 3×3×3 (27 LEDs)
**Programming Environment:** Arduino IDE
**CAD Software:** Autodesk Fusion 360
