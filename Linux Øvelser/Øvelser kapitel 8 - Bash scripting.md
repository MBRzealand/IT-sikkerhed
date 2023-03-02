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
touch MSSQLscanner.sh
echo '#! /bin/bash' >> MSSQLscanner.sh
chmod 755 MSSQLscanner.sh

mousepad MSSQLscanner.sh
```
selve scriptet:  
![image](https://user-images.githubusercontent.com/70659124/221950775-5e0c41b6-24db-4df8-b936-d203560a382b.png)


Scan resultatet i filen MSSQLscan:  
![image](https://user-images.githubusercontent.com/70659124/221950081-7b785fc5-57fe-4b1f-9608-775c88ef6c6b.png)

Da resultatet af scannet kun indeholder lukkede porte, vil grep funktionen ikke finde noget med "open" søgningen.  
Deraf vil MSSQL2 filen være tom, og scriptet printer altså intet i konsollen.

## Øvelse 3:
Alter that *MSSQLscanner* script to prompt the user for a starting and end-
ing IP address and the port to search for. Then filter out all the IP addresses
where those ports are closed and display only those that are open.

#### Besvarelse:
   
```shell
touch MySQLscanner.sh
echo '#! /bin/bash' >> MySQLscanner.sh

mousepad MySQLscanner.sh
```
Selve scriptet:  
![image](https://user-images.githubusercontent.com/70659124/222367321-490eab37-23cf-492d-b269-71fe4f921067.png)






