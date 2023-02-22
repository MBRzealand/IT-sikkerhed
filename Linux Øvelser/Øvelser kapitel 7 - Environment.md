## Øvelse 1:
View all of your environment variables with the more command

#### Besvarelse:
   
```shell
set | more
```
![image](https://user-images.githubusercontent.com/70659124/220564156-b6960a65-ce39-42be-8c34-c35cf310529a.png)



## Øvelse 2:
Use the echo command to view the ```HOSTNAME``` variable.

#### Besvarelse:
   
```shell
set | $HOSTNAME
```
![image](https://user-images.githubusercontent.com/70659124/220565168-2b353ff8-22a0-400a-902f-790d29c680f8.png)


## Øvelse 3
Find a method to change the slash (/) to a backslash (\) in the faux
Microsoft ```cmd PS1``` example (see Listing 7-2).

#### Besvarelse:
   
```shell
export PS1="\[\e[01;32m\]C\072\w \[\e[0m\]> "
```
![image](https://user-images.githubusercontent.com/70659124/220577301-7ec48b45-8056-4dec-90da-f4e54cf59598.png)


## Øvelse 4:
Create a variable named ```MYNEWVARIABLE``` and put your name in it.

#### Besvarelse:
   
```shell
MYNEWVARIABLE="Mikkel Boye Rasmussen"
```

## Øvelse 5:
Use echo to view the contents of ```MYNEWVARIABLE```.

#### Besvarelse:
   
```shell
echo $MYNEWVARIABLE
```
![image](https://user-images.githubusercontent.com/70659124/220567800-7f48e296-eaa0-4fff-b25a-d2c7d7089423.png)


## Øvelse 6:
Export ```MYNEWVARIABLE``` so that it’s available in all environments.

#### Besvarelse:
   
```shell
export MYNEWVARIABLE
```
![image](https://user-images.githubusercontent.com/70659124/220570140-20d67575-e115-4051-ba38-0bbbe3c6850c.png)



## Øvelse 7:
Use the echo command to view the contents of the ```PATH``` variable

#### Besvarelse:
   
```shell
echo $PATH
```
![image](https://user-images.githubusercontent.com/70659124/220570905-c3041a98-3173-4770-b761-1a89e1e12688.png)



## Øvelse 8:
Add your home directory to the ```PATH``` variable so that any binaries in your
home directory can be used in any directory.


#### Besvarelse:
   
```shell
PATH+=:~
echo $PATH
```
![image](https://user-images.githubusercontent.com/70659124/220571953-3040de80-4f9d-44e3-a6de-1097898377a8.png)


## Øvelse 9:
Change your ```PS1``` variable to "World's Greatest Hacker:".

#### Besvarelse:
   
```shell
PS1="World's Greatest Hacker:"
```
![image](https://user-images.githubusercontent.com/70659124/220574180-d828e709-1d40-4c5a-b402-c585e8ad088c.png)
