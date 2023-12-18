# Cyber Security

## Brute-force Attack

> Repeatedly guessing password until correct one is found

#### Prevention
- Strong password
- Biometrics (e.g. fingerprints)
- Limiting password tries
- [Two-step verification](#two-step-verification)

## Data Interception

> Packets are intercepted and examined using **packet sniffers**

#### Prevention
- [HTTPS](./internet.md#https)

## DDoS Attack[^DDoS]

> Flood server with requests using **botnet** \
> to cause it to crash

1. **Malware** is sent to computer
2. Computer becomes **bot**
   - Dormant computer: **zombie**
   - Network of bots: **botnet**

#### Prevention
- [Proxy server](#proxy-server)
- [Anti-malware](#anti-malware)

## Hacking

> Unauthorised access \
> by exploiting vulnerability in computer/network

#### Prevention
- [Firewall](#firewall)
- Automatic software updates
- Strong password
- Biometrics (e.g. fingerprints)
- [Two-step verification](#two-step-verification)

## Malware

> Malicious software

| Malware      | Description                                                                                            |
| ------------ | ------------------------------------------------------------------------------------------------------ |
| Virus        | <ul><li>Replicates</li><li>Corrupts data</li><li>Uses up memory</li></ul>                              |
| Worm         | <ul><li>Replicates</li><li>Clog up bandwidth</li></ul>                                                 |
| Trojan horse | <ul><li>Malware disguised as harmless program</li></ul>                                                |
| Spyware      | <ul><li>Record actions on computer<ul><li>Keylogger - records all keyboard presses</li></ul></li></ul> |
| Adware       | <ul><li>Create ads automatically</li></ul>                                                             |
| Ransomware   | <ul><li>Encrypt data to prevent access</li><li>Ransom to decrypt data</li></ul>                        |

#### Prevention
- [Anti-malware](#anti-malware)
- [Firewall](#firewall)
- Download from trusted sites
- Backup data

## Pharming

> Malware \
> redirects to fake website

#### Prevention
- [Anti-malware](#anti-malware)
- Download from trusted sites
- Visually checking website

## Phishing

> Email \
> link to fake website

#### Prevention
- Checking spelling/tone
- Visually checking website

## Social Engineering

> Manipulating/deceiving people

#### Prevention
- [Access levels](#access-levels)

<br>

---

<br>

# Prevention

## Anti-malware

<p></p>
Also

- Anti-virus
- Anti-spyware

> Scans computer for virus

- Compare files with list of known malware
- If malware found, put into quarantine area for deletion

#### Used for
- [Malware](#malware)
- [DDoS attack](#ddos-attackddos)
- [Pharming](#pharming)

## Two-step verification

> Input two different data to access device

- Verification code sent to email/phone

#### Used for
- [Brute-force attack](#brute-force-attack)
- [Hacking](#hacking)

## Firewall

> Examine traffic from a computer or network

- Reject data from passing through
- Close unused ports

#### Used for
- [Malware](#malware)
- [Hacking](#hacking)

## Proxy server

> Examines requests sent to web server

- Limit rate of requests if too many
- Caching - stop repeated requests from same IP address

#### Used for
- [DDoS attack](#ddos-attackddos)

## Access levels

> Limit amount of data that can be accessed \
> by employee

#### Used for
- [Social engineering](#social-engineering)

<br>

[^DDoS]: Distributed Denial of Service
