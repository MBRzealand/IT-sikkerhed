# [FÆRDIG]: Eksamensrapport - Mikkel Boye Rasmussen

## Indledning
Introforløbet har haft en praktisk-teoretisk tilgang hvor de forskellige fags undervisningselementer naturligt overlapper. Vi har haft en indgangsvinkel, hvor vi selv har fået lov til at prøve kræfter af med forskellige typer cyberangreb. Deraf har vi fået hands-on viden/erfaring vedrørende hvilke trusler en virksomhed kan være udsat for, samt skabt bedre vilkår for at vi kan mitigere risici forbundet med cyberangreb. I min optik kan undervisningsstrukturen og den generelle røde tråd i forløbet, ses lidt som de forskellige indledende skridt for at kunne udføre en pentest. 

- Vi har lært hvordan man kan identificere et sårbart system, samt typiske systemsvagheder.
- Vi har igennem netværksteori lært hvordan man kan tilslutte sig et system, samt aflæse trafik.
- Vi har lært linux således vi kan navigere og kontrollere de systemer vi tilslutter os.
- Vores mere komplekse linux undervisning har lært os at hente data, samt slette vores spor.
- Vi har lært om kryptering og kryptologi således vi kan få information ud af de tilgåede data.
- Til sidst har vi fået opsat diverse troværdige virtuelle miljø hvor vi etisk kan prøve kræfter af med vores nye viden.

Denne proces kulminerer til sidst i vores første CTF-event hvor alt denne viden skal anvendes.

Arbejdsbyrden jeg har lagt i forståelsen af disse forskellige processkridt kan ses nedenfor, ligeledes er hele GitHub repositoriet en samling af alt hvad jeg har udarbejdet i forbindelse med introforløbet, inklusiv [forelæsningsnoter](https://github.com/MBRzealand/IT-sikkerhed/tree/main/Forel%C3%A6sningsnoter).


## Kali Linux
For at lære at anvende Linux, har vi taget udgangspunkt i at læse bogen "Linux basics for hackers", hvorefter vi har suppleret med løsning af øvelserne i slutningen af de respektive kapitler. Vi har deraf været igennem et intensivt forløb indeholdende alt fra [basale terminal-kommandoer](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%201%20-%20Basics.md), til mere [systemnære kommandoer](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%207%20-%20Environment%20variables.md). Vi har gennemgået diverse råd til hvordan man kan [forblive anonym på nettet](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%2013%20-%20Becoming%20secure%20and%20anonymous.md). Yderligere har vi lært at skrive vores egne [bash](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/%C3%98velser%20kapitel%208%20-%20Bash%20scripting.md) scripts samt vurderet disse [python scripts](https://github.com/andracs/Ovelser-til-kapitel-17). Til sidst har vi har lært at anvende SSH samt hydra til at cracke ind i en server samt hvordan man kan udføre et DDOS angreb.

Alle Linux opgaverne løst af mig, kan findes [her](https://github.com/MBRzealand/IT-sikkerhed/tree/main/Linux%20%C3%98velser).


## Kryptering, Kryptologi og Kryptografi
Vi har i forbindelse med introforløbet været inde over kryptografi, kryptologi og steganografi, hvor vi har beskæftiget os med [historiske chifre](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Historiske%20Chifre.md), [assymetrisk kryptering](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Asymmetrisk%20Kryptering.md) og [moderne Kryptografi](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Krypterings%C3%B8velser/Moderne%20Kryptografi.md). Vi har i undervisningen lært at anvende forskellige redskaber til kryptering/dekryptering samt steganografi. Eksempelvis har vi anvendt [Cyberchef](https://gchq.github.io/CyberChef/), [Steganography Online](https://stylesuxx.github.io/steganography/) og [Crackstation](https://crackstation.net/) til at prøve kræfter med de forskellige muligheder for at skjule data.

## Systemsikkerhed
I undervisningen har vi gennemgået diverse imødegåelsesstrategier i tilfælde af cyberangreb. Vi har gennemgået redskaber både til vurdering af hvilket angrebsstadie man befinder sig i ([Mitre ATT&CK](https://attack.mitre.org/)), men også awareness omkring de største typer af angreb der eksisterer derude ([OWASP](https://owasp.org/www-project-top-ten/), [Recorded Future](https://www.recordedfuture.com/) og [Enisa](https://www.enisa.europa.eu/topics/cyber-threats/threats-and-trends)). På samme vis har vi gennemgået forskellige  analyseredskaber til at vurdere trusselsgraden af forskellige typer malware ([Hybrid Analysis](https://www.hybrid-analysis.com/)).

<b>Shodan aflevering</b><br/>
For at danne et overblik over trusselsbilledet har vi udarbejdet en opgave om redskabet Shodan. [Opgaven](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Systemsikkerhed/Shodan%20aflevering.md) har givet indblik i både mængden af devices der indeholder sikkerhedshuller, antallet af sikkerhedshuller per device, samt hvilke sårbarheder diverse devices typisk lider af. Opgaven har medvirket til at skabe awareness, da devices som valgmaskiner, vindmøller og ubådskontrolpaneler nemt kan findes. Ligeledes kan man se hvilke exploits et givent device vil være sårbar overfor.

<b>PicoCTF</b><br/>
Vi har skullet klargøre til vores første CTF-event ved at lave øvelser på platformen [PicoGym](https://play.picoctf.org/practice), til at lære om diverse typer angreb og exploits man kan anvende på systemer, jeg har derigennem taget følgende flag:

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
I netværk og kommunikationssikkerhed har hovedfokus været 5-lags modellen og grundlæggende netværksteori. Vi har dog haft den praktiske indgangsvinkel, at vi skal blive avancerede brugere af redskabet WireShark, til at få dybdegående forståelse netværkstrafik. Heraf har vi været udsat for [diverse øvelser](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Netv%C3%A6rk%20og%20kommunikationssikkerhed/Network%20Challenge.md) hvor vi skulle snuse rundt i netværkstrafik samt vurdere hvad har foregået.


## Øvelser udover pensum

<b>Online Bootcamp</b><br/>
Jeg har valgt at supplere den viden vi får fra studiet, med kurser tilknyttet afholdelsen af [de danske mesterskaber i cybersikkerhed](https://www.cybermesterskaberne.dk/online-traening/). Igennem disse kurser har jeg fået et par ugers forspring og deraf tidligt prøvet kræfter af med redskaber som **Hydra** og **metasploit**. Vi benyttet en CTF-platform ved nawn Haaukins til at prøve kræfter af med forskellige XSS-angreb, packet sniffing samt exploits som Heartbleed og Samba.

<b>Fritid</b><br/>
I min fritid har jeg prøvet kræfter af med flere elementer af Aircrack-ng suiten, (airmon-ng, airodump-ng etc.) til at lave et evil twin angreb på min egen router. Jeg har yderligere undersøgt hvordan photoshop kombineret med moderne AI-teknologier kan skjule billeddata således forensics-redskaber som [Forensically](https://29a.ch/photo-forensics/) ikke kan vurdere hvorvidt billedet er ændret.

Til sidst har jeg samlet en kort liste af et par [ekstra kommandoer](https://github.com/MBRzealand/IT-sikkerhed/blob/main/Linux%20%C3%98velser/ekstra_linux_kommandoer.md)
 brugt undervejs i forløbet som ikke helt har været pensum. 

 
