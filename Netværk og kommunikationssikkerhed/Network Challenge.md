# Network Challenge
First download the file cap.pcapng from fronter.
A host (lets call it Thor) is connections to demo.testfire.net. Try to investigate the traffic.
Also note down the packet numbers where you found the answers.

## Øvelse 1:  
What is the IP address of demo.testfire.net, and what is Thors IP address?

#### Besvarelse:

Thors IP address is: ```192.168.1.125``` (the website he visits sends a login suggestion in frame 1587)

```shell

```

## Øvelse 2:  
In what package(s) did we get the DNS response, and what happened?

#### Besvarelse:

```shell
```

## Øvelse 3:  
What kind of service(s) did Thor access on demo.testfire.net?

#### Besvarelse:

```shell
```

## Øvelse 4:  
HTTP traffic was observed. Tell what elements the first page accessed contained?

#### Besvarelse:

```shell
```

## Øvelse 5:  
How did the user land on demo.testfire.net? Any indications on what directed him there?

#### Besvarelse:

```shell
```

## Øvelse 6:  
A photo called “home1.jpg” is fetched from demo.testfire.net. Try to extract it

#### Besvarelse:
![image](https://user-images.githubusercontent.com/70659124/218327115-87be3f78-1768-4482-927e-24412a58c685.png)

## Øvelse 7:  
Which packet(s) contains the photo?

#### Besvarelse:
Packet ```1631``` is the HTTP get request that contains the image.

## Øvelse 8:  
How many HTTP requests were in total made to demo.testfire.net?

#### Besvarelse:

```shell
```

## Øvelse 9:  
What is going on in packet 1694, and to what is that packet replying?

#### Besvarelse:

```shell
```

## Øvelse 10:  
TCP connection with demo.testfire.net torn down? If yes then where, and if no then why not?

#### Besvarelse:

```shell
```

## Øvelse 11:  
Figure out who is behind the IP address 172.217.19.195 (without using google)

#### Besvarelse:
Go to statistics > resolved addresses > search for the IP

The address for the IP is: ```www.gstatic.com```

## Øvelse 12:  
A machine has the IP address 192.168.1.101. Try to find its hostname

#### Besvarelse:
Først søg efter ip adressen: ```ip.addr == 192.168.1.101```  
Dette giver source device: ```Apple_8d:83:a1```  

Derefter kan vi finde navnet på devicet ved:  
Go to statistics > Endpoints > Ethernet > klik "name resolution" > apply as filter > selected > kig på DHCP requesten efter "host name"

IP adressens hostname er ```DanyKallasiPad``` 

## Øvelse 13:  
Generate a list of all the endpoints (IPv4) seen on the network

#### Besvarelse:

```shell
```
