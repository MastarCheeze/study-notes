# Hardware

# Von Neumann Architecture

## Components
- **CPU**
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
- **Storage**
    - Primary
        - [RAM](#primary) (random access memory)
        - [ROM](#primary) (read only memory)
    - Secondary
        - [Magnetic](#secondary)
        - [Optical](#secondary)
        - [Solid-state](#secondary)

#### CU



#### ALU

- Math calculations
- Logic operations
- Stored interim values in [ACC](#acc)

#### PC



#### MAR



#### MDR



#### CIR



#### ACC



#### Data bus



#### Address bus



#### Control bus



#### Core



#### Cache



#### Clock




## Stored program concept

- **Instructions** & **data** stored in memory
- Instructions **fetched → decoded → executed** one by one

<br>

# CPU[^CPU]

> Input \
> Process data and instructions \
> Output

## FDE cycle[^FDE]

> <p></p>
> <b><a href="#cu">CU</a></b> coordinates all operations in CPU
>
> - Transmits control signals to all components
> - Using [control bus](#control-bus)

### Fetch

![Fetch cycle](images/fetch.png)

1. **[PC](#pc)** stores address of next instruction (to be processed)
   - send to [MAR](#mar) - [Address bus](#address-bus)
2. **[MAR](#mar)** holds address of data/instruction (to be located in [RAM](#primary))
   - send to [RAM](#primary) - [Address bus](#address-bus)
3. [RAM](#primary) retrieves data/instruction
   - send to [MDR](#mdr) - [Data bus](#data-bus)
4. **[MDR](#mdr)** holds address of data/instruction (fetched from [RAM](#primary))
   - send to [CIR](#cir) - [Data bus](#data-bus)
5. **[CIR](#cir)** stores current instruction (being processed)

### Decode

6. **[CU](#cu)** decodes instruction into machine code
   - Using **instruction set** \
     (set of commands that are understood by CPU)

### Execute

7. **[ALU](#alu)** performs mathematical/logical operations (if needed)
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
If [RAM](#primary) is full

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

> Directly accessed by CPU

| RAM                                                                                                   | ROM                                                                                                                 |
| ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <p></p>Volatile<ul><li>Temporary storage</li><li>Contents are lost when power is turned off</li></ul> | <p></p>Non-volatile<ul><li>Permanent storage</li><li>Contents are preserved even when power is turned off</li></ul> |
| Stores data currently in use                                                                          | <p></p>Stores startup instructions<ul><li>Bootstrap</li><li>BIOS</li><li>Firmware</li></ul>                         |
| Contents constantly changing                                                                          | Contents fixed                                                                                                      |
| Can increase amount of RAM                                                                            | Cannot increase amount of ROM                                                                                       |

## Secondary

> Permanent data storage (non-volatile)
> <p></p>
> Cannot be directly accessed by CPU
>
> - Has to be sent to primary storage first

|                                    | Description                                                                                         | Examples                                                                 |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Magnetic                           | <ul><li>Uses **electromagnets**</li><li>Spinning platters (separated into tracks/sectors)</li></ul> | <ul><li>Hard disk drive (HDD)</li></ul>                                  |
| Optical                            | <ul><li>Uses **lasers**</li><ul><li>Pits/lands</li></ul></ul>                                       | <ul><li>CD</li><li>DVD</li><li>Blu-ray</li></ul>                         |
| Solid-state<br>(flash&nbsp;memory) | <ul><li>Uses **transistors**<ul><li>NAND/NOR</li><li>Control/floating gates</li></ul></li></ul>     | <ul><li><nobr>Solid-state</nobr> drive (SSD)</li><li>USB stick</li></ul> |

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
