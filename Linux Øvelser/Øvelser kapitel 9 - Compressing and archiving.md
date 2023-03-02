## Øvelse 1:
Create three scripts to combine, similar to what we did in Chapter 8.
Name them *Linux4Hackers1*, *Linux4Hackers2*, and *Linux4Hackers3*.

#### Besvarelse:
   
```shell
touch file1
echo hello > file1
touch file2
echo my > file2
touch file3
echo friend > file3
```

## Øvelse 2:
Create a tarball from these three files. Name the tarball *L4H*. Note how the
size of the sum of the three files changes when they are tarred together.

#### Besvarelse:
   
```shell
tar -cvf L4H file1 file2 file3
ll
```
![image](https://user-images.githubusercontent.com/70659124/222456981-7c1ceecd-dad9-44a7-b3d2-9337ae649c40.png)
![image](https://user-images.githubusercontent.com/70659124/222459192-982294fe-3dff-453e-91ae-764ac7534e1c.png)


## Øvelse 3:
Compress the *L4H* tarball with ```gzip```. Note how the size of the file changes.
Investigate how you can control overwriting existing files. Now uncompress
the *L4H* file.

#### Besvarelse:
   
```shell
gzip L4H
```
![image](https://user-images.githubusercontent.com/70659124/222459593-3160bf63-4ba6-4f13-8c5f-18991d37163e.png)


## Øvelse 4:
Repeat Exercise 3 using both ```bzip2``` and ```compress```

#### Besvarelse:
   
```shell
gunzip
bzip2 L4H
bunzip2 L4H
compress L4H
```

![image](https://user-images.githubusercontent.com/70659124/222460463-ef1b8b74-e6d5-4d81-9519-3e3dd3c6d47e.png)

![image](https://user-images.githubusercontent.com/70659124/222460933-59f2ac2e-e9ef-49d4-a664-6ffded135e1a.png)



## Øvelse 5:
Make a physical, bit-by-bit copy of one of your flash drives using the ```dd```
command.

#### Besvarelse:
   
I dont have a flash drive, however i can copy the compressed file:

```shell
dd if='L4H.Z' of='copy'
```

![image](https://user-images.githubusercontent.com/70659124/222463690-e4f1b925-dbd3-4c73-b6f4-cb69d5960e3c.png)
