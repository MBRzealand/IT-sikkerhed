## Øvelse 1:
Run the ```ps``` command with the ```aux``` options on your system and note which
process is first and which is last


#### Besvarelse:
   
```shell
ps aux
```
Den første process:  
![image](https://user-images.githubusercontent.com/70659124/221853037-c19193be-db41-4d87-b145-64158de31074.png)
Den sidste process:  
![image](https://user-images.githubusercontent.com/70659124/221853148-8726a429-1e0c-4801-b146-3e8368664cb7.png)




## Øvelse 2:
Run the ```top``` command and note the two processes using the greatest
amount of your resources.

#### Besvarelse:
   
```shell
top
```

Xorg og panel-13-cpugra er de to processer der kræver flest resourcer.  
![image](https://user-images.githubusercontent.com/70659124/221853729-a684b3be-e314-4e89-bc04-8ab3fd67c4f7.png)


## Øvelse 3:
Use the kill command to kill the process that uses the most resources.

#### Besvarelse:
   
```shell
sudo kill -15 33148
```
kommandoen smed mig tilbage til loginskærmen (da den formentligt lukkede en process essentiel for systemet):  
![image](https://user-images.githubusercontent.com/70659124/221854896-8469c39f-0127-499f-a2ed-9373f74bd039.png)


## Øvelse 4:
Use the ```renice``` command to reduce the priority of a running process
to +19.

#### Besvarelse:
   
```shell
renice 19 189120
```
![image](https://user-images.githubusercontent.com/70659124/221865895-f96f5af6-f264-40d6-b2e8-51b4142c9b92.png)


## Øvelse 5:
Create a script called ```myscanning``` (the content is not important) with a text
editor and then schedule it to run next Wednesday at 1 Am .


#### Besvarelse:
   
```shell
touch myscanning
echo "#! /bin/bash" >> myscanning
echo "echo hello" >> myscanning
chmod u+x myscanning


```
