# [IKKE FÆRDIG]: Eksamensrapport - Mikkel Boye Rasmussen

## Kali Linux
For at lære at benytte Linux, har vi taget udgangspunkt i at læse bogen "Linux basics for hackers", hvorefter vi har suppleret med løsning af øvelserne i slutningen af de respektive kapitler. Vi har deraf været igennem et intensivt forløb indeholdende alt fra [basale terminal-kommandoer](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%201%20-%20Basics.md), til mere [systemnære kommandoer](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%207%20-%20Environment%20variables.md). Vi har gennemgået diverse råd til hvordan man kan [blive anonym på nettet](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%2013%20-%20Becoming%20secure%20and%20anonymous.md). Vi har lært at skrive vores egne [bash](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%208%20-%20Bash%20scripting.md) og python scripts. 

[Alle Linux Opgaver](https://github.com/MBRzealand/IT-sikkerhed/tree/main/Linux%20%C3%98velser)


## Kryptering og Kryptologi
Vi har i forbindelse med introforløbet været inde over kryptografi, kryptologi og steganografi, hvor vi har beskæftiget os med både [historiske chifre](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Historiske%20Chifre.md), [assymetrisk kryptering](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Asymmetrisk%20Kryptering.md) og [moderne Kryptografi](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Moderne%20Kryptografi.md). Vi har i undervisningen lært at anvende forskellige redskaber til kryptering/dekryptering samt steganografi. Eksempelvis har vi anvendt [Cyberchef](https://gchq.github.io/CyberChef/), [Steganography Online](https://stylesuxx.github.io/steganography/) og [Crackstation](https://crackstation.net/) til at prøve kræfter med de forskellige muligheder for at skjule data.

## Systemsikkerhed
I undervisningen har vi gennemgået diverse imødegåelsesstrategier i tilfælde af cyberangreb. Vi har gennemgået redskaber både til vurdering af hvilket angrebesstadie man befinder sig i ([Mitre ATT&CK](https://attack.mitre.org/)), men også awareness omkring de største typer af angreb der eksisterer derude ([OWASP](https://owasp.org/www-project-top-ten/)). På samme vis har vi gennemgået forskellige  analyseredskaber til at vurdere trusselsgraden af forskellige typer malware ([Hybrid Analysis](https://www.hybrid-analysis.com/)).

<b>Shodan aflevering</b><br/>
For at danne et overblik over trusselsbilledet har vi udarbejdet en opgave om redskabet Shodan. [Opgaven](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Systemsikkerhed/Shodan%20aflevering.md) har givet indblik i både mængden af devices der indeholder sikkerhedshuller, antallet af sikkerhedshuller per device, samt hvilke sårbarheder diverse devices typisk lider af. Opgaven har medvirket til at skabe awareness, da devices som valgmaskiner, vindmøller og ubådskontrolpaneler nemt kan findes. Ligeledes kan man se hvilke exploits et givent device vil være sårbar overfor.

<b>PicoCTF</b><br/>
Vi har skullet klargøre til vores første CTF-event ved at lave øvelser på platformen PicoGym, til at lære om diverse typer angreb og exploits man kan anvende på systemer, jeg har derigennem taget følgende flag:
<ul>
  <li>Obedient Cat</li>
  <li>Mod 26</li>
  <li>Nice netcat...</li>
  <li>Insp3ct0r</li>
  <li>Lets Warm Up</li>
  <li>Wireshark doo dooo do doo...</li>
  <li>where are the robots</li>
  <li>what's a netcat?</li>
  <li>13</li>
  <li>Inspect HTML</li>
  <li>Vigenere</li>
</ul>




## Netværk- og kommunikationssikkerhed


## Øvelser udover pensum

<b>Online Bootcamp</b><br/>
Jeg har valgt at supplere den viden vi får fra studiet, med kurser tilknyttet afholdelsen af [de danske mesterskaber i cybersikkerhed](https://www.cybermesterskaberne.dk/online-traening/). Igennem disse har jeg fået et par ugers forspring og deraf allerede fra start prøvet kræfter af med redskaber som **Hydra** og **metasploit**. I disse kurser har vi benyttet deres egen CTF-platform til at prøve kræfter af med forskellige XSS-angreb, packet sniffing samt exploits som Heartbleed og Samba.

<b>Fritid</b><br/>
I min fritid har jeg prøvet kræfter af med flere elementer af Aircrack-ng suiten, (airmon-ng, airodump-ng etc.) til at lave et evil twin angreb på min egen routers. Jeg har yderligere undersøgt hvordan photoshop kombineret med moderne AI-teknologier kan skjule billededata således forensics-redskaber som [Forensically](https://29a.ch/photo-forensics/) ikke kan vurdere hvorvidt billedet er ændret.

