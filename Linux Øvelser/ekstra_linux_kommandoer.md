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
