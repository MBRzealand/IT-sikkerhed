## Opgavebeskrivelse
Aflever et dokument, hvor du beskriver, hvordan du har anvendt Shodan til ovenstående opgaver (gerne med links og eksempler.) 

Du skal bruge ca. 2 timer på opgaven (plus minus en time.)

## Øvelse 1:
[Få en academic upgrade](https://help.shodan.io/the-basics/academic-upgrade) med din Zealand mail 

#### Besvarelse:
![image](https://user-images.githubusercontent.com/70659124/221358892-95be34ba-ec29-440f-bb71-646659bced43.png)


## Øvelse 2:
Se forskellige muligheder for søgninger med Shodan under [Examples](https://www.shodan.io/search/examples)

#### Besvarelse:
Efter at have afprøvet de forskellige eksempler kan det ses at selv med et Academic upgrade er eksemplet;  
"Industrial control systems running an industrial protocol (i.e. no web servers)" begrænset til enterprice brugere da det indeholder ```ICS``` tagget.  
<br/>
![image](https://user-images.githubusercontent.com/70659124/221359250-80200dfb-8d43-4444-9949-0100115c7764.png)  
<br/>
```ICS``` tagget holder øje med udsatte "industrial control systems", dette betyder altså devices som i colonial pipeline eller stuxnet angrebene.  
Det virker til vi har adgang til de resterende eksempler, interesante søgemuligheder vil gennemgås i næste spørgsmål.

*bemærk: vi har heller ikke adgang til* ```honeypot``` *tagget*

## Øvelse 3:
Undersøg, hvilke søgemuligheder der er i Shodan under [Filtre](https://www.shodan.io/search/filters)

#### Besvarelse:
Der er en stor række filtre, jeg vil derfor liste et par der ved første øjekast virker spændende.

**Til at finde sårbarheder i specifikke områder:**
<ul>
  <li>city - Søgning efter specifikke byer</li>
  <li>country - Søgning efter specifikke lande</li>
  <li>postal - Søgning efter postaddresse</li>
</ul>

**Til at finde sårbarheder i specifikke virksomheder:**
<ul>
  <li>org - Søgning efter devices ejet af specifikke virksomheder</li>
  <li>product - Hvis man eksempelvis vil finde devices der anvender services udviklet af Google</li>
</ul>

**Til reconnaissance:**

<ul>
  <li>http.component - fortæller hvilken teknologi hjemmesider er udviklet med</li>
  <li>has_screenshot - viser billeder fra devices, kamera feeds kan potentielt anvendes til phishing: <a href="https://user-images.githubusercontent.com/70659124/221361668-611a672a-2dd1-4a89-8675-67a3c8c9376b.png">eksempel på navn og udseende af person</a></li>
  <li>ip - hvis man eksempelvis har adgang til et specifikt netværk kan sårbare devices kørende på netværket findes ved en ip søgning</li>
</ul>

**Kan misbruges:**
<ul>
  <li>server - eksempelvis kan man finde alle netgear servere og anvende at de har default username: admin og default password: password</li>
  <li>has_vuln - kan kombineres med andre søgninger til at finde sårbare devices</li>
  <li>vuln - kan finde devices sårbare over for specifikke typer angreb</li>
  <li></li>
</ul>


**Lidt vilde queries:**
<ul>
  <li>title:"Slocum Fleet Mission Control" - Ubåds kontrol paneler <a href="https://user-images.githubusercontent.com/70659124/221364257-be699bcb-6852-4f03-8b1f-52126027ca95.png">Eksempel</a></li>
  <li>"voter system serial" country:US - Valgautomater i amerika <a href="https://user-images.githubusercontent.com/70659124/221364387-2e4c0657-59cb-406d-bc12-448590bc4c52.png">Eksempel</a></li>
  <li>http.title:"Nordex Control" "Windows 2000 5.0 x86" "Jetty/3.1 (JSP 1.1; Servlet 2.2; java 1.6.0_14)": Vindmølle farms <a href="https://user-images.githubusercontent.com/70659124/221364302-af2e3bb2-f04b-4859-b051-c4cd42585a51.png">Eksempel</a></li>
  <li>"Chromecast:" port:8008 - Chromecasts/smartTV's <a href="https://user-images.githubusercontent.com/70659124/221364670-2b47971b-51a2-406c-a852-551e2e6d61cd.png">Eksempel</a></li>
</ul>




## Øvelse 4:

#### Besvarelse:


## Øvelse 5:

#### Besvarelse:


## Øvelse 6:

#### Besvarelse:
