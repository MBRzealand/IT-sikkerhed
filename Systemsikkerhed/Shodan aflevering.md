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
</ul>


**Lidt vilde queries:**
<ul>
  <li>title:"Slocum Fleet Mission Control" - Ubåds kontrol paneler <a href="https://user-images.githubusercontent.com/70659124/221364257-be699bcb-6852-4f03-8b1f-52126027ca95.png">Eksempel</a></li>
  <li>"voter system serial" country:US - Valgautomater i amerika <a href="https://user-images.githubusercontent.com/70659124/221364387-2e4c0657-59cb-406d-bc12-448590bc4c52.png">Eksempel</a></li>
  <li>http.title:"Nordex Control" "Windows 2000 5.0 x86" "Jetty/3.1 (JSP 1.1; Servlet 2.2; java 1.6.0_14)": Vindmølle farms <a href="https://user-images.githubusercontent.com/70659124/221364302-af2e3bb2-f04b-4859-b051-c4cd42585a51.png">Eksempel</a></li>
  <li>"Chromecast:" port:8008 - Chromecasts/smartTV's <a href="https://user-images.githubusercontent.com/70659124/221364670-2b47971b-51a2-406c-a852-551e2e6d61cd.png">Eksempel</a></li>
</ul>




## Øvelse 4:
[Find sårbarheder](https://exposure.shodan.io/#/) i et udvalgt land

#### Besvarelse:
Det ligger naturligtvis lige til højrebenet at vælge Danmark, for at gøre det lidt interresant vælger vi i stedet Sverige.

query: ```country:se has_vuln:true```


eksempel:  
![image](https://user-images.githubusercontent.com/70659124/221367559-a858871c-0259-42cf-9dad-3c3634fdec70.png)

liste af devicets sårbarheder (Alle sårbarheder er PHP relaterede):
<ul>
  <li>CVE-2018-19396</li>
  <li>CVE-2018-19395</li>
  <li>CVE-2022-31628</li>
  <li>CVE-2022-31629</li>
  <li>CVE-2019-9641</li>
  <li>CVE-2017-7963</li>
  <li>CVE-2017-7272</li>
  <li>CVE-2019-9639</li>
  <li>CVE-2019-9638</li>
  <li>CVE-2015-9253</li>
  <li>CVE-2019-9637</li>
</ul>


## Øvelse 5:
Find forskellige enheder i nærheden af dit bopæl ([fx has_screenshot:true](https://maps.shodan.io/#55.845069296840485/11.040662303566934/8/satellite/has_screenshot:true))

#### Besvarelse:

query: ```city:Albertslund has_screenshot:true```

Eksempel:
![image](https://user-images.githubusercontent.com/70659124/221424999-72e18ba4-0a26-44af-9f16-57bc21558d40.png)



## Øvelse 6:
[Sæt op en overvågning](https://monitor.shodan.io/dashboard?language=en) på nogle ip-numre (fx dit eget ip-nummer eller Zealands ip-numre)

#### Besvarelse:
Jeg opsætter en overvågning på min egen IP da jeg ikke kan finde Zealands hjemmefra:
![image](https://user-images.githubusercontent.com/70659124/221428928-ac29eff5-3125-48f8-a8f2-11bb82599261.png)

![image](https://user-images.githubusercontent.com/70659124/221429054-fe3d2302-a5fa-48f2-9f03-740e46850b6e.png)


Dette bliver en lidt kedelig overvågning da en søgning på min ip, ikke giver nogle resultater:
![image](https://user-images.githubusercontent.com/70659124/221429014-11292bf3-300d-4910-b114-897b9b865c58.png)



## Øvelse 7:
Konstruer en søgning, der viser sårbare maskiner i Danmark, og gennemgå nogle af sårbarheder. 

#### Besvarelse:
Først kan vi søge efter sikkerhedsbrud i hele Danmark:

query: ```country:dk has_vuln:true```

130.226.237.173 (DTU) - [Sårbarheder](https://user-images.githubusercontent.com/70659124/221425604-a87b4e87-9a3a-4bc2-bc96-f93ecd94ab12.png)  
217.157.159.181 (Telenor) - [Sårbarheder](https://user-images.githubusercontent.com/70659124/221425757-c293b7b7-1713-4e73-be1f-fb7575eb01f5.png) (FREAK, Logjam)  
217.157.159.181 (Telia Stofa A/S) - [Sårbarheder](https://user-images.githubusercontent.com/70659124/221426196-c28bb2c0-3953-4421-bc3f-a5cab2732164.png) (FREAK, Logjam)  
217.157.159.181 (Kartago Capital A/S) - [Sårbarheder](https://user-images.githubusercontent.com/70659124/221426241-ae990345-7d8d-4819-9f96-6a27a526cb54.png) (CVE-2022-32548 - unauthorized remote code execution)  
193.162.253.150 - (SU Styrelsen) - [Sårbarheder](https://user-images.githubusercontent.com/70659124/221428502-49806c80-2668-49fb-9922-8eb171f527fd.png) (MANGE!)


Jeg skal til jobsamtale hos den danske virksomhed Tryg Forsikring, så passende kan vi lave en søgning på dem:

query: ```org:Tryg has_vuln:true```

![image](https://user-images.githubusercontent.com/70659124/221428582-924893d7-a905-429f-965d-f3608b76d822.png)

begge servere har følgende sårbarhed:
![image](https://user-images.githubusercontent.com/70659124/221428612-c4c65f8f-384b-44af-87b1-454c3b2cb2da.png)





## Anvendt Arbejdstid:
![image](https://user-images.githubusercontent.com/70659124/221368519-46c3cfeb-750f-4206-be02-1c2969da9478.png)

