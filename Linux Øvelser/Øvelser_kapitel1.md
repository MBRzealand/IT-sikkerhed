## Øvelse 1:
Use the ```ls``` command from the root (```/```) directory to explore the directory 
structure of Linux. Move to each of the directories with the ```cd``` command 
and run ```pwd``` to verify where you are in the directory structure.

#### Besvarelse:
   
```shell
cd /  
ls  
cd home  
pwd  
ls  
cd kali  
ls  
pwd  
```

## Øvelse 2:  
Use the ```whoami``` command to verify which user you are logged in as.

#### Besvarelse:

```shell
whoami
```
![image](https://user-images.githubusercontent.com/70659124/216373028-0960f093-470f-4408-a054-132fa5607131.png)


## Øvelse 3:
Use the ```locate``` command to find wordlists that can be used for password 
cracking

#### Besvarelse:

```shell
locate 'wordlist'
cd /usr/share/wordlists
ls
```
![image](https://user-images.githubusercontent.com/70659124/216372815-8cb79a6e-0c86-4c11-84ee-734cf557bd84.png)

## Øvelse 4:
Use the ```cat``` command to create a new file and then append to that file. 
Keep in mind that ```>``` redirects input to a file and ```>>``` appends to a file.

#### Besvarelse:

```shell
cd Desktop
cat > task_4_file.txt
cat task_4_file.txt
cat >> task_4_file.txt
cat task_4_file.txt
```

## Øvelse 5:
Create a new directory called *hackerdirectory* and create a new file in 
that directory named *hackedfile*. Now copy that file to your */root* directory 
and rename it *secretfile*.

#### Besvarelse:

```shell
cd Desktop
mkdir 'hackerdirectory'
cd hackerdirectory
touch 'hackedfile'
cp hackedfile /root/secretfile
sudo cp hackedfile /root/secretfile
```

![image](https://user-images.githubusercontent.com/70659124/216771639-a50f2be3-906f-48bc-9831-30637a66a6a1.png)




