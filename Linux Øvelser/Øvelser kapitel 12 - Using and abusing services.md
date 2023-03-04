## Øvelse 1:
Start your apache2 service through the command line.

#### Besvarelse:
   
```shell
sudo apt install apache2
services apache2 start
```
![image](https://user-images.githubusercontent.com/70659124/222910306-a2d4aced-846a-475c-9db0-d0313ad48097.png)


## Øvelse 2:
Using the *index.html* file, create a simple website announcing your arrival
into the exciting world of hacking.

#### Besvarelse:
   
```shell
chmod 777 /var/www/html/index.html
mousepad /var/www/html/index.html
```
![image](https://user-images.githubusercontent.com/70659124/222913245-9e2d2521-15c4-44bc-96bc-b3c55746687d.png)
![image](https://user-images.githubusercontent.com/70659124/222913307-86eeed76-0d67-4394-a72c-35a888e02072.png)

vi stopper serveren før vi går videre

```shell
service apache2 stop
```

<br/>

# ufærdige øvelser


## Øvelse 3:
Start your SSH service via the command line. Now connect to your Kali
system from another system on your LAN.

#### Besvarelse:
   
```shell
service ssh start

```

## Øvelse 4:
Start your MySQL database service and change the root user password to
*hackers-arise*. Change to the ```mysql``` database.

#### Besvarelse:
   
```shell

```

## Øvelse 5:
Start your PostgreSQL database service. Set it up as described in this
chapter to be used by Metasploit.

#### Besvarelse:
   
```shell

```
