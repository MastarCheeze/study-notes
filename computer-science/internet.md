# Internet

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

> Routes data to a specific destination on a network

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

<br>

---

<br>

## MAC address[^MAC]

> Unique identifier (for NIC) \
> Assigned to NIC by manufacturer \
> Static

> `34:4D:EA:89:75:B2`

- Hexadecimal
- Separated by colons
- Manufacturer code + serial code

## IP address[^IP]

> Unique address (for device)

### Static

> Assigned by Internet Service Provider (ISP) \
> Does not change

### Dynamic

> Assigned by router \
> Changes each time device connects to network

### Types of IP addresses

| IPv4                 | IPv6                        |
| -------------------- | --------------------------- |
| `12.244.233.165`     | `2001:0db8::ff00:0042:7879` |
| 32-bit               | 128-bit                     |
| Separated by periods | Separated by colons         |

## URL[^URL]

> Text-based address (for website)

$$\large\underbrace{\textsf{https}}_{\text{protocol}}\textsf{://www.}\underbrace{\textsf{cambridge.org}}_{\text{domain name}}\textsf{/}\underbrace{\textsf{education}}_{\text{web page}}$$

## Protocols

### HTTP[^HTTP]

> Protocol used for transmission of web pages across internet

### HTTPS[^HTTPS]

> Secure version of HTTP \
> HTTP + SSL = HTTPS

- SSL (secure socket layer)
    - Security protocol
    - Encrypts data
    - Digital certificates
        - Authenticator
        - Contains public key
        - Requested by browser before allow communication
        - Awarded by certificate authority
- TLS (transport layer security)
    - Newer version of SSL

<br>

---

<br>

## Web browser

> Renders HTML and displays web pages

- Address bar
- Navigation tools
- Bookmark
- History
- Multiple tabs
- Cookies

## Scripting languages

### HTML[^HTML]

> Mark-up language to create web page

### CSS[^CSS]

> Define formatting/style of web page

### JavaScript

> Active script \
> Produce interactive elements of web page

## Cookies

> Data file \
> created/stored by web browser

<p></p>
Stores:

- Login details
- Credit card details
- Track history (for personalised ads)
- User preferences
- Items in shopping cart

### Session cookies

> Deleted when web browser is closed

### Persistent cookies

> Stored by web browser \
> until expired or deleted by user

<br>

---

<br>

> ## How web pages are requested
>
> 1. Browser sends URL to DNS
> 2. DNS sends IP address to browser
> 3. Browser locates web server with IP address \
>    requests web page
>    - using HTTP/HTTPS
> 4. Web server sends data to browser (HTML/CSS/JS)
>    - using HTTP/HTTPS
> 5. Browser
>    - Renders HTML and CSS
>    - Runs JavaScript

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
