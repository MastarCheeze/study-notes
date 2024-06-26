# Hardware

-   [Von Neumann Architecture](#von-neumann-architecture)
    -   [Stored program concept](#stored-program-concept)
    -   [Components](#components)
-   [CPU](#cpu)
    -   [FDE cycle](#fde-cycle)
        -   [Fetch](#fetch)
        -   [Decode](#decode)
        -   [Execute](#execute)
    -   [Performance](#performance)
    -   [Virtual memory](#virtual-memory)
-   [Microprocessor](#microprocessor)
    -   [Embedded systems](#embedded-systems)
-   [Storage](#storage)
    -   [Primary](#primary)
    -   [Secondary](#secondary)
    -   [Cloud](#cloud)

<br>

# Von Neumann Architecture

## Stored program concept

-   **Instructions** & **data** stored in memory
-   Instructions **fetched → decoded → executed** one by one

## Components

-   [**CPU**](#cpu)
    -   [CU](#cu) (control unit)
    -   [ALU](#alu) (arithmetic logic unit)
    -   Registers
        -   [PC](#pc) (program counter)
        -   [MAR](#mar) (memory address register)
        -   [MDR](#mdr) (memory data register / buffer)
        -   [CIR](#cir) (current instruction register) - inside CU
        -   [ACC](#acc) (accumulator) - inside ALU
    -   Buses
        -   [Data bus](#data-bus)
        -   [Address bus](#address-bus)
        -   [Control bus](#control-bus)
    -   [_Core_](#core)
    -   [_Cache_](#cache)
    -   [_Clock_](#clock)
-   [**Storage**](#storage)
    -   Primary
        -   [RAM](#primary) (random access memory)
        -   [ROM](#primary) (read only memory)
    -   Secondary
        -   [Magnetic](#secondary)
        -   [Optical](#secondary)
        -   [Solid-state](#secondary)

#### CU

-   Control signals
    -   Via [control bus](#control-bus)
    -   Controls transfer of data & instructions \
        between CPU and components
    -   Synchronises FDE cycle
-   Decodes instruction into machine code
    -   Using **instruction set** \
        (set of commands that are understood by CPU)

#### ALU

-   Math calculations
-   Logic operations
-   Stored interim values in [ACC](#acc)

#### PC

#### MAR

-   Stores addresses of data/instructions
-   to be fetched from memory \
    to be written to memory

#### MDR

-   Stores data/instructions
-   has been fetched from memory \
    to be written to memory

#### CIR

#### ACC

-   Store interim values calculated by [ALU](#alu)

#### Data bus

-   Bi-directional

#### Address bus

-   Uni-directional

#### Control bus

-   Bi-directional

#### _Core_

#### _Cache_

-   Volatile storage
-   Store frequently accessed data/instructions
-   Speed up access
    -   Faster than RAM
-   Has levels L1, L2, L3

#### _Clock_

-   **Regulates** number of FDE cycles CPU can perform in a second

<br>

# CPU[^CPU]

> Process **data** and **instructions** \
> Perform **calculations** and **logical operations** \
> Carry out FDE cycle

## FDE cycle[^FDE]

### Fetch

![Fetch cycle](../images/fetch.png)

1. **[PC](#pc)** stores address of next instruction (to be processed)
    - copied to [MAR](#mar) via [Address bus](#address-bus)
2. **[MAR](#mar)** temporarily holds address of data/instruction (to be located in [RAM](#primary))
    - send to [RAM](#primary) via [Address bus](#address-bus)
3. [RAM](#primary) retrieves data/instruction
    - copied to [MDR](#mdr) via [Data bus](#data-bus)
4. **[MDR](#mdr)** temporarily holds data/instruction (fetched from [RAM](#primary))
    - send to [CIR](#cir) via [Data bus](#data-bus)
5. **[CIR](#cir)** stores current instruction (being processed)
    - send to [CU](#cu) via [Data bus](#data-bus)

### Decode

6. **[CU](#cu)** decodes instruction into machine code \
   using instruction set

### Execute

7. **[ALU](#alu)** performs calculations (if needed)
8. **[ACC](#acc)** stores interim values created by calculations

## Performance

-   More cores
    -   **[Core](#core)** - contains all components used for FDE cycle
    -   Perform multiple FDE cycles at once
-   Higher clock speed
    -   **[Clock](#clock)** - synchronise components, controls speed of FDE cycle
-   More cache
    -   **[Cache](#cache)** - fast data storage inside CPU
    -   Less time spent fetching data from [RAM](#primary)

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
> -   Limited instructions
> -   Used in **embedded systems**

### Embedded systems

-   Performs a dedicated function only
-   Cannot be reprogrammed
-   Has
    -   Microprocessor
    -   Dedicated hardware
    -   Firmware

<br>

# Storage

## Primary

> **Directly accessed by CPU**

| RAM                                                                                                                                            | ROM                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Stores current running...<ul><li>Instructions</li><li>Data</li><li>Application software</li><li>Utility software</li><li>Parts of OS</li></ul> | Stores... <ul><li>Startup instructions</li><li>Firmware</li><ul><li>BIOS</li><li>Bootstrap</li></ul></ul>    |
| Volatile<ul><li>Temporary storage</li><li>Contents are lost when power is turned off</li></ul>                                                 | Non-volatile<ul><li>Permanent storage</li><li>Contents are preserved even when power is turned off</li></ul> |
| Can be written to<br>Contents constantly changing                                                                                              | Cannot be written to<br>Contents fixed                                                                       |
| Can increase amount of RAM                                                                                                                     | Cannot increase amount of ROM                                                                                |

## Secondary

> **Permanent** data storage (**non-volatile**)
>
> <p></p>
> Stores...
>
> -   data currently not required by CPU
> -   data to transfer to other devices
>
> <p></p>
> <b>Cannot be directly accessed by CPU</b>
>
> -   Has to be sent to primary storage first

|                                            | Description                                                                                                                                                                                                                                                          | Examples                                                                                            |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Magnetic                                   | <ul><li>Data stored on platters</li><li>Platters divided into tracks/sectors</li><li>Platters can spin</li><li>Read/write arm with<br>**electromagnets**</li><li>Data stored as dots</li><ul><li>Magnetised = 1</li><li><nobr>Demagnetised = 0</nobr></li></ul></ul> | <ul><li>Hard disk drive (HDD)</li><li>Magnetic tape</li></ul>                                       |
| Optical                                    | <ul><li>Read/write arm with<br>**lasers** + **sensors**</li><ul><li>Burn pits</li><li>Read pits/lands<br>using reflections</li></ul></ul>                                                                                                                            | <ul><li>CD[^CD]</li><li>DVD[^DVD]</li><li>Blu-ray</li></ul>                                         |
| <nobr>Solid-state</nobr><br>(flash memory) | <ul><li>Uses flash memory</li><li>Data flashed onto chips</li><li>Uses **transistors**<ul><li>NAND/NOR<br>(flip-flop)</li><li>Control gates</li><li>Floating gates</li><li>Control electron flow</li></ul></li><li>Type of EEPROM</li></ul>                          | <ul><li><nobr>Solid-state</nobr> drive (SSD)</li><li>USB flash drive</li><li>SD card[^SD]</li></ul> |

| Magnetic           | Solid-state                   |
| ------------------ | ----------------------------- |
| ✅ Large capacity  | ✅ Large capacity             |
| ✅ Cheap           | ❌ Expensive                  |
| ✅ Long life       | ❌ Short life                 |
| ❌ Slow read/write | ✅ Fast read/write            |
| ❌ High power      | ✅ Low power                  |
| ❌ Moving parts    | ✅ No moving parts (portable) |
| ❌ Larger size     | ✅ Smaller size               |

| Optical Storage | Differences                                                                                                 |
| --------------- | ----------------------------------------------------------------------------------------------------------- |
| CD / DVD        | <ul><li>Red laser</li><li>Less capacity</li><li>Slow transfer rate</li></ul>                                |
| Blu-ray         | <ul><li>Blue laser</li><li>More capacity</li><li>Fast transfer rate</li><li>Has secure encryption</li></ul> |

## Cloud

> Data stored in servers \
> Data can be accessed remotely through network

<br>

# Videos

-   FDE cycle \
    [Craig'n'Dave](https://youtu.be/KBmoqwVt4Qg?si=3MH5FiUI4wUsV4zV&t=353)

<br>

[^CPU]: Central Processing Unit
[^FDE]: Fetch-Decode-Execute
[^CD]: Compact Disc
[^DVD]: Digital Versatile Disc
[^SD]: Secure Digital
