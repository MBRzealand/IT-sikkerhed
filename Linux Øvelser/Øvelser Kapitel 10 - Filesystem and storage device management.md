## Øvelse 1:
Use the ```mount``` and ```umount``` commands to mount and unmount your flash
drive.


#### Besvarelse:

Først skal vi have navnet på USB-drevet:

```shell
sudo fdisk -l
```
![image](https://user-images.githubusercontent.com/70659124/222897226-ad6adf3f-66d1-4920-bef7-f3e21b2cf83b.png)

Dernæst kan vi lave et mounting point:
```shell
sudo mkdir /media/usb-drive
sudo mount /dev/sdc1 /media/usb-drive/
cd /media/usb-drive/
ls
```
![image](https://user-images.githubusercontent.com/70659124/222898597-dc32016d-a85b-4347-8626-7d2ae7f37f60.png)

Vi prøver unmount:

```shell
sudo umount /media/usb-drive
```
![image](https://user-images.githubusercontent.com/70659124/222899127-67a38dd6-d9ac-4250-b68b-903163dbb923.png)




## Øvelse 2:
Check the amount of disk space free on your primary hard drive.

#### Besvarelse:
   
```shell
sudo fdisk -l
```

![image](https://user-images.githubusercontent.com/70659124/222900459-66dd01fb-975c-4ab2-8196-0bea3220cb3a.png)

alternativt kan ```df``` beyttes:  
![image](https://user-images.githubusercontent.com/70659124/222902111-6f5862bd-4a1a-45d1-91b0-fdd92b4625f9.png)
  

## Øvelse 3:
Check for errors on your flash drive with ```fsck```.

#### Besvarelse:
```shell
fsck
```

Hele vores system er et mounted virtuelt drev, vi kan derfor ikke benytte fsck som set i fejlen:  
![image](https://user-images.githubusercontent.com/70659124/222902967-731eb129-95a0-4170-a34c-77fdf446c62c.png)


## Øvelse 4:
Use the ``dd`` command to copy the entire contents of one flash drive to
another, including deleted files.

#### Besvarelse:
```shell
sudo dd if=/dev/sdb1 of=~/Desktop/copiedUSB 
```
![image](https://user-images.githubusercontent.com/70659124/222906930-8500c502-0b0c-491f-ab32-f23c542c13b9.png)


## Øvelse 5:
Use the ```lsblk``` command to determine basic characteristics of your block
devices.

#### Besvarelse:
   
```shell
lsblk
```

![image](https://user-images.githubusercontent.com/70659124/222907003-8a91e2ad-3ab9-40a1-8b90-2ccae2d6111d.png)
