## Øvelse 1:
Select a directory and run a long listing on it. Note the permissions on the 
files and directories.

#### Besvarelse:
   
```shell
cd Desktop/hackerdirectory
ls -l hackedfile
```

![image](https://user-images.githubusercontent.com/70659124/217213123-c780956d-1933-4a27-ac40-0d533b64eebd.png)

## Øvelse 2:
Select a file you don’t have permission to execute and give yourself execute 
permissions using the chmod command. Try using both the numeral method 
(777) and the UGO method.

#### Besvarelse:

##### (777)
"100" giver udelukkende brugeren execute rights
```shell
chmod 000 hackedfile
chmod 100 hackedfile
```

tallene repræsenterer rettigheder for forskellige grupper  
(```7```77) - repræsenterer brugeren  
(7```7```7) - repræsenterer grupper  
(77```7```) - repræsenterer andre

0 - No permission
1 - Execute
2 - Write
3 - Execute + write
4 - Read
5 - Read + execute
6 - Read + write
7 - Read + write + execute


   
##### UGO
"u+x" giver udelukkende brugeren execute rights
```shell
chmod 000 hackedfile
chmod u+x hackedfile
```

brugere:  
U - user  
G - group  
O - others

rettigheder:  
r - read  
w - write  
x - execute

## Øvelse 3:
Choose another file and change its ownership using chown.

#### Besvarelse:
For at vise ændring af ejerskab oprettes en ny bruger:
   
```shell
sudo useradd Mikkel
```
Dernæst kan en fil oprettes og ændres:

```shell
mkdir tmp_folder
cd tmp_folder
touch tmp_file
```
![image](https://user-images.githubusercontent.com/70659124/218725320-1eca7317-c3e3-4d57-bdb9-c547796db818.png)

Fil-ejeren ændres:
```shell
sudo chown Mikkel tmp_file
```
![image](https://user-images.githubusercontent.com/70659124/218722772-05ee2fbb-967d-442b-8bc4-894a4a9bec6e.png)


## Øvelse 4:
Use the find command to find all files with the SGID bit set.

#### Besvarelse:
   
```shell
sudo find / -perm /2000 
```
![image](https://user-images.githubusercontent.com/70659124/218730493-5144327b-8ab2-4730-a962-c4a13809287a.png)

