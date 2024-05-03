# Data Representation

-   [Text](#text)
    -   [Character set](#character-set)
    -   [ASCII](#ascii)
    -   [Unicode](#unicode)
-   [Images](#images)
    -   [JPEG](#jpeg)
-   [Sound](#sound)
    -   [MIDI](#midi)
    -   [MP3](#mp3)
-   [Video](#video)
    -   [MP4](#mp4)
-   [Units](#units)
-   [Compression](#compression)
    -   [Lossy](#lossy)
    -   [Lossless](#lossless)

## Text

### Character set

> All characters that can be represented \
> Each character has unique value

### ASCII

-   8-bit binary
-   256 characters

### Unicode

-   16-bit binary
-   65536 characters

## Images

-   Pixels
    -   Represent **one** colour
    -   Each colour has unique binary value
    -   Colour values stored in sequence
-   Resolution
    -   Dimensions of image
-   Colour depth
    -   Number of bits used to represent each colour

### JPEG[^JPEG]

> Lossy compression

-   Reduce resolution

## Sound

-   Sample rate
    -   Number of samples taken per second
    -   Pitch
-   Sample resolution
    -   Number of bits used to represent each sample
    -   Amplitude

### MIDI[^MIDI]

-   Protocol \
    Electronic musical instruments to interact with each other
-   Stored as series of demands (no music notes)
-   8-bit serial transmission

### MP3

> Lossy compression

-   Perceptual music shaping
    -   Removes sounds that cannot be heard by the human ear

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

-   Less storage space
-   Faster transmission
-   Faster upload/download time
-   Less bandwith required
-   Less buffering (video)

### Lossy

> **Compression algorithm** \
> Reduce file size by **permanently** removing data

### Lossless

> **Compression algorithm** \
> Reduce file size without **permanently** removing data \
> Original file can be restored

1. Finds **repeating** patterns
2. Indexes patterns
    - Store position
    - Store frequency

<p></p>
Example

-   Run length encoding (RLE)

<br>

| Lossy                                                                                          | Lossless                                                                                       |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| ✅ More compression <br> - Less storage space <br> - Faster transmission <br> - Less bandwidth | ❌ Less compression <br> - More storage space <br> - Slower transmission <br> - More bandwidth |
| ❌ Quality lost                                                                                | ✅ Quality preserved                                                                           |
|                                                                                                | ✅ Can edit original file                                                                      |

<br>

[^JPEG]: Joint Photographic Experts Group
[^MIDI]: Musical Instrument Digital Format
