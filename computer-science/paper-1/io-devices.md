# Contents

-   [Input devices](#input-devices)
    -   Mouse
        -   [Trackball](#trackball-mouse)
        -   [Optical](#optical-mouse)
    -   [Keyboard](#keyboard)
    -   [Microphone](#microphone)
    -   [Digital camera](#digital-camera)
    -   Code scanner
        -   [Barcode](#barcode-scanner)
        -   [QR code](#qr-code-scanner)
    -   Touch screen
        -   [Resistive](#resistive-touch-screen)
        -   [Capacitive](#capacitive-touch-screen)
        -   [Infrared (heat)](#infrared-touch-screen-heat)
        -   [Infrared (optical)](#infrared-touch-screen-optical)
    -   Scanner
        -   [2D](#2d-scanner)
        -   [3D](#3d-scanner)
    -   [Sensors](#sensors)
        -   Acoustic
        -   Accelerometer
        -   Flow
        -   Gas
        -   Humidity
        -   Infrared
        -   Level
        -   Light
        -   Magnetic field
        -   Moisture
        -   pH
        -   Pressure
        -   Proximity
        -   Temperature
-   [Output devices](#output-devices)
    -   Screen
        -   [LED](#led-screen)
        -   [LCD](#lcd-screen)
    -   [Speaker](#speaker)
    -   Projector
        -   [LCD](#lcd-projector)
        -   [DLP](#dlp-projector)
    -   Printer
        -   [Inkjet](#inkjet-printer)
        -   [Laser](#laser-printer)
    -   [3D printer](#3d-printer)
    -   [Actuator](#actuator)

<br><br>

# Input devices

### Trackball mouse

-   Mechanical ball

### Optical mouse

-   Red LED

### Keyboard

1. Each character has unique binary value
2. Converted into digital signal
    - Using character map
    - ASCII / Unicode

### Microphone

1. Sound causes diaphragm vibrate \
   Produces electric signal
2. ADC (sound card)

### Digital camera

1. Light pass through lens \
   onto light sensitive cell
2. Split into pixels \
   Measure light intensity of each pixel
3. Convert to binary

-   Microprocessor adjusts
    -   Shutter speed
    -   Focus

### Barcode scanner

> <p></p>
> Barcode
>
> -   Parallel dark/light lines
> -   0-9 represented by unique series of lines
> -   Left/right separate using guard bars

1. Red laser
2. Light reflected
    - Dark - reflect less
    - Light - reflect more
3. Photoelectric cells read reflected light
4. Reflections converted to binary

### QR code scanner[^QR]

> <p></p>
> QR code
>
> -   Matrix of dark squares on light background
> -   More storage than barcode
> -   Can store URL

1. Laser
2. Corners used to determine orientation
3. Light reflected
    - Dark - reflect less
    - Light - reflect more
4. Photoelectric cells read reflected light
5. Reflections converted to binary

### Resistive touch screen

> -   Upper layer polyester
> -   Bottom layer glass

1. When touched, top connects with bottom \
   Circuit complete
2. Processor calculates coordinate

### Capacitive touch screen

> -   Layers of glass
> -   Electric fields between glass layers \
>     Spread across screen

1. When touched, electric field changes \
   Affected by conductivity of finger
2. Sensor detects electric field
3. Processor calculates coordinate

### Infrared touch screen (heat)

> -   Glass screen

-   Needs warm object as input

### Infrared touch screen (optical)

> -   Expensive
> -   Glass screen
> -   Grid of sensors

-   Processor calculates coordinate \
    based on which grid coordinate is touched

| Resistive                         | Capacitive                              | Infrared                           |
| --------------------------------- | --------------------------------------- | ---------------------------------- |
| ✅ Cheap                          | ❌ Expensive                            | ❌ Expensive                       |
| ✅ Waterproof                     |                                         |                                    |
| ✅ Can be activated with anything | ❌ Must be activated with finger/stylus | ✅ Can be activated with anything  |
| ✅ Harder to shatter              | ❌ Easier to shatter                    | ❌ Easier to shatter               |
| ✅ Low power usage                |                                         |                                    |
| ❌ Short use life                 | ✅ Long use life                        | ✅ Long use life                   |
| ❌ Not sensitive                  | ✅ Sensitive                            | ✅ Sensitive <br> ❌ Too sensitive |
|                                   | ✅ Multitouch                           | ✅ Multitouch                      |
| ❌ Poor image quality             | ✅ Good image quality                   | ✅ Good image quality              |
| ❌ Poor visibility in sunlight    | ✅ Good visibility in sunlight          | ✅ Good visibility in sunlight     |

### 2D scanner

-   Scan hard-copy documents

1. Document placed on glass panel
2. Light illuminates document
3. Scan head moves across whole document
4. Light captured using mirrors/lenses
5. Light sensors detects light
6. Software produces digital image

### 3D scanner

-   Scan 3D objects
-   Take images at several points
-   Using
    -   Lasers
    -   Magnetic
    -   White light
-   Scanned images used in
    -   CAD (computer aided design)
    -   3D printing

### Sensors

> -   ADC (analogue-to-digital converter)

| Sensor (14)    | Measures                                 |
| -------------- | ---------------------------------------- |
| Acoustic       | Sound                                    |
| Accelerometer  | Acceleration forces (gravity/vibrations) |
| Flow           | Amount of fluid flowing                  |
| Gas            | Concentration of gas                     |
| Humidity       | Moisture in atmosphere                   |
| Infrared       |                                          |
| Level          | If liquid is at certain level            |
| Light          |                                          |
| Magnetic field |                                          |
| Moisture       | Moisture in soil                         |
| pH             |                                          |
| Pressure       |                                          |
| Proximity      | Distance (using echo)                    |
| Temperature    |                                          |

<br>

# Output devices

### LED screen[^LED]

-   Display made of pixels arranged in matrix
-   LEDs behind the screen
-   Light shone at pixels
-   Diffuser distributes light evenly
-   RGB filters
    -   mix to create different colours

### LCD screen[^LCD]

-   Front layer LCD
    -   Millions of liquid crystals arranged in matrix
-   LED backlight
    -   Reach max brightness immediately
    -   Higher resolution
    -   Better colour
    -   Thin screen
    -   Less power

<!---->

-   CCFL[^CCFL] backlight (old)
    -   Two fluorescent tubes
    -   Yellow tint

### Speaker

1. DAC (sound card)
2. Current amplifier
3. Cone vibrates at different frequencies
    - Caused by voltage differences

### LCD projector[^LCD]

> Old

1. White light
2. Light hits chromatic-coated mirrors \
   Splits into R, G, B light
3. R, G, B light pass through 3 LCD screens with grey image \
   Color image formed
4. Color image pass through lens, projected

### DLP projector[^DLP]

> New

1. White light
2. Pass through color filter \
   Splits into R, G, B light
3. Millions of micro-mirrors \
   Creates dark/bright pixels
    - Number of micro-mirrors = resolution
    - Tilt towards light = on \
      Tilt away from light = off

<br>

| LCD                           | DLP                            |
| ----------------------------- | ------------------------------ |
| ✅ Less expensive             | ❌ More expensive              |
| ✅ Less power                 | ❌ More power                  |
| ✅ High saturation (brighter) | ❌ Low saturation (dimmer)     |
| ✅ No rainbow effect          | ❌ Rainbow effect              |
| ✅ Quiet                      | ❌ Noisy                       |
| ❌ Bigger, heavier            | ✅ Smaller, lighter (portable) |
| ❌ Low contrast (dull)        | ✅ High contrast (vivid)       |
| ❌ Choppy video               | ✅ Smooth video                |

### Inkjet printer

> Print one-off documents

1. **Rollers** push paper
2. **Nozzle** spray ink on paper
3. **Print head** move across paper

-   **Piezoelectric** technology
    1. Electrical current applied to crystal
    2. Vibrates
    3. Forces droplet of ink through nozzle
-   **Thermal bubble** technology
    1. Ink heated
    2. Expands into bubble
    3. Bubble pushed through nozzle
    4. Bubble collapses

### Laser printer

> Print many documents

1. Printing **drum** (+ve charge)
2. **Laser** scans drum
    - Becomes -ve charge
3. Drum coated with **toner** (+ve charge)
    - Stick onto -ve charge area of drum
4. Drum rolled over paper (-ve charge)
    - Toner stick onto paper
5. Paper goes through fuser (heated rollers)
    - Toner melts
6. Discharge lamp
    - Removes all charges

<br>

| Inkjet printer            | Laser printer             |
| ------------------------- | ------------------------- |
| ✅ High quality           | ❌ Low quality            |
| ✅ No warm-up time        | ❌ Long warm-up time      |
| ✅ Various printing media | ❌ Limited printing media |
| ❌ Slow                   | ✅ Fast                   |
| ❌ Small volume printing  | ✅ Large volume printing  |
| ❌ Ink can be smudged     | ✅ No ink                 |

### 3D printer

-   Materials
    -   Plastic
    -   Resin
    -   Ceramic
-   Built layer by layer
-   Designed using CAD (computer aided design)

### Actuator

-   Cause physical movement
-   Operated by signals

<br>

[^QR]: Quick Response
[^LED]: Light Emitting Diode
[^LCD]: Liquid Crystal Display
[^CCFL]: Cold Cathode Fluorescent Lamps
[^DLP]: Digital Light Processing
