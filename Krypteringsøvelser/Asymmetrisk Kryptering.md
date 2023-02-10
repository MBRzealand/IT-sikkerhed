## Øvelse 1:
Lav en ```md5``` hashværdi af en besked i Cyberchef. Send besked og hashværdi til makker. Makker skal afgøre, om beskeden passer til hashværdien eller ej. 

#### Besvarelse:
Besked: ```Hej min ven```  
Hash: ```c8b7f1dd84b5f3f7af2a5ed41868e777```

## Øvelse 2:
Find en indbygget kommando til dit operativsystem, som kan lave md5 hash af en fil. Lav en tekstfil, og lav en hashværdi af filen. Udveksl filen og hashvværdien med makker, som skal afgøre ægtheden af filen. 

#### Besvarelse:
   
```powershell
 Get-FileHash "C:\Users\mikma\OneDrive\Dokumenter\hej_lukas.txt" -Algorithm MD5
```
Hash: ```06001A2EBE34C730FA5040DAAB6D60B9```

## Øvelse 3:
Find et eksempel på et dårligt password, minimum 6 tegn. Lav en md5 hash af passwordet. Kan du cracke hashen på crackstation.net?  

#### Besvarelse:

Password: ```coolpassword```  
Hash: ```995ddff75421a80c6b932292422ab336```

![Imgur](https://i.imgur.com/Z7MQ0O2.png)


## Øvelse 4:
Tilføj en 20 tegn lang saltværdi, og hash igen. Kan det stadig crackes?

#### Besvarelse:

Først genereres salt:
```shell
 node
 const crypto = require('crypto')
 crypto.randombytes(10).toString('hex')
```
Output: ```6a1b75657a5da7b81bb9```  
Password: ```coolpassword6a1b75657a5da7b81bb9```  
Hash: ```f86f143bc315a53b5fcb85226eff42ac```  

![Imgur](https://i.imgur.com/fxupWFG.png)


## Øvelse 5:
Lav øvelsen 1, 3 og 4 med mere sikre hashingalgoritmer som fx sha256, sha384, sha512. 

### sha256:
#### Øvelse 1
Besked: ```Hej min ven```  
Hash: ```0725d47a6b0ebc1cc7a19da041410c81eaa3e0fcfb593a77536cd585e17078ff```

#### Øvelse 3
Password: ```coolpassword```  
Hash: ```fadb68f2a094c1db2f6fa959ec350a9c51507a14ae7f2324c00b082f2493efaa```
![Imgur](https://i.imgur.com/FlrVQlD.png)

#### Øvelse 4
Password: ```coolpasswordf41ab1d71dd09481dfac```  
Hash: ```b8bc569f82e50400f4e7c63e8e77c576bec2df54c53c1372d94a7e0602f73580```
![Imgur](https://i.imgur.com/EALvWwm.png)

### sha384:
#### Øvelse 1
Besked: ```Hej min ven```  
Hash: ```bd98167d2aa8698cd497183509c85e7d467be7c6d995e0e81d5a53b1045a86e53b2636c3f6ba1b8bfac64402c3d8b882```

#### Øvelse 3
Password: ```coolpassword```  
Hash: ```f7ef328fbb90f1246fc9474c05746c3c95378cba696dac2a94d37a042e2c90cc000118c76ffd7fef9958bd564ee22519```
![Imgur](https://i.imgur.com/xtrR00r.png)

#### Øvelse 4
Password: ```coolpassword3cd0d56c41b2945667ae```  
Hash: ```b9d65d111e2c4a835fc811738db362cec020418f41d591d3339d24a149b7ecf1e1e0734474bf42a15a740c32c02ccdf9```
![Imgur](https://i.imgur.com/e9QbFo1.png)

### sha512
#### Øvelse 1
Besked: ```Hej min ven```  
Hash: ```d368120cef691dc3f5e969af4e11acc0ef7740be7c4f12717202d02e2564ad7e92fd8dbd64f77c46516237998527c4fe69fb0d00af2ed6cfccd2c7e6d54abcac```

#### Øvelse 3
Password: ```coolpassword```  
Hash: ```d2e82b13c169642338ca2150fac2489d453b5cd32e910737d063a9f49b29a3b8a5577cb5e2b358c760f845ef0bfafd427f36f84298fea37bad7203ba0489774a```
![Imgur](https://i.imgur.com/ZSrDD3A.png)

#### Øvelse 4
Password: ```coolpasswordbd24341eb0925de1c654```  
Hash: ```139352166a84fe2809837b2d72b8a82c0101f336b983d48622bd17dbc3280ee7a8cb3cfe3aba34e445b62b01788d9db5407a6ff5c37685b242c0ae2f3033339f```
![Imgur](https://i.imgur.com/8HpzIad.png)


## Øvelse 6:
Prøv også bcrypt (bruges til passwords) og sha3 i Cyberchef.

#### Besvarelse:
   
```shell
 
```
