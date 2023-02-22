## Øvelse 1:
Navigate to */usr/share/wordlists/metasploit*. This is a directory of multiple 
wordlists that can be used to brute force passwords in various password protected devices using Metasploit, the most popular pentesting and hacking framework.

#### Besvarelse:
   
```shell
cd /usr/share/wordlists/metasploit
```

## Øvelse 2:  
Use the ```cat``` command to view the contents of the file *passwords.lst*.

#### Besvarelse:
Der er ingen fil der hedder *passwords.lst* jeg antager derfor der menes *password.lst*.

```shell
cat password.lst
```
![image](https://user-images.githubusercontent.com/70659124/216774630-7c824161-5215-4d2a-9efd-a7567e137468.png)



## Øvelse 3:
Use the ```more``` command to display the file *passwords.lst*.

#### Besvarelse:

```shell
more password.lst
```
![image](https://user-images.githubusercontent.com/70659124/216774670-c8d14c87-7dbf-4bef-911e-0a27a2cdf75d.png)


## Øvelse 4:
Use the ```less``` command to view the file *passwords.lst*.

#### Besvarelse:

```shell
less password.lst
```
![image](https://user-images.githubusercontent.com/70659124/216774709-6bd3fcae-bbb8-4db9-b093-1d6a36bbceff.png)


## Øvelse 5:
Now use the ```nl``` command to place line numbers on the passwords in 
*passwords.lst*. There should be 88,396 passwords.

#### Besvarelse:

```shell
nl password.lst
```
![image](https://user-images.githubusercontent.com/70659124/216774463-73df93c8-b48f-41de-b18b-341f344c19a0.png)


## Øvelse 6:
Use the ```tail``` command to see the last 20 passwords in *passwords.lst*.

#### Besvarelse:

```shell
tail password.lst
```
![image](https://user-images.githubusercontent.com/70659124/216774743-788baa80-7eea-46c7-a389-40f1aebb8f6e.png)


## Øvelse 7:
Use the ```cat``` command to display *passwords.lst* and pipe it to find all the 
passwords that contain 123.



#### Besvarelse:

```shell
cat password.lst | grep '123'
```
![image](https://user-images.githubusercontent.com/70659124/216774895-bf253500-6220-4469-83f8-1fac5569a114.png)




