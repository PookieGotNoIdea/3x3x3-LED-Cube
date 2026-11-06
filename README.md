3×3×3 LED Cube

A small LED cube made using an Arduino Uno and 27 white LEDs. Three layers, nine LEDs in each layer, all connected to create a 3D display that can show different lighting patterns and animations.

I followed a YouTube tutorial for this project, but I had to make a few changes because I couldn't find all the exact materials. I used white LEDs instead of RGB LEDs, an Arduino Uno instead of an Arduino Nano, and a cycle rim instead of the iron rod used in the tutorial.



Why I Made This

I wanted to try building something that wasn't just another basic Arduino project. A 3D LED cube looked interesting because it involved electronics, soldering, and a bit of mechanical work all in one project.

The idea was to arrange 27 LEDs into three layers and control them using an Arduino. It looked simple enough when I first saw the tutorial, but getting all the LEDs aligned, soldered, and connected properly turned out to be a different story.

What It Can Do

Display different LED patterns and animations.

Control 27 LEDs using an Arduino Uno.

Arrange LEDs into three horizontal layers and nine vertical columns.

Use a multiplexed layer-and-column connection.

Run from the Arduino's USB power.

Includes a supporting base CAD model designed in Fusion 360.

Components

## BOM – Bill of Materials

| Component | Quantity | Purpose |
|---|---:|---|
| Arduino Uno | 1 | Controls the LEDs |
| White LEDs | 27 | Creates the LED cube |
| 220 Ω resistors | 3 | Current limiting |
| Cardboard | 1 piece | LED spacing template |
| Cycle rim | As requirede | Structural support |
| Thermocol | As required | Used during assembly |
| Connecting wires | As required | Circuit connections |
| USB cable | 1 | Programming and power |


I used white LEDs because I couldn't find the RGB LEDs from the tutorial. The cycle rim was another substitution because I couldn't get the iron rod shown in the reference build.

## Circuit Diagram

The LED cube is wired using a row/column configuration. The rows (horizontal) of LEDs are all connected together to a common cathode connection. The positive legs of the LEDs are connected together into 9 columns.

This means that we can use the Arduino Uno to control the rows and columns to create a variety of lighting patterns.

### Main Connections

<img width="553" height="735" alt="Screenshot 2026-11-06 at 11 30 20 PM" src="https://github.com/user-attachments/assets/128e8f24-ad9f-44cf-807a-73290a158b55" />


### LED Layer Connections

There are 9 LED's per horizontal layer. The negative leads are then bent and soldered to create a shared cathode connection.

Each horizontal layer has its own connection to the Arduino.

### LED Column Connections

The positive leads are then connected vertically for each of the 3 layers. This gives us 9 vertical columns.

We now have our main connections for controlling the cube.

## How to Build This

Step 1 – Collect the Parts

Before starting, I gathered the components and materials needed for the build:

Arduino Uno

27 white LEDs

Three 220 Ω resistors

Connecting wires

Cardboard for making the LED template

Cycle rim for structural support

Thermocol (used during construction)

I used white LEDs because I couldn't find the exact RGB LEDs shown in the original tutorial.


Step 2 – Make the LED Template

I made a template out of cardboard to keep the LEDs properly spaced. The template was approximately 5 × 5 cm.

I made nine holes in the cardboard so that I could place the LEDs in a 3×3 formation. This made it easier to keep the LEDs aligned while soldering.

Cardboard template with nine holes for arranging the LEDs.
<img width="1958" height="1524" alt="cardboard-template" src="https://github.com/user-attachments/assets/aae62288-d62a-45bd-a70d-938580b3ed92" />


Step 3 – Build the LED Layers

I placed nine LEDs into the cardboard template for each layer.

After positioning them, I bent the negative legs of the LEDs and soldered them together to create a common cathode connection.

I repeated the same process to make three individual layers, giving me a total of 27 LEDs.

[led-layers]
<img width="553" height="735" alt="Screenshot 2026-11-06 at 11 30 20 PM" src="https://github.com/user-attachments/assets/14f67d25-4fca-481c-9f5e-607e96e362b4" />




Step 4 – Assemble the 3D Structure

Once all three layers were ready, I stacked them on top of each other to form the cube.

The positive legs of the LEDs were connected vertically to create nine columns across the three layers.

For the supporting structure, I used a cycle rim instead of an iron rod because I couldn't find the material used in the tutorial.

I also tried using thermocol during construction, but it started melting when the soldering iron came too close.

qwesaxz[LED Cube Structure]
<img width="553" height="735" alt="Screenshot 2026-11-06 at 11 30 20 PM" src="https://github.com/user-attachments/assets/45e60681-ac11-4c9a-acc5-8f8452b2e9d4" />



Step 5 – Make the Circuit Connections

After assembling the cube, I connected the three horizontal layers and nine vertical columns to the Arduino Uno.

I also used the three 220 Ω resistors in the circuit, following the wiring arrangement from the tutorial.

I checked the soldering points and connections carefully before powering up the circuit.


[LED Cube Wiring]
<img width="1512" height="982" alt="cube-wiring-1" src="https://github.com/user-attachments/assets/bfd71469-0024-4441-84ad-15f73203d69a" />
[cube-wiring-2]
<img width="553" height="735" alt="Screenshot 2026-11-06 at 11 30 20 PM" src="https://github.com/user-attachments/assets/23f43ce8-79a9-4355-9726-8843681ba212" />




Code

I used the code provided in the description of the reference tutorial and uploaded it through the Arduino IDE. I didn't make any changes to the original code.

The program controls the LED layers and columns in sequence to create the lighting patterns.

The main code is available here:
<img width="1366" height="768" alt="code" src="https://github.com/user-attachments/assets/ce1b92c2-5ba8-4930-98e7-51b6c69d3d46" />


CAD Model

I also designed a supporting base for the LED cube using Autodesk Fusion 360. The idea was to create a foundation that could support the structure.

I've included the CAD files in this repository:

Fusion 360 archive – 
<img width="1512" height="982" alt="Screenshot 2026-11-06 at 11 06 15 PM" src="https://github.com/user-attachments/assets/80496b71-12e2-474b-9392-380368cd8f97" />

STL model – 
<img width="1512" height="982" alt="Screenshot 2026-11-06 at 11 09 20 PM" src="https://github.com/user-attachments/assets/9d19d0da-8059-4220-aa34-c06157007780" />


The STL file can be opened in most 3D modelling and slicing applications.

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

A Few Problems Along the Way

It wasn't a perfect build on the first attempt.

Finding LEDs: I couldn't find the RGB LEDs used in the tutorial, so I switched to white LEDs.

Supporting the structure: I couldn't find the iron rod, so I used a cycle rim instead.

Thermocol: It started melting when the soldering iron came too close. Not exactly the best material to work around while soldering!

Soldering: Getting all the LED legs connected properly took multiple attempts.

Alignment: Keeping the LEDs evenly spaced and the three layers properly aligned needed patience.

I had to fix a few wiring and soldering issues along the way, but eventually all 27 LEDs worked.


Final Result

After all the assembly, soldering, and debugging, the cube finally worked as expected. All 27 LEDs were working, and the Arduino was able to display the programmed lighting patterns and animations.

It was a fun project and a good introduction to building something more physical with Arduino. I got to work with LED multiplexing, soldering, circuit connections, and even a little CAD design along the way.
<img width="558" height="743" alt="Screenshot 2026-11-06 at 11 29 07 PM" src="https://github.com/user-attachments/assets/4b68a639-1e38-465b-a789-d449c2101456" />



Reference

I used a YouTube tutorial as the reference for the LED arrangement, circuit connections, and Arduino code.

[Original tutorial – YouTube](https://youtu.be/Xd7PekWo_xs?si=PCvpikXvwghyTYnH)
