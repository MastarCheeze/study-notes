# Hardware

# Von Neumann Architecture

## Stored program concept

- **Instructions** & **data** stored in memory
- Instructions **fetched → decoded → executed** one by one

## Components
- [**CPU**](#cpu)
    - [CU](#cu) (control unit)
    - [ALU](#alu) (arithmetic logic unit)
    - Registers
        - [PC](#pc) (program counter)
        - [MAR](#mar) (memory address register)
        - [MDR](#mdr) (memory data register / buffer)
        - [CIR](#cir) (current instruction register) - inside CU
        - [ACC](#acc) (accumulator) - inside ALU
    - Buses
        - [Data bus](#data-bus)
        - [Address bus](#address-bus)
        - [Control bus](#control-bus)
    - [*Core*](#core)
    - [*Cache*](#cache)
    - [*Clock*](#clock)
- [**Storage**](#storage)
    - Primary
        - [RAM](#primary) (random access memory)
        - [ROM](#primary) (read only memory)
    - Secondary
        - [Magnetic](#secondary)
        - [Optical](#secondary)
        - [Solid-state](#secondary)

#### CU

- Coordinates all operations in CPU
    - Transmits control signals to all components
        - Using [control bus](#control-bus)
- Decodes instruction into machine code
    - Using **instruction set** \
      (set of commands that are understood by CPU)

#### ALU

- Math calculations
- Logic operations
- Stored interim values in [ACC](#acc)

#### PC

#### MAR

#### MDR

#### CIR

#### ACC

- Store interim values calculated by [ALU](#alu)

#### Data bus

- Bi-directional

#### Address bus

- Uni-directional

#### Control bus

- Bi-directional

#### Core

#### Cache

#### Clock

<br>

# CPU[^CPU]

> Process **data** and **instructions** \
> Perform **calculations** and **logical operations**

## FDE cycle[^FDE]

### Fetch

![Fetch cycle](images/fetch.png)

1. **[PC](#pc)** stores address of next instruction (to be processed)
   - copied to [MAR](#mar) - [Address bus](#address-bus)
2. **[MAR](#mar)** temporarily holds address of data/instruction (to be located in [RAM](#primary))
   - send to [RAM](#primary) - [Address bus](#address-bus)
3. [RAM](#primary) retrieves data/instruction
   - copied to [MDR](#mdr) - [Data bus](#data-bus)
4. **[MDR](#mdr)** temporarily holds address of data/instruction (fetched from [RAM](#primary))
   - send to [CIR](#cir) - [Data bus](#data-bus)
5. **[CIR](#cir)** stores current instruction (being processed)

### Decode

1. **[CU](#cu)** decodes instruction into machine code

### Execute

7. **[ALU](#alu)** performs calculations (if needed)
8. **[ACC](#acc)** stores interim values created by calculations

## Performance

- More cores
    - **[Core](#core)** - contains all components used for FDE cycle
    - Perform multiple FDE cycles at once
- Higher clock speed
    - **[Clock](#clock)** - synchronise components, controls speed of FDE cycle
- More cache
    - **[Cache](#cache)** - fast data storage inside CPU
    - Less time spent fetching data from [RAM](#primary)

## Virtual memory

> Partition in hard drive

<p></p>
If <a href="#primary">RAM</a> is full

1. **Page** is sent to virtual memory

<p></p>
When page is needed

2. Space made available in [RAM](#primary)
   - Send another page to CPU to process
   - Send another page to virtual memory
3. Page needed is sent back to [RAM](#primary)

<br>

# Microprocessor
> <p></p>
> Integrated circuit on a single chip
>
> - Limited instructions
> - Used in **embedded systems**
>   - Performs a dedicated function only

<br>

# Storage

## Primary

> **Directly accessed by CPU**

| RAM                                                                                                   | ROM                                                                                                                 |
| ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Stores data currently in use                                                                          | <p></p>Stores startup instructions<ul><li>Bootstrap</li><li>BIOS</li><li>Firmware</li></ul>                         |
| <p></p>Volatile<ul><li>Temporary storage</li><li>Contents are lost when power is turned off</li></ul> | <p></p>Non-volatile<ul><li>Permanent storage</li><li>Contents are preserved even when power is turned off</li></ul> |
| Can be written to<br>Contents constantly changing                                                     | Cannot be written to<br>Contents fixed                                                                              |
| Can increase amount of RAM                                                                            | Cannot increase amount of ROM                                                                                       |

## Secondary

> **Permanent** data storage (**non-volatile**)
> <p></p>
> <b>Cannot be directly accessed by CPU</b>
>
> - Has to be sent to primary storage first

|                                            | Description                                                                                                                                                                                                             | Examples                                                                                            |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Magnetic                                   | <ul><li>Read/write arm with<br>**electromagnets**</li><li>Spinning platters (separated into tracks/sectors)</li><li>Data stored as dots</li><ul><li>Magnetised = 1</li><li><nobr>Demagnetised = 0</nobr></li></ul></ul> | <ul><li>Hard disk drive (HDD)</li><li>Magnetic tape</li></ul>                                       |
| Optical                                    | <ul><li>Read/write arm with<br>**lasers** + **sensors**</li><ul><li>Burn pits</li><li>Read pits/lands<br>using reflections</li></ul></ul>                                                                               | <ul><li>CD[^CD]</li><li>DVD[^DVD]</li><li>Blu-ray</li></ul>                                         |
| <nobr>Solid-state</nobr><br>(flash memory) | <ul><li>Data flashed onto silicon chips</li><li>Uses **transistors**<ul><li>NAND/NOR<br>(flip-flop)</li><li>Control/floating gates</li><li>Control electron flow</li></ul></li><li>EEPROM technology</li></ul>          | <ul><li><nobr>Solid-state</nobr> drive (SSD)</li><li>USB flash drive</li><li>SD card[^SD]</li></ul> |

|             | Advantages                                                                                                                                                                 | Disadvantages |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| Magnetic    | <ul><li>Cheaper per storage unit</li><li>Longetivity</li></ul>                                                                                                             |
| Solid-state | <ul><li>Faster read/write speed</li><li>Low power consumption</li><li>Runs cooler</li><li>Portable (no moving parts)<br>Lighter<br>Smaller size per storage unit</li></ul> |


| Optical Storage | Differences                                                                                                 |
| --------------- | ----------------------------------------------------------------------------------------------------------- |
| CD / DVD        | <ul><li>Red laser</li><li>Less capacity</li><li>Slow transfer rate</li></ul>                                |
| Blu-ray         | <ul><li>Blue laser</li><li>More capacity</li><li>Fast transfer rate</li><li>Has secure encryption</li></ul> |

## Cloud

> Data stored in servers \
> Data can be accessed remotely

<br>

# Videos

- FDE cycle \
  [Craig'n'Dave](https://youtu.be/KBmoqwVt4Qg?si=3MH5FiUI4wUsV4zV&t=353)

<br>

[^CPU]: Central Processing Unit
[^FDE]: Fetch-Decode-Execute
[^CD]: Compact Disc
[^DVD]: Digital Versatile Disc
[^SD]: Secure Digital
