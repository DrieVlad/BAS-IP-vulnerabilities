# BAS-IP-vulnerabilities

## CVE-2024-37654

An issue in BAS-IP AV-01D, AV-01MD, AV-01MFD, AV-01ED, AV-01KD, AV-01BD, AV-01KBD, AV-02D, AV-02IDE, AV-02IDR, AV-02IPD, AV-02FDE, AV-02FDR, AV-03D, AV-03BD, AV-04AFD, AV-04ASD, AV-04FD, AV-04SD, AV-05FD, AV-05SD, AA-07BD, AA-07BDI, BA-04BD, BA-04MD, BA-08BD, BA-08MD, BA-12BD, BA-12MD, CR-02BD before 3.9.2 allows a remote attacker to obtain RTSP passwords via a crafted HTTP GET request.

### Exploitation
Web interface administrator credentials required.

1. Access the web interface
2. Execute an HTTP GET request to /api/v1/device/settings/rtsp
3. Find the cleartext password in the received HTTP response

<img width="291" alt="Снимок экрана 2024-06-20 в 00 13 47" src="https://github.com/DrieVlad/BAS-IP-vulnerabilities/assets/43147263/dd0fe40b-2dea-4976-801b-3476d564f5e5">


To fix the vulnerability, install the update.

## Remediation
Update firmware to version 3.9.2 or later. 
Details on the official website. https://bas-ip.com/bsa-000001
