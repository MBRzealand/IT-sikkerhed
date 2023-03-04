# Øvelser fra timen:

## Øvelse SSH:
<ul>
   <li>Besøg min server i Amazon vha kommandoen <i>ssh noobs@18.195.65.114</i><br/>
      <b><i>noobs / M=bg*6GCn<~^t+;4</i></b> </li>
   <li><i>Find flaget på dit skrivebord.</i></li>
   <li><i>Prøv at downloade filen via SCP (<a href="https://gist.github.com/andracs/5918331f2ac38eb2ed552b148a90bc8f">hint</a>)</i></li>
   <li><i>Placer dit eget flag på skrivebordet.</i></li>
   <li><i>Kan du placere en hacked.html fil i <b>/var/www/</b> som du kan tilgå på http://18.195.65.114/hacked.html ? </i></li>
</ul>

```shell
# Bemærk: Jeg var til jobsamtale på dagen, øvelserne er lavet efterfølgende, uden adgang til serveren.
ssh noobs@18.195.65.114
cd ~/Desktop
scp noobs@18.195.65.114:/home/noobs/flag.txt ~/Desktop  # alternativt kan vi anvende "get flag.txt"
touch MikkelsFlag.txt  # alternativt kan vi uploade et lokalt flag til serveren med scp
echo "dette er mikkels flag" > MikkelsFlag.txt # eksempelvis scp ~/Desktop/MikkelsFlag.txt noobs@18.195.65.114:~/Desktop
scp ~/Desktop/hacked.html noobs@18.195.65.114:/var/www/
```

<br/>

# Øvelser fra bogen

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
