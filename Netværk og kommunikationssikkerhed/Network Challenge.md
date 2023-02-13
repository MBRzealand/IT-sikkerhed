# Network Challenge
First download the file cap.pcapng from fronter.
A host (lets call it Thor) is connections to demo.testfire.net. Try to investigate the traffic.
Also note down the packet numbers where you found the answers.

## Øvelse 1:  
What is the IP address of demo.testfire.net, and what is Thors IP address?

#### Besvarelse:
The ip of demo.testfire.net can be found the following way:  
Statistics > Resolved addresses > search for "demo"  

the IP of demo.testfire.net is: ```65.61.137.117```  

Thors IP address is: ```192.168.1.125``` (the website he visits sends a login suggestion in frame 1587)


## Øvelse 2:  
In what package(s) did we get the DNS response, and what happened?

#### Besvarelse:
if we filter by: ```dns contains "demo"``` we get all dns related activity to "demo.testfire.net"
we see the first response failed, and the second is a retransmission of the first, the remaining 3 got regular responses
![image](https://user-images.githubusercontent.com/70659124/218411550-d1362e89-462e-463d-8339-1833b9274a4a.png)


## Øvelse 3: banking?
What kind of service(s) did Thor access on demo.testfire.net?

#### Besvarelse:
Thor accessed banking services, however if we download the html page, we can see the following text:

The Altoro Mutual website is published by Watchfire, Inc. for the sole purpose of demonstrating the effectiveness of Watchfire products in detecting web application vulnerabilities and website defects. This site is not a real banking site. Similarities, if any, to third party products and/or websites are purely coincidental. This site is provided "as is" without warranty of any kind, either express or implied. Watchfire does not assume any risk in relation to your use of this website. For additional Terms of Use, please go to http://www.watchfire.com/statements/terms.aspx.

This technically means that the website is just a demonstrational website, and not a real banking website

## Øvelse 4:  
HTTP traffic was observed. Tell what elements the first page accessed contained?

#### Besvarelse:
ekstrabladet?


## Øvelse 5:  
How did the user land on demo.testfire.net? Any indications on what directed him there?

#### Besvarelse:
Statistics > HTTP > Request sequences:
we can see demo.testfire.net is nested under Google, meaning the user went there through Google.

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
10 packets in total

Statistics > HTTP > packet counter > filter by ip (```ip.addr == 65.61.137.117```):

![image](https://user-images.githubusercontent.com/70659124/218336265-0e6a8e99-7d5e-408b-ad93-13a1da9a04cc.png)


## Øvelse 9:  
What is going on in packet 1694, and to what is that packet replying?

#### Besvarelse:
The packet cant find the favicon:
follow > http stream > scroll ned og se response header


## Øvelse 10:  
TCP connection with demo.testfire.net torn down? If yes then where, and if no then why not?

#### Besvarelse:
# ?

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
Go to statistics > IPv4 statistics > all addresses
