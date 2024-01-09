# Data transmission

- [Transmission](#transmission)
    - [Serial](#serial)
    - [Parallel](#parallel)
- [Direction](#direction)
    - [Simplex](#simplex)
    - [Half-duplex](#half-duplex)
    - [Full-duplex](#full-duplex)
- [Universal serial bus (USB)](#universal-serial-bus-usb)

<br>

# Transmission

## Serial

- Single wire
- One bit at a time

## Parallel

- Multiple wires
- Multiple bits simultaneously

<br>

|          | Advantages                                                                                                             | Disadvantages                                                                                                                        |
| -------- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Serial   | <ul><li>Less error</li><li>Less skew (arrive in order)</li><li>Less interference (single wire)</li><li>Cheap</li></ul> | <ul><li>Slow</li><li>Additional data (start/stop bit)</li></ul>                                                                      |
| Parallel | <ul><li>Fast</li></ul>                                                                                                 | <ul><li>More error</li><li>More skew (do not arrive in order)</li><li>More interference (multiple wires)</li><li>Expensive</li></ul> |

# Direction

## Simplex

- Transmission in one direction only

## Half-duplex

- Transmission in both directions
- But only one at a time

## Full-duplex

- Transmission in both directions
- At the same time

<br>

# Universal serial bus (USB)

- Industry standard used to transmit data
- Serial
- High-speed

<br>

|     | Advantages                                                                                                                                                                                                            | Disadvantages                                                                     |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| USB | <ul><li>Universal standard</li><li>Supports different transmission speeds</li><li>Can only fit one way</li><li>Backwards compatible</li><li>Automatically detect/download drivers</li><li>Can charge device</li></ul> | <ul><li>Limited transmission rate (500Mb/s)</li><li>Limited length (5m)</li></ul> |
