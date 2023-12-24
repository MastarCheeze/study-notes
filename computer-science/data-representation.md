# Data Representation

- [Text](#text)
    - [ASCII](#ascii)
    - [Unicode](#unicode)
- [Images](#images)
    - [JPEG](#jpeg)
- [Sound](#sound)
    - [MIDI](#midi)
    - [MP3](#mp3)
- [Video](#video)
    - [MP4](#mp4)
- [Units](#units)
- [Compression](#compression)
    - [Lossy](#lossy)
    - [Lossless](#lossless)

## Text

### ASCII

- 8-bit binary
- 256 characters

### Unicode

- 16-bit binary
- 65536 characters

## Images

- Resolution
    - Dimensions of image
- Colour depth
    - Number of bits used to represent each colour

### JPEG[^JPEG]

> Lossy compression

- Reduce resolution

## Sound

- Sample rate
    - Number of samples taken per second
- Sample resolution
    - Number os bits used to represent each sample

### MIDI[^MIDI]

- Protocol \
  Electronic musical instruments to interact with each other
- Stored as series of demands (no music notes)
- 8-bit serial transmission

### MP3

> Lossy compression

- Perceptual music shaping
    - Removes sounds that cannot be heard by the human ear

## Video

### MP4

<br><br>

## Units

|                 |            |                      |
| --------------- | ---------- | -------------------- |
| Bit             |            |                      |
| Nibble          | 4 bits     |                      |
| Byte            | 8 bits     |                      |
| Kibibtye (KiB)  | 1024 bytes | 2<sup>10</sup> bytes |
| Mebibtye (MiB)  | 1024 KiB   | 2<sup>20</sup> bytes |
| Gibibtye (GiB)  | 1024 MiB   | 2<sup>30</sup> bytes |
| Tebibtye (TiB)  | 1024 GiB   | 2<sup>40</sup> bytes |
| Pebibtye (PiB)  | 1024 TiB   | 2<sup>50</sup> bytes |
| Exibibtye (EiB) | 1024 EiB   | 2<sup>60</sup> bytes |

## Compression

> Algorithm

- Less storage
- Faster transmission
- Faster upload/download time
- Less bandwith required

### Lossy

> Reduce file size by permanently removing data

### Lossless

> Reduce file size without permanent loss of data \
> Original file can be restored

1. Finds **repeating** patterns
2. Indexes patterns
    - Store position
    - Store frequency

<p></p>
Example

- Run length encoding (RLE)

<br>

|          | Advantages                          | Disadvantages                      |
| -------- | ----------------------------------- | ---------------------------------- |
| Lossy    | <ul><li>More compression</li></ul>  |
| Lossless | <ul><li>Quality preserved</li></ul> | <ul><li>Less compression</li></ul> |

<br>

[^JPEG]: Joint Photographic Experts Group
[^MIDI]: Musical Instrument Digital Format
