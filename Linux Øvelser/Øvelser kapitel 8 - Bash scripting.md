## Øvelse 1:
Create your own greeting script similar to our HelloHackersArise script

#### Besvarelse:
   
```shell
touch MyFirstBashScript
echo '#! /bin/bash' >> MyFirstBashScript
echo 'echo "Ungabunga welcome script"' >> MyFirstBashScript

chmod 755 MyFirstBashScript

./MyFirstBashScript
```
![image](https://user-images.githubusercontent.com/70659124/221920265-87abcff6-d996-44af-aba4-dc844ed08b28.png)


## Øvelse 2:
Create a script similar to *MySQLscanner.sh* but design it to find systems with
Microsoft’s SQL Server database at port 1433. Call it *MSSQLscanner*.

#### Besvarelse:
   
```shell
touch MySQLscanner.sh
echo '#! /bin/bash' >> MySQLscanner.sh
echo 'echo "What is your name?"' 

```

## Øvelse 3:
Alter that *MSSQLscanner* script to prompt the user for a starting and end-
ing IP address and the port to search for. Then filter out all the IP addresses
where those ports are closed and display only those that are open.

#### Besvarelse:
   
```shell
```
