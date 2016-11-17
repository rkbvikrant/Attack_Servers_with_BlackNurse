A simple PoC for the [Blacknurse][ref-1] attack.

"Blacknurse is a low bandwidth ICMP attack that is capable of doing denial of service to well known firewalls".

Blacknurse apparently makes the CPU hot on:

*  Cisco ASA 5505, 5506, 5515, 5525 , 5540 (default settings)
*  Cisco 6500 routers with SUP2T and Netflow v9 on the inbound interface - 100% CPU load
*  Cisco ASA 5550 (Legacy) and 5515-X (latest generation)
*  Cisco Router 897 - Can be mitigated
*  SonicWall - Misconfiguration can be changed and mitigated (Enable Anti-DDOS)
*  Palo Alto 5050 Firewalls with firmware 7.1.4-h2
*  Zyxel NWA3560-N (Wireless attack from LAN Side)
*  Zyxel Zywall USG50
*  Fortinet v5.4.1 - One CPU consumed
*  Fortigate units 60c and 100D (even with drop ICMP on)
*  SonicWall

Maybe more
See [blacknurse.dk][ref-2] for the full list and updates.

Vendor responses:

* [Checkpoint][ref-3]
* [Fortinet][ref-4]
* [Palo Alto][ref-5]

This attack is 20+ years old, but it didn't had a logo.
[ref-1]:http://www.blacknurse.dk/
[ref-2]:http://www.blacknurse.dk/
[ref-3]:https://supportcenter.checkpoint.com/supportcenter/portal?eventSubmit_doGoviewsolutiondetails=&solutionid=sk114500
[ref-4]:https://blog.fortinet.com/2016/11/14/black-nurse-ddos-attack-power-of-granular-packet-inspection-of-fortiddos-with-unpredictable-ddos-attacks
[ref-5]:http://researchcenter.paloaltonetworks.com/2016/11/note-customers-regarding-blacknurse-report/
