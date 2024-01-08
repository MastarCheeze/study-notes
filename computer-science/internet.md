# Internet

- [Internet](#internet)
    - [Internet](#internet-1)
    - [World wide web](#world-wide-web)
    - [NIC](#nicnic)
    - [Router](#router)
    - [DNS](#dns)
    - [Web server](#web-server)
- [Addresses and Protocols](#addresses-and-protocols)
    - [MAC address](#mac-address)
    - [IP address](#ip-address)
    - [URL](#url)
    - [Protocols](#protocols)
        - [HTTP](#http)
        - [HTTPS](#https)
- [Web browser](#web-browser)
    - [Scripting languages](#scripting-languages)
    - [Cookies](#cookies)
    - [How web pages are requested](#how-web-pages-are-requested)
    - [How websites are authorised](#how-websites-are-authorised)


## Internet

> Infrastructure (physical) \
> Network of devices connected to each other

## World wide web

> Collection of websites and web pages \
> Accessed using the internet

## NIC[^NIC]

> Hardware component \
> for connecting to networks

## Router

> Forwards packets to a specific destination on a network

- Connects local network to the internet
- Assigns dynamic IP address

## DNS[^DNS]

> <p></p>
> Server with database of
>
> - Domain names (URL)
> - Corresponding IP addresses

## Web server

> Device where web pages for website are stored

<br><br>

# Addresses and Protocols

## MAC address[^MAC]

> Unique identifier (for device) \
> Assigned to NIC by manufacturer \
> Static
> Manufacturer code + serial code

`34:4D:EA:89:75:B2`

- 48-bit
- Hexadecimal

## IP address[^IP]

> Unique address (for device)

### Static

> Assigned by Internet Service Provider (ISP) \
> Does not change

### Dynamic

> Assigned by router \
> Changes each time device connects to network

### Types of IP addresses

| IPv4                        | IPv6                                   |
| --------------------------- | -------------------------------------- |
| `12.244.233.165`            | `2001:0db8::ff00:0042:7879`            |
| 32-bit                      | 128-bit                                |
| Denary                      | Hexadecimal                            |
| 0-255                       | 0000-FFFF                              |
| 4 groups of digits          | 8 groups of digits                     |
| Separated with dots         | Separated with colons                  |
| All 0s have to be displayed | 0000 can be omitted with double colons |

## URL[^URL]

> Text-based address (for website)

$$\large\underbrace{\textsf{https}}_{\text{protocol}}\textsf{://www.}\underbrace{\textsf{cambridge.org}}_{\text{domain name}}\textsf{/}\underbrace{\textsf{education}}_{\text{web page}}$$

## Protocols

### HTTP[^HTTP]

> Protocol used for transmission of web pages across internet

### HTTPS[^HTTPS]

> Secure version of HTTP \
> HTTP + SSL = HTTPS

- **SSL** (secure socket layer)
    - Security protocol
    - Encrypts data
    - Digital certificates
        - Contains public key
        - Awarded by certificate authority
- **TLS** (transport layer security)
    - Newer version of SSL

<br><br>

# Web browser

> <p></p>
> Displays web pages
>
> - Renders HTML
> - Runs active script

- Requests web pages from **web server**
- Manages protocols
    - Authenticates website
- Cookies
- Features
    - Create multiple tabs
    - History & bookmarks
    - Nav tools
    - Address bar
    - Downloads

## Scripting languages

### HTML[^HTML]

> Mark-up language to create web page

| Structure                   | Presentation                                  |
| --------------------------- | --------------------------------------------- |
| Layout                      | Formatting                                    |
| <ul><li>Placement</li></ul> | <ul><li>Colours</li><li>Font family</li></ul> |

### CSS[^CSS]

> Define formatting/style of web page

### JavaScript

> Active script \
> Produce interactive elements of web page

## Cookies

> Data file \
> created/stored by browser

<p></p>
Stores:

- Login details
- Credit card details
- Track history (for personalised ads)
- User preferences
- Items in shopping cart

### Session cookies

> Deleted when browser is closed \
> Stored in RAM

### Persistent cookies

> Stored until expired / deleted by user \
> Stored in secondary storage


## How web pages are requested

<p></p>
Using HTTP/HTTPS:

1. Browser sends URL to DNS
2. DNS looks up **matching** IP address
3. DNS sends IP address to browser
4. Browser locates web server with IP address \
   requests web page
5. Web server sends data to browser (HTML/CSS/JS)
6. Browser
   - Renders HTML and CSS
   - Runs JavaScript

## How websites are authorised

1. Browser requests certificate from web server
2. Receives copy of certificate
3. Checks if authentic
4. Sends signal to web server \
   that certificate is authentic
5. Establishes communication

<br>

[^NIC]: Network Interface Card
[^DNS]: Domain Name Server
[^MAC]: Media Access Control
[^IP]: Internet Protocol
[^URL]: Uniform Resource Locator
[^HTTP]: Hypertext Transfer Protocol
[^HTTPS]: Hypertext Transfer Protocol Secure
[^HTML]: Hypertext Markup Language
[^CSS]: Cascading Style Sheet
