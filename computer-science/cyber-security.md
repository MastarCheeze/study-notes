# Cyber Security

- [Cyber Threats](#cyber-threats)
    - [Brute-force attack](#brute-force-attack)
    - [Data interception](#data-interception)
    - [DDoS attack](#ddos-attack)
    - [Hacking](#hacking)
    - [Malware](#malware)
    - [Phishing](#phishing)
    - [Pharming](#pharming)
    - [Social engineering](#social-engineering)
- [Prevention](#prevention-8)
    - [Strong password](#strong-password)
    - [Biometrics](#biometrics)
    - [Anti-malware](#anti-malware)
    - [Two-step verification](#two-step-verification)
    - [Firewall](#firewall)
    - [Proxy server](#proxy-server)
    - [Access levels](#access-levels)

<br>

# Cyber Threats

## Brute-force attack

> **Repeatedly guessing combinations of passwords until correct one is found \
> Can be manual/automated

#### Prevention
- [Two-step verification](#two-step-verification)
- [Strong password](#strong-password)
- [Biometrics](#biometrics)

## Data interception

> Packets are intercepted and monitored using **packet sniffers**

#### Prevention
- [HTTPS](./internet.md#https)

## DDoS attack[^DDoS]

> Deny people access to website \
> by crashing it

1. **Malware** is sent to computer
2. Computer becomes **bot**
   - Dormant computer: **zombie**
   - Network of bots: **botnet**
3. During attack (initiated by third party): \
   Web server **flooded** \
   with **numerous** requests simultaneously \
   using botnet
4. Server unable to handle, crash

#### Prevention
- [Proxy server](#proxy-server)
- [Firewall](#firewall)
- [Anti-malware](#anti-malware)

## Hacking

> Unauthorised access \
> by exploiting vulnerability in computer/network

#### Prevention
- [Firewall](#firewall)
- [Two-step verification](#two-step-verification)
- [Strong password](#strong-password)
- [Biometrics](#biometrics)
- Automatic software updates

## Malware

> Malicious software

| Malware      | Description                                                                                                                                                                                                                                                             |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Virus        | <ul><li>Replicates</li><li>Corrupts data</li><li>Fills up storage space</li><li>Clogs up memory</li></ul>                                                                                                                                                               |
| Worm         | <ul><li>Replicates</li><li>Clog up bandwidth</li></ul>                                                                                                                                                                                                                  |
| Spyware      | <ol><li>Record actions on computer<ul><li>Keylogger - records all keyboard presses</li></ul></li><li>Data sent back to perpetrator</li><li>Perpetrator analyses data</li><li>Common pattern used to identify password</li><li>Perpetrator can log in remotely</li></ol> |
| Ransomware   | <ul><li>Encrypt data to prevent access</li><li>Ransom to decrypt data</li></ul>                                                                                                                                                                                         |
| Adware       | <ul><li>Create ads automatically</li></ul>                                                                                                                                                                                                                              |
| Trojan horse | <ul><li>Malware disguised as harmless program</li></ul>                                                                                                                                                                                                                 |

#### Prevention
- [Anti-malware](#anti-malware)
- [Firewall](#firewall)
- Download from trusted sites
- Backup data

<!---->

- **Spyware**
    - [Two-step verification](#two-step-verification)
    - Partial password
    - Drop-down box for password
    - Virtual keyboard

## Phishing

> 1. Legitimate looking **email**
> 2. User **click** link to **fake website**
> 3. Enter personal details

#### Prevention
- Checking spelling/tone
- Visually checking website

## Pharming

> 1. Malware
> 2. **Redirects** to **fake website**
> 3. Enter personal details

#### Prevention
- [Anti-malware](#anti-malware)
- Download from trusted sites
- Visually checking website

## Social engineering

> Manipulating/deceiving people

#### Prevention
- [Access levels](#access-levels)

<br>

---

<br>

# Prevention

## Strong password

- Changing regularly
- Limiting number of tries

#### Used for
- [Brute-force attack](#brute-force-attack)
- [Hacking](#hacking)

## Biometrics

> Biological data

- Unique
- Quicker access

<!---->

- Examples
    - Fingerprint
    - Facial recognition
    - Retina recognition
    - Voice recognition

#### Used for
- [Brute-force attack](#brute-force-attack)
- [Hacking](#hacking)

## Two-step verification

> Input two different data to access device

- Verification code sent to email/phone
    - Difficult for perpetrator to obtain

#### Used for
- [Brute-force attack](#brute-force-attack)
- [Hacking](#hacking)

## Anti-malware

> Scans computer for virus

- Compare files with list of known malware
- If malware found, put into quarantine area for deletion

<!---->

- Examples
    - Anti-virus
    - Anti-spyware

#### Used for
- [Malware](#malware)
- [DDoS attack](#ddos-attack)
- [Pharming](#pharming)

## Firewall

> <p></p>
> Monitors incoming/outgoing traffic for
>
> - Network (software)
> - Computer (hardware)

- Set criteria (blacklist/whitelist)
    - Compare data with criteria
    - Reject data from passing through \
      if criteria is met
- Close unused ports
- Logs all attempts to access blocked websites

#### Used for
- [Malware](#malware)
- [Hacking](#hacking)
- [DDoS attack](#ddos-attack)

## Proxy server

> Monitors requests sent to web server

- Limit rate of requests if too many
- Caching - stop repeated requests from same IP address

#### Used for
- [DDoS attack](#ddos-attack)

## Access levels

> <p></p>
> Permissions
>
> - Limit data that can be read
> - Limit data that can be edited
> - Linked to a account / username

#### Used for
- [Social engineering](#social-engineering)

<br>

[^DDoS]: Distributed Denial of Service
