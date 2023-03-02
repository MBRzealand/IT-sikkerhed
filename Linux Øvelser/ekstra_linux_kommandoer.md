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
sudo tcpdump -i eth0 host kallas.dk
sudo tcpdump tcp port 80 and host kallas.dk
sudo tcpdump tcp port 80 and dst host kallas.dk
```
