## Øvelse 1:
Find information on your active network interfaces.

#### Besvarelse:
```shell
ifconfig
```
![image](https://user-images.githubusercontent.com/70659124/218735748-9923cafe-9b6b-4d00-8fc4-34e7bb2c0161.png)



## Øvelse 2:
Change the IP address on ```eth0``` to 192.168.1.1.

#### Besvarelse:
   
```shell
sudo ifconfig eth0 192.168.1.1
```
![image](https://user-images.githubusercontent.com/70659124/218737224-6f2cbcae-a6a7-4627-ba8f-6d1b011687c5.png)


## Øvelse 3:
Change your hardware address on ```eth0```.

#### Besvarelse:
   
```shell
sudo ifconfig eth0 down
sudo ifconfig eth0 hw ether 04:20:69:69:04:20
sudo ifconfig eth0 up
```
![image](https://user-images.githubusercontent.com/70659124/218740575-8bb5b43f-b54e-43b4-aac2-31478800ff1e.png)


## Øvelse 4:
Check whether you have any available wireless interfaces active.

#### Besvarelse:
   
```shell
iwconfig
```
![image](https://user-images.githubusercontent.com/70659124/218742919-b4da15de-ac1b-478f-9d9b-182aba278f74.png)


## Øvelse 5:
Reset your IP address to a DHCP-assigned address.


#### Besvarelse:
   
```shell
dhclient eth0
```

## Øvelse 6:
Find the nameserver and email server of your favorite website.

#### Besvarelse:
   
```shell
dig mikkel-boye-rasmussen.dk ns
```
![image](https://user-images.githubusercontent.com/70659124/218812230-3388350f-4801-49a8-bf1e-9e6587cdb15e.png)

```shell
dig mikkel-boye-rasmussen.dk mx
```
![image](https://user-images.githubusercontent.com/70659124/218812445-20917884-1d52-4914-bbdf-bd668c4a5e27.png)

## Øvelse 7:
Add Google’s DNS server to your /etc/resolv.conf file so your system
refers to that server when it can’t resolve a domain name query with
your local DNS server.

#### Besvarelse:
   
```shell
sudo chmod 777 /etc/resolv.conf
mousepad /etc/resolv.conf
```
![image](https://user-images.githubusercontent.com/70659124/218814494-d6c68edf-2e65-4a27-ab40-e71656285257.png)



