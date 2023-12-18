# Hardware

# Components <small><sup><sub>(Von Neumann architecture)</sub></sup></small>

- **CPU**
    - CU (control unit)
    - ALU (arithmetic logic unit)
    - Registers
        - PC (program counter)
        - MAR (memory address register)
        - MDR (memory data register / buffer)
        - CIR (current instruction register) - inside CU
        - ACC (accumulator) - inside ALU
    - Buses
        - Data bus
        - Address bus
        - Control bus
    - *Core*
    - *Cache*
    - *Clock*
- **Storage**
    - Primary
        - RAM (random access memory)
        - ROM (read only memory)
    - Secondary
        - Magnetic
        - Optical
        - Solid-state

<br>

# CPU[^CPU]

> Input \
> Process data and instructions \
> Output

## FDE cycle[^FDE]

> <p></p>
> <b>CU</b> coordinates all operations in CPU
>
> - Transmits control signals to all components
> - Using control bus

### Fetch

![Fetch cycle](images/fetch.png)

1. **PC** stores address of next instruction (to be processed)
   - send to MAR - Address bus
2. **MAR** holds address of data/instruction (to be located in RAM)
   - send to RAM - Address bus
3. RAM retrieves data/instruction
   - send to MDR - Data bus
4. **MDR** holds address of data/instruction (fetched from RAM)
   - send to CIR - Data bus
5. **CIR** stores current instruction (being processed)

### Decode

6. **CU** decodes instruction into machine code
   - Using **instruction set** \
     (set of commands that are understood by CPU)

### Execute

7. **ALU** performs mathematical/logical operations (if needed)
8. **ACC** stores interim values created by calculations

## Performance

- More cores
    - **Core** - contains all components used for FDE cycle
    - Perform multiple FDE cycles at once
- Higher clock speed
    - **Clock** - synchronise components, controls speed of FDE cycle
- More cache
    - **Cache** - fast data storage inside CPU
    - Less time spent fetching data from RAM

## Virtual memory

> Partition in hard drive

<p></p>
If RAM is full

1. **Page** is sent to virtual memory

<p></p>
When page is needed

2. Space made available in RAM
   - Send another page to CPU to process
   - Send another page to virtual memory
3. Page needed is sent back to RAM

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
| Stores data currently in use                                                                          | <p></p>Stores startup instructions<ul><li>Bootstrap</li><li>BIOS</li></ul>                                          |
| Contents constantly changing                                                                          | Contents fixed                                                                                                      |
| Can increase amount of RAM                                                                            | Cannot increase amount of ROM                                                                                       |

## Secondary

> Permanent data storage \
> Has to be sent to primary storage first to be accessed by CPU

|                                    |                                                                                                     |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- |
| Magnetic                           | <ul><li>Uses **electromagnets**</li><li>Spinning platters (separated into tracks/sectors)</li></ul> |
| Optical                            | <ul><li>Uses **lasers**</li><ul><li>Pits/lands</li></ul></ul>                                       |
| Solid-state<br>(flash&nbsp;memory) | <ul><li>Uses **transistors**<ul><li>NAND/NOR</li><li>Control/floating gates</li></ul></li></ul>     |

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
