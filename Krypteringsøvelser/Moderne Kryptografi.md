## Redskaber
[Cyberchef](https://gchq.github.io/CyberChef/)  

## Øvelse 1
Afprøv algoritmerne DES, 3DES, AES og RSA i Cyberchef ved at kryptere en besked og sende kryptoteksten til makkeren, som skal dekryptere.

#### DES:
Besked: ```Moderne kryptering er cool!```  
Krypteret besked: ```25e851d97992effef835f144e832c51123c10c94766b3bc8f042d251eac4f288```  
Key: ```Password```  
IV: ```IVIVIVIV```  
Link: https://gchq.github.io/CyberChef/#recipe=DES_Encrypt(%7B'option':'UTF8','string':'Password'%7D,%7B'option':'UTF8','string':'IVIVIVIV'%7D,'CBC','Raw','Hex')&input=TW9kZXJuZSBrcnlwdGVyaW5nIGVyIGNvb2wh

#### 3DES:
Besked: ```3DES er 3 gange så nice!```  
Krypteret besked: ```84ab6ee83f697cdf459bec5cf33391fb1e5e435801bdf4e5```  
Key: ```ThisIsMySuperRadPassword```  
IV: ```IVIVIVIV```  
Link: https://gchq.github.io/CyberChef/#recipe=Triple_DES_Encrypt(%7B'option':'UTF8','string':'ThisIsMySuperRadPassword'%7D,%7B'option':'UTF8','string':'IVIVIVIV'%7D,'CBC','Raw','Hex')&input=M0RFUyBlciAzIGdhbmdlIHPlIG5pY2Uh

#### AES:
Besked: ```AES må stå for Awesome Encryption Standard```  
Krypteret besked: ```146ab746948f8c6b0fd1a2f3445a286fa6afae4b2111a9ec439f8c6aa76c210722a1a4aafa067b4027784d3e713b11e9```  
Key: ```ThisIsMyCoolKey!```  
IV: ```IVIVIVIVIVIVIVIV```  
Link: https://gchq.github.io/CyberChef/#recipe=AES_Encrypt(%7B'option':'UTF8','string':'ThisIsMyCoolKey!'%7D,%7B'option':'UTF8','string':'IVIVIVIVIVIVIVIV'%7D,'CBC','Raw','Hex',%7B'option':'Hex','string':''%7D)&input=QUVTIG3lIHN05SBmb3IgQXdlc29tZSBFbmNyeXB0aW9uIFN0YW5kYXJk


#### RSA:
Besked: ```RSA står for Really Secure Algorithm, right?```   
Krypteret besked: ```.x.e§.ô¢ú>q.6.ä7ùL>±±ZY¢GPX~#º..ÿ{óÃRbÔ~.g7.ù]5Æ:.§¥Úÿ.yÐ.ÞfT¿.ÃõÓ&UbÎLxEP...¹ê¦ÐD.§.I:.ÕÌý.Ðë.Ça`µ9vj.ÛW°'¬q.·ÖeuÆAåÐ8w³."b.º(û```

Public Key: 
```
-----BEGIN PUBLIC KEY-----
MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQCwkPJlRXd3bYaGzm/+XoDvSF/A
PkdzrSjcDedNpvS5BRKF+MC6B6SPahua/UrYNwnRnu+S2rWnIkpFz3S93XNiYFGK
37nqrXJvxFPzmf//1kBCXqo1m35FQRzp+OIUEaUL1Pz4Rss5/nEcfDYg+t35Ushz
HshqjqG36lepPYljZQIDAQAB
-----END PUBLIC KEY-----
```

Private Key: 
```
-----BEGIN RSA PRIVATE KEY-----
MIICXQIBAAKBgQCwkPJlRXd3bYaGzm/+XoDvSF/APkdzrSjcDedNpvS5BRKF+MC6
B6SPahua/UrYNwnRnu+S2rWnIkpFz3S93XNiYFGK37nqrXJvxFPzmf//1kBCXqo1
m35FQRzp+OIUEaUL1Pz4Rss5/nEcfDYg+t35UshzHshqjqG36lepPYljZQIDAQAB
AoGAGJUBjlxqys+Omm+c04UMPeQtYoo5L+90gBiWcq7zJNxCLTFKAcxlGotrDvvD
QxF8ljjiwWceQcfqH8iHiBSQBu+zizPTEZv8ngQCL8Q5qz+3bFc0BkItX2g6NrEt
86//xKnJPsSEpjK7riHGTR4nnGxGkC5G98eke/BjQfNONGECQQDh4FIzEn9yx1wR
/RrVcy7KtbtzXPqr8DSGkraFovUWMigzi6QexceoWFXlYPhtNLG/Cb+vW3rkld9Y
XLUpUb+FAkEAyB0feASs7ioK0e7RPKZ5vA67AOxn/y+jBckdQMSOrAGgCFSlVtRy
It4wdPg4Ac3gvnghq0f7vyp2BCj/6tQqYQJActzvEBe1BfpJYMB0V91WCzF1XIoI
00y4eUK8XKLsvVfOR8AYOqnbCUm6jIXOb0JfrUVY2+TKTtnEFRw36AYxPQJBAJ4N
cndmqfcJubYJu7T9f5SqxcR688C3rTi6maI4HL96IR2zTUuBTAyCFR+tlP7HzsRh
OaaAmjNopAGxKEAfBsECQQDFulPHCKoMAoe1ClyohULGS84bnSTgFi9Ol8ezkIJZ
99rGIfHlUSAYYcc7Vtz2slzQ5HXb4uoYq4DGnPrmduP5
-----END RSA PRIVATE KEY-----
```

Link: https://gchq.github.io/CyberChef/#recipe=Generate_RSA_Key_Pair('1024','PEM'/disabled)RSA_Encrypt('-----BEGIN%20PUBLIC%20KEY-----%5CnMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQCwkPJlRXd3bYaGzm/%2BXoDvSF/A%5CnPkdzrSjcDedNpvS5BRKF%2BMC6B6SPahua/UrYNwnRnu%2BS2rWnIkpFz3S93XNiYFGK%5Cn37nqrXJvxFPzmf//1kBCXqo1m35FQRzp%2BOIUEaUL1Pz4Rss5/nEcfDYg%2Bt35Ushz%5CnHshqjqG36lepPYljZQIDAQAB%5Cn-----END%20PUBLIC%20KEY-----','RSA-OAEP','SHA-1')RSA_Decrypt('-----BEGIN%20RSA%20PRIVATE%20KEY-----%5CnMIICXQIBAAKBgQCwkPJlRXd3bYaGzm/%2BXoDvSF/APkdzrSjcDedNpvS5BRKF%2BMC6%5CnB6SPahua/UrYNwnRnu%2BS2rWnIkpFz3S93XNiYFGK37nqrXJvxFPzmf//1kBCXqo1%5Cnm35FQRzp%2BOIUEaUL1Pz4Rss5/nEcfDYg%2Bt35UshzHshqjqG36lepPYljZQIDAQAB%5CnAoGAGJUBjlxqys%2BOmm%2Bc04UMPeQtYoo5L%2B90gBiWcq7zJNxCLTFKAcxlGotrDvvD%5CnQxF8ljjiwWceQcfqH8iHiBSQBu%2BzizPTEZv8ngQCL8Q5qz%2B3bFc0BkItX2g6NrEt%5Cn86//xKnJPsSEpjK7riHGTR4nnGxGkC5G98eke/BjQfNONGECQQDh4FIzEn9yx1wR%5Cn/RrVcy7KtbtzXPqr8DSGkraFovUWMigzi6QexceoWFXlYPhtNLG/Cb%2BvW3rkld9Y%5CnXLUpUb%2BFAkEAyB0feASs7ioK0e7RPKZ5vA67AOxn/y%2BjBckdQMSOrAGgCFSlVtRy%5CnIt4wdPg4Ac3gvnghq0f7vyp2BCj/6tQqYQJActzvEBe1BfpJYMB0V91WCzF1XIoI%5Cn00y4eUK8XKLsvVfOR8AYOqnbCUm6jIXOb0JfrUVY2%2BTKTtnEFRw36AYxPQJBAJ4N%5CncndmqfcJubYJu7T9f5SqxcR688C3rTi6maI4HL96IR2zTUuBTAyCFR%2BtlP7HzsRh%5CnOaaAmjNopAGxKEAfBsECQQDFulPHCKoMAoe1ClyohULGS84bnSTgFi9Ol8ezkIJZ%5Cn99rGIfHlUSAYYcc7Vtz2slzQ5HXb4uoYq4DGnPrmduP5%5Cn-----END%20RSA%20PRIVATE%20KEY-----','','RSA-OAEP','SHA-1')&input=UlNBIHN05XIgZm9yIFJlYWxseSBTZWN1cmUgQWxnb3JpdGhtLCByaWdodD8
