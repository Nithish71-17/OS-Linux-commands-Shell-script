# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Sc# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 41 28_5c01dacd](https://github.com/user-attachments/assets/e9778b0f-4a65-4323-99de-b388c96f4f33)
cat < file2
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 41 58_e075d889](https://github.com/user-attachments/assets/06300be1-1718-4551-b551-175f1362624f)
# Comparing Files
cmp file1 file2
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 16 46 45_f6902247](https://github.com/user-attachments/assets/6e6af3bc-e468-42c6-b7d8-f517092df203)
comm file1 file2
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 16 48 49_faabc960](https://github.com/user-attachments/assets/37b5518d-265c-4820-adb4-2710b89a85a8)
diff file1 file2
## OUTPUT


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
cut -c1-3 file11
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 50 07_b4920c50](https://github.com/user-attachments/assets/c0037fdd-09de-4bf8-a29f-ffed6bfdee96)
cut -d "|" -f 1 file22
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 50 48_54dbdb2e](https://github.com/user-attachments/assets/cf62d642-7c35-45dd-a8d3-d2f8f3b7a4cc)
cut -d "|" -f 2 file22
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 51 15_33b013ce](https://github.com/user-attachments/assets/154f8566-b99a-4d9f-b698-f45fec6b8e5a)
cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 53 14_8e3b52d5](https://github.com/user-attachments/assets/a1ab4a00-def7-47e7-82aa-a085e9083c83)
grep hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 53 39_648b1a7c](https://github.com/user-attachments/assets/1af20d18-38d7-4838-9193-687696655431)
grep -v hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 11 50_59bdbb46](https://github.com/user-attachments/assets/1a98d332-2297-4ce0-9477-b8b1bb1fc161)

cat newfile | grep -i "hello"
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 09 45_637135a7](https://github.com/user-attachments/assets/8de8eaef-f65d-464e-b158-93cdcfc51508)

cat newfile | grep -i -c "hello"
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 58 52_2c655907](https://github.com/user-attachments/assets/9016389f-9291-480b-aa22-4821eb7fa847)
grep -R ubuntu /etc
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 00 19_91a34f01](https://github.com/user-attachments/assets/63059349-e8cd-49d3-a77a-0c09576ed29d)
grep -w -n world newfile   
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 00 40_6f98b2af](https://github.com/user-attachments/assets/735a4e61-36f4-4646-82d3-f8786be6de34)
cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 13 58_df8c18a6](https://github.com/user-attachments/assets/c66a00d0-2f31-442e-9491-8a21a9a77dc7)
egrep -w '(H|h)ello' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 15 02_3e7bf289](https://github.com/user-attachments/assets/5d5d23cf-d42a-4842-b14a-b9b57cfe36d7)
egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 15 49_2388e863](https://github.com/user-attachments/assets/947cc3e0-9536-4617-ba81-20c264890054)
egrep '(^hello)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 16 43_2f56d67d](https://github.com/user-attachments/assets/bbbb00ef-1cce-415e-aa16-57511e3acbb5)
egrep '(world$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 17 23_095c213b](https://github.com/user-attachments/assets/bc4d7001-d43d-46a0-b732-d3a35740fd9a)
egrep '(World$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 18 20_17b46e92](https://github.com/user-attachments/assets/053c5673-1c73-479e-b456-2b179b5610e1)
egrep '((W|w)orld$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 18 55_04e8da42](https://github.com/user-attachments/assets/9930ae2e-468c-4437-a4d8-42608951b4d9)
egrep '[1-9]' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 19 49_b89f97c9](https://github.com/user-attachments/assets/e871bdd5-0eeb-4a33-819a-9acde03de19e)
egrep 'Linux.*world' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 20 28_39e185c3](https://github.com/user-attachments/assets/55ceee3c-3f03-4712-89bd-2c89597ffc3a)
egrep 'Linux.*World' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 21 04_2e26dad4](https://github.com/user-attachments/assets/2df181bd-3cb0-47fa-9b37-0c0f5fbf5023)
egrep l{2} newfile
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 22 02_521e0f5d](https://github.com/user-attachments/assets/5d983d23-7a06-4ff4-8174-5a2a9fb67170)
egrep 's{1,2}' newfile
## OUTPUT 
![WhatsApp Image 2025-09-12 at 17 22 28_4dd75d9a](https://github.com/user-attachments/assets/ccd742a8-e0e0-4524-a6c4-4b672f71566e)
cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
sed -n -e '3p' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 30 07_2927bf8f](https://github.com/user-attachments/assets/710cc277-8f1c-44b2-9b79-4ab23a7be922)

sed -n-e'$p'file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 30 38_0af4724b](https://github.com/user-attachments/assets/bfd01db1-8665-44e9-9268-579fd208eda6)

sed  -e 's/Ram/Sita/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 31 15_5e4faf35](https://github.com/user-attachments/assets/ebc03bec-81ec-4461-a271-5548a2cf81eb)

sed  -e '2s/Ram/Sita/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 31 51_23b2017e](https://github.com/user-attachments/assets/50814b8e-5d70-4d54-b4a6-1b87c650539e)

sed  '/tom/s/5000/6000/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 32 12_6ee8777c](https://github.com/user-attachments/assets/61e1e47c-5301-4a5e-b96b-da6f65b8704f)

sed -n -e '1,5p' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 32 33_35e672a5](https://github.com/user-attachments/assets/1bedefcc-1de8-4986-bb96-959e5e13dbfd)
sed -n -e '2,/Joe/p' file23
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 33 37_02db12c8](https://github.com/user-attachments/assets/324b5003-e4d7-4b46-afec-16d5eed8d8be)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT


![WhatsApp Image 2025-09-12 at 17 33 58_39959454](https://github.com/user-attachments/assets/c1c57a7e-25e4-4b50-ad0f-07f0adc1abd9)

seq 10 
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 34 16_e2f445ff](https://github.com/user-attachments/assets/bb577637-aa9a-4cfb-ab2d-280e16d6e87a)


seq 10 | sed -n '4,6p'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 35 55_7b1c72a7](https://github.com/user-attachments/assets/1e05fe01-19a7-4972-ba8d-25c3d36ead52)


seq 10 | sed -n '2,~4p'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 36 34_a9d56273](https://github.com/user-attachments/assets/d47357d1-2407-43f5-85b8-8607fdc90cc4)


seq 3 | sed '2a hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 36 55_b29b3ce4](https://github.com/user-attachments/assets/22ee8ec5-c9fa-4cc8-8aeb-58a2c968999d)


seq 2 | sed '2i hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 37 23_f21be9a2](https://github.com/user-attachments/assets/ba5538ce-4c93-4d52-9abb-cf2d86a00196)

seq 10 | sed '2,9c hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 37 54_756eefea](https://github.com/user-attachments/assets/ce116a01-21c0-41c4-a924-a195badb7953)

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 39 22_f7564a2b](https://github.com/user-attachments/assets/690dea4a-5c0e-4e7f-96df-e9e25d3ad8e5)
sed -n '2,4{s/$/*/;p}' file23
#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 40 05_0165c7b1](https://github.com/user-attachments/assets/de14f879-a285-4303-abdd-6eda8a15aee2)

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 17 42 23_3d5d0a1f](https://github.com/user-attachments/assets/97fb8be5-d114-4711-90fd-1c16e88b446a)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 17 43 20_8d0a080c](https://github.com/user-attachments/assets/f28d9187-0433-463d-a286-557318d4d45a)


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 43 47_35aefd4f](https://github.com/user-attachments/assets/17826454-2a90-45f1-9338-09d7bd55b1bc)


#Backup commands
tar -cvf backup.tar *
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 44 11_b02272f4](https://github.com/user-attachments/assets/ee8133f0-36be-4622-9843-722bb75dfa96)


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 45 55_1c20e142](https://github.com/user-attachments/assets/320470e2-f0a3-43c2-a1eb-d537f6649468)


tar -xvf backup.tar
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 46 21_bdccb10c](https://github.com/user-attachments/assets/f867bd6d-b734-4074-97ed-ef14997423f0)

gzip backup.tar

ls .gz
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 17 47 24_d5b5c759](https://github.com/user-attachments/assets/13d6a963-7a31-40ac-8448-b0c63a346793)

gunzip backup.tar.gz
## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 47 43_f250f5b1](https://github.com/user-attachments/assets/ad5fb46c-5e00-4fbb-81d3-8d4cc5e68b2f)

# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 48 30_bf27b77b](https://github.com/user-attachments/assets/e4ec32a8-4337-4779-ac12-e3609b272477)

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 48 50_fdff880a](https://github.com/user-attachments/assets/edc2b2ba-6efb-4619-9394-c33faced32e3)

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 50 22_e4d09e91](https://github.com/user-attachments/assets/c3062e45-2007-41ff-91a5-043619956f6c)

ls file1
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 50 43_16d51d7c](https://github.com/user-attachments/assets/c8c730d3-8964-42ee-bb3b-ab127b080e97)
echo $?
## OUTPUT 
![WhatsApp Image 2025-09-12 at 17 52 01_43767b18](https://github.com/user-attachments/assets/9b0c9f29-e7ba-48a6-85ab-319bd9e5db16)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT

![WhatsApp Image 2025-09-12 at 17 52 33_a8f25ea1](https://github.com/user-attachments/assets/b6305a07-fb3d-4234-8230-75cdab5999c6)

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT


![WhatsApp Image 2025-09-12 at 17 54 15_18cb1e1f](https://github.com/user-attachments/assets/39c797d9-fb34-483e-87c4-4084e76d7006)

chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 54 34_5118e3fd](https://github.com/user-attachments/assets/e59b9dd3-512f-4cee-9c89-c935121eda24)


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 57 15_8ea24a47](https://github.com/user-attachments/assets/04759b0c-5b8c-48a2-ad73-7886df616b43)

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 58 20_90355d56](https://github.com/user-attachments/assets/8fd9c9fc-5d4e-4e2d-b92f-f9c3e398e752)


# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
![WhatsApp Image 2025-09-12 at 17 59 03_cbf5736c](https://github.com/user-attachments/assets/cbf83bb7-be88-4185-83d2-2f46558714b0)

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
![WhatsApp Image 2025-09-12 at 17 59 55_40dd023f](https://github.com/user-attachments/assets/28fe6b82-99c2-4e61-a89e-676f408355ac)

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 18 00 28_69eb61b4](https://github.com/user-attachments/assets/d90cdbdc-ff87-4745-9575-af9819dde6dd)

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 01 07_721fc1c3](https://github.com/user-attachments/assets/b32f97ec-9c8c-4510-9ed1-2fcb3ee5150b)

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
##output
![WhatsApp Image 2025-09-12 at 18 02 16_f4781ce5](https://github.com/user-attachments/assets/2b65ebba-e6e9-4d50-8f4d-b263f33ecc60)

cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 ##output
 
 ![WhatsApp Image 2025-09-12 at 18 03 29_7dd428ee](https://github.com/user-attachments/assets/c0d67e5d-7a50-4592-b6e3-8aa5633f10dd)

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 ##output
 
 
 ![WhatsApp Image 2025-09-12 at 18 04 22_6e0c7575](https://github.com/user-attachments/assets/68a13ed0-e9e3-4ae1-89af-08af9f861b83)

cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 ##output
 ![WhatsApp Image 2025-09-12 at 18 05 26_7c8d5a72](https://github.com/user-attachments/assets/7b45a3e4-79a5-47a2-ace8-7c0da6c0b4a0)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
##output
![WhatsApp Image 2025-09-12 at 18 06 34_7848d1b3](https://github.com/user-attachments/assets/1164f9e5-8df5-43b6-be15-8e5e43ba8a9d)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
##output
![WhatsApp Image 2025-09-12 at 18 07 52_07132bc3](https://github.com/user-attachments/assets/1cce9923-f9dc-4073-b1c0-0cd84ec2b7fe)

cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
##output
![WhatsApp Image 2025-09-12 at 18 09 45_3d2d1c35](https://github.com/user-attachments/assets/1aa862f9-9fc3-4774-84e3-5e4e380c63b4)

cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
![WhatsApp Image 2025-09-12 at 18 17 55_684f042e](https://github.com/user-attachments/assets/9c845b18-5010-4407-87ed-1fd13658ecb2)

cat forinfile.sh 
4![WhatsApp Image 2025-09-12 at 18 18 53_de395bf6](https://github.com/user-attachments/assets/45fbd568-1c37-43e8-8dae-f88b2019f50e)

```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT

![WhatsApp Image 2025-09-12 at 18 27 28_5ece8537](https://github.com/user-attachments/assets/d2c48e1c-304f-4246-9b7d-d4d924e6d1d3)

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 26 55_6a0b1d46](https://github.com/user-attachments/assets/1623ce57-ccc0-47f8-b1b8-c41eccb0e316)

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 26 20_4481fa90](https://github.com/user-attachments/assets/7d358334-2e8f-439d-8b09-544e89c01be7)

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 ![WhatsApp Image 2025-09-12 at 18 25 50_5e3e335a](https://github.com/user-attachments/assets/9c659c2d-eb4a-485a-9a9e-708202bf5eb5)

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 ![WhatsApp Image 2025-09-12 at 18 25 14_e8135411](https://github.com/user-attachments/assets/5ea22fe6-5942-4ffa-88df-e9b8fd8df3eb)

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 18 23 18_450439f9](https://github.com/user-attachments/assets/05e061a4-e693-4feb-83e1-1f2d7201c34d)

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 18 24 05_504e1dbf](https://github.com/user-attachments/assets/346da1d4-322a-431d-a6f8-45d5f451b691)

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

![WhatsApp Image 2025-09-12 at 18 22 35_b8418258](https://github.com/user-attachments/assets/25d5d289-5835-4fc9-b2ea-5b45b0f88cb6)


$ ./exread1.sh 
 
cat funcex.sh
![WhatsApp Image 2025-09-12 at 18 21 48_8b9ef2e7](https://github.com/user-attachments/assets/e5551ce8-8f48-48b2-a7b5-957e4dc0c580)

```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 15 52_b2a20bef](https://github.com/user-attachments/assets/472b3eaf-c3d7-489d-98a4-6e2058b9baa0)

 ./funcex.sh 

 
 ./funcex.sh 1 2
 ## output
 ![WhatsApp Image 2025-09-12 at 18 15 12_299e4c08](https://github.com/user-attachments/assets/fe4b63ea-bde1-48f9-bea5-9b091eb20515)

cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3

 ![WhatsApp Image 2025-09-12 at 18 14 11_11e062b1](https://github.com/user-attachments/assets/09159720-970f-4477-b4f0-d5dd95c15f51)

 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 ![WhatsApp Image 2025-09-12 at 18 12 20_831dc5b5](https://github.com/user-attachments/assets/1dfb0465-dede-4ba0-854f-05641d370473)

cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 11 07_4086de85](https://github.com/user-attachments/assets/5a270ce0-022e-41b1-ab12-cb5f0d97c7b0)
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 

![WhatsApp Image 2025-09-12 at 18 10 32_e2eab8cf](https://github.com/user-attachments/assets/5a76f785-bd5f-4ee6-af6b-2f820dd34335)

# RESULT:
The Commands are executed successfully.
ripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 41 28_5c01dacd](https://github.com/user-attachments/assets/e9778b0f-4a65-4323-99de-b388c96f4f33)
cat < file2
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 41 58_e075d889](https://github.com/user-attachments/assets/06300be1-1718-4551-b551-175f1362624f)
# Comparing Files
cmp file1 file2
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 16 46 45_f6902247](https://github.com/user-attachments/assets/6e6af3bc-e468-42c6-b7d8-f517092df203)
comm file1 file2
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 16 48 49_faabc960](https://github.com/user-attachments/assets/37b5518d-265c-4820-adb4-2710b89a85a8)
diff file1 file2
## OUTPUT


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
cut -c1-3 file11
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 50 07_b4920c50](https://github.com/user-attachments/assets/c0037fdd-09de-4bf8-a29f-ffed6bfdee96)
cut -d "|" -f 1 file22
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 50 48_54dbdb2e](https://github.com/user-attachments/assets/cf62d642-7c35-45dd-a8d3-d2f8f3b7a4cc)
cut -d "|" -f 2 file22
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 51 15_33b013ce](https://github.com/user-attachments/assets/154f8566-b99a-4d9f-b698-f45fec6b8e5a)
cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 53 14_8e3b52d5](https://github.com/user-attachments/assets/a1ab4a00-def7-47e7-82aa-a085e9083c83)
grep hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 53 39_648b1a7c](https://github.com/user-attachments/assets/1af20d18-38d7-4838-9193-687696655431)
grep -v hello newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 11 50_59bdbb46](https://github.com/user-attachments/assets/1a98d332-2297-4ce0-9477-b8b1bb1fc161)

cat newfile | grep -i "hello"
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 09 45_637135a7](https://github.com/user-attachments/assets/8de8eaef-f65d-464e-b158-93cdcfc51508)

cat newfile | grep -i -c "hello"
## OUTPUT
![WhatsApp Image 2025-09-12 at 16 58 52_2c655907](https://github.com/user-attachments/assets/9016389f-9291-480b-aa22-4821eb7fa847)
grep -R ubuntu /etc
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 00 19_91a34f01](https://github.com/user-attachments/assets/63059349-e8cd-49d3-a77a-0c09576ed29d)
grep -w -n world newfile   
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 00 40_6f98b2af](https://github.com/user-attachments/assets/735a4e61-36f4-4646-82d3-f8786be6de34)
cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 13 58_df8c18a6](https://github.com/user-attachments/assets/c66a00d0-2f31-442e-9491-8a21a9a77dc7)
egrep -w '(H|h)ello' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 15 02_3e7bf289](https://github.com/user-attachments/assets/5d5d23cf-d42a-4842-b14a-b9b57cfe36d7)
egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 15 49_2388e863](https://github.com/user-attachments/assets/947cc3e0-9536-4617-ba81-20c264890054)
egrep '(^hello)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 16 43_2f56d67d](https://github.com/user-attachments/assets/bbbb00ef-1cce-415e-aa16-57511e3acbb5)
egrep '(world$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 17 23_095c213b](https://github.com/user-attachments/assets/bc4d7001-d43d-46a0-b732-d3a35740fd9a)
egrep '(World$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 18 20_17b46e92](https://github.com/user-attachments/assets/053c5673-1c73-479e-b456-2b179b5610e1)
egrep '((W|w)orld$)' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 18 55_04e8da42](https://github.com/user-attachments/assets/9930ae2e-468c-4437-a4d8-42608951b4d9)
egrep '[1-9]' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 19 49_b89f97c9](https://github.com/user-attachments/assets/e871bdd5-0eeb-4a33-819a-9acde03de19e)
egrep 'Linux.*world' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 20 28_39e185c3](https://github.com/user-attachments/assets/55ceee3c-3f03-4712-89bd-2c89597ffc3a)
egrep 'Linux.*World' newfile 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 21 04_2e26dad4](https://github.com/user-attachments/assets/2df181bd-3cb0-47fa-9b37-0c0f5fbf5023)
egrep l{2} newfile
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 22 02_521e0f5d](https://github.com/user-attachments/assets/5d983d23-7a06-4ff4-8174-5a2a9fb67170)
egrep 's{1,2}' newfile
## OUTPUT 
![WhatsApp Image 2025-09-12 at 17 22 28_4dd75d9a](https://github.com/user-attachments/assets/ccd742a8-e0e0-4524-a6c4-4b672f71566e)
cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
sed -n -e '3p' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 30 07_2927bf8f](https://github.com/user-attachments/assets/710cc277-8f1c-44b2-9b79-4ab23a7be922)

sed -n-e'$p'file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 30 38_0af4724b](https://github.com/user-attachments/assets/bfd01db1-8665-44e9-9268-579fd208eda6)

sed  -e 's/Ram/Sita/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 31 15_5e4faf35](https://github.com/user-attachments/assets/ebc03bec-81ec-4461-a271-5548a2cf81eb)

sed  -e '2s/Ram/Sita/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 31 51_23b2017e](https://github.com/user-attachments/assets/50814b8e-5d70-4d54-b4a6-1b87c650539e)

sed  '/tom/s/5000/6000/' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 32 12_6ee8777c](https://github.com/user-attachments/assets/61e1e47c-5301-4a5e-b96b-da6f65b8704f)

sed -n -e '1,5p' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 32 33_35e672a5](https://github.com/user-attachments/assets/1bedefcc-1de8-4986-bb96-959e5e13dbfd)
sed -n -e '2,/Joe/p' file23
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 33 37_02db12c8](https://github.com/user-attachments/assets/324b5003-e4d7-4b46-afec-16d5eed8d8be)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT


![WhatsApp Image 2025-09-12 at 17 33 58_39959454](https://github.com/user-attachments/assets/c1c57a7e-25e4-4b50-ad0f-07f0adc1abd9)

seq 10 
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 34 16_e2f445ff](https://github.com/user-attachments/assets/bb577637-aa9a-4cfb-ab2d-280e16d6e87a)


seq 10 | sed -n '4,6p'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 35 55_7b1c72a7](https://github.com/user-attachments/assets/1e05fe01-19a7-4972-ba8d-25c3d36ead52)


seq 10 | sed -n '2,~4p'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 36 34_a9d56273](https://github.com/user-attachments/assets/d47357d1-2407-43f5-85b8-8607fdc90cc4)


seq 3 | sed '2a hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 36 55_b29b3ce4](https://github.com/user-attachments/assets/22ee8ec5-c9fa-4cc8-8aeb-58a2c968999d)


seq 2 | sed '2i hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 37 23_f21be9a2](https://github.com/user-attachments/assets/ba5538ce-4c93-4d52-9abb-cf2d86a00196)

seq 10 | sed '2,9c hello'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 37 54_756eefea](https://github.com/user-attachments/assets/ce116a01-21c0-41c4-a924-a195badb7953)

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 39 22_f7564a2b](https://github.com/user-attachments/assets/690dea4a-5c0e-4e7f-96df-e9e25d3ad8e5)
sed -n '2,4{s/$/*/;p}' file23
#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 40 05_0165c7b1](https://github.com/user-attachments/assets/de14f879-a285-4303-abdd-6eda8a15aee2)

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 17 42 23_3d5d0a1f](https://github.com/user-attachments/assets/97fb8be5-d114-4711-90fd-1c16e88b446a)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT
![WhatsApp Image 2025-09-12 at 17 43 20_8d0a080c](https://github.com/user-attachments/assets/f28d9187-0433-463d-a286-557318d4d45a)


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 43 47_35aefd4f](https://github.com/user-attachments/assets/17826454-2a90-45f1-9338-09d7bd55b1bc)


#Backup commands
tar -cvf backup.tar *
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 44 11_b02272f4](https://github.com/user-attachments/assets/ee8133f0-36be-4622-9843-722bb75dfa96)


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 45 55_1c20e142](https://github.com/user-attachments/assets/320470e2-f0a3-43c2-a1eb-d537f6649468)


tar -xvf backup.tar
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 46 21_bdccb10c](https://github.com/user-attachments/assets/f867bd6d-b734-4074-97ed-ef14997423f0)

gzip backup.tar

ls .gz
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 17 47 24_d5b5c759](https://github.com/user-attachments/assets/13d6a963-7a31-40ac-8448-b0c63a346793)

gunzip backup.tar.gz
## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 47 43_f250f5b1](https://github.com/user-attachments/assets/ad5fb46c-5e00-4fbb-81d3-8d4cc5e68b2f)

# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 48 30_bf27b77b](https://github.com/user-attachments/assets/e4ec32a8-4337-4779-ac12-e3609b272477)

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 48 50_fdff880a](https://github.com/user-attachments/assets/edc2b2ba-6efb-4619-9394-c33faced32e3)

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 ![WhatsApp Image 2025-09-12 at 17 50 22_e4d09e91](https://github.com/user-attachments/assets/c3062e45-2007-41ff-91a5-043619956f6c)

ls file1
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 50 43_16d51d7c](https://github.com/user-attachments/assets/c8c730d3-8964-42ee-bb3b-ab127b080e97)
echo $?
## OUTPUT 
![WhatsApp Image 2025-09-12 at 17 52 01_43767b18](https://github.com/user-attachments/assets/9b0c9f29-e7ba-48a6-85ab-319bd9e5db16)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT

![WhatsApp Image 2025-09-12 at 17 52 33_a8f25ea1](https://github.com/user-attachments/assets/b6305a07-fb3d-4234-8230-75cdab5999c6)

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT


![WhatsApp Image 2025-09-12 at 17 54 15_18cb1e1f](https://github.com/user-attachments/assets/39c797d9-fb34-483e-87c4-4084e76d7006)

chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 54 34_5118e3fd](https://github.com/user-attachments/assets/e59b9dd3-512f-4cee-9c89-c935121eda24)


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![WhatsApp Image 2025-09-12 at 17 57 15_8ea24a47](https://github.com/user-attachments/assets/04759b0c-5b8c-48a2-ad73-7886df616b43)

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 17 58 20_90355d56](https://github.com/user-attachments/assets/8fd9c9fc-5d4e-4e2d-b92f-f9c3e398e752)


# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
![WhatsApp Image 2025-09-12 at 17 59 03_cbf5736c](https://github.com/user-attachments/assets/cbf83bb7-be88-4185-83d2-2f46558714b0)

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
![WhatsApp Image 2025-09-12 at 17 59 55_40dd023f](https://github.com/user-attachments/assets/28fe6b82-99c2-4e61-a89e-676f408355ac)

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 18 00 28_69eb61b4](https://github.com/user-attachments/assets/d90cdbdc-ff87-4745-9575-af9819dde6dd)

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 01 07_721fc1c3](https://github.com/user-attachments/assets/b32f97ec-9c8c-4510-9ed1-2fcb3ee5150b)

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
##output
![WhatsApp Image 2025-09-12 at 18 02 16_f4781ce5](https://github.com/user-attachments/assets/2b65ebba-e6e9-4d50-8f4d-b263f33ecc60)

cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 ##output
 
 ![WhatsApp Image 2025-09-12 at 18 03 29_7dd428ee](https://github.com/user-attachments/assets/c0d67e5d-7a50-4592-b6e3-8aa5633f10dd)

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 ##output
 
 
 ![WhatsApp Image 2025-09-12 at 18 04 22_6e0c7575](https://github.com/user-attachments/assets/68a13ed0-e9e3-4ae1-89af-08af9f861b83)

cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 ##output
 ![WhatsApp Image 2025-09-12 at 18 05 26_7c8d5a72](https://github.com/user-attachments/assets/7b45a3e4-79a5-47a2-ace8-7c0da6c0b4a0)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
##output
![WhatsApp Image 2025-09-12 at 18 06 34_7848d1b3](https://github.com/user-attachments/assets/1164f9e5-8df5-43b6-be15-8e5e43ba8a9d)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
##output
![WhatsApp Image 2025-09-12 at 18 07 52_07132bc3](https://github.com/user-attachments/assets/1cce9923-f9dc-4073-b1c0-0cd84ec2b7fe)

cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
##output
![WhatsApp Image 2025-09-12 at 18 09 45_3d2d1c35](https://github.com/user-attachments/assets/1aa862f9-9fc3-4774-84e3-5e4e380c63b4)

cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
![WhatsApp Image 2025-09-12 at 18 17 55_684f042e](https://github.com/user-attachments/assets/9c845b18-5010-4407-87ed-1fd13658ecb2)

cat forinfile.sh 
4![WhatsApp Image 2025-09-12 at 18 18 53_de395bf6](https://github.com/user-attachments/assets/45fbd568-1c37-43e8-8dae-f88b2019f50e)

```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT

![WhatsApp Image 2025-09-12 at 18 27 28_5ece8537](https://github.com/user-attachments/assets/d2c48e1c-304f-4246-9b7d-d4d924e6d1d3)

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 26 55_6a0b1d46](https://github.com/user-attachments/assets/1623ce57-ccc0-47f8-b1b8-c41eccb0e316)

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 26 20_4481fa90](https://github.com/user-attachments/assets/7d358334-2e8f-439d-8b09-544e89c01be7)

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 ![WhatsApp Image 2025-09-12 at 18 25 50_5e3e335a](https://github.com/user-attachments/assets/9c659c2d-eb4a-485a-9a9e-708202bf5eb5)

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 ![WhatsApp Image 2025-09-12 at 18 25 14_e8135411](https://github.com/user-attachments/assets/5ea22fe6-5942-4ffa-88df-e9b8fd8df3eb)

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 ![WhatsApp Image 2025-09-12 at 18 23 18_450439f9](https://github.com/user-attachments/assets/05e061a4-e693-4feb-83e1-1f2d7201c34d)

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

![WhatsApp Image 2025-09-12 at 18 24 05_504e1dbf](https://github.com/user-attachments/assets/346da1d4-322a-431d-a6f8-45d5f451b691)

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

![WhatsApp Image 2025-09-12 at 18 22 35_b8418258](https://github.com/user-attachments/assets/25d5d289-5835-4fc9-b2ea-5b45b0f88cb6)


$ ./exread1.sh 
 
cat funcex.sh
![WhatsApp Image 2025-09-12 at 18 21 48_8b9ef2e7](https://github.com/user-attachments/assets/e5551ce8-8f48-48b2-a7b5-957e4dc0c580)

```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 15 52_b2a20bef](https://github.com/user-attachments/assets/472b3eaf-c3d7-489d-98a4-6e2058b9baa0)

 ./funcex.sh 

 
 ./funcex.sh 1 2
 ## output
 ![WhatsApp Image 2025-09-12 at 18 15 12_299e4c08](https://github.com/user-attachments/assets/fe4b63ea-bde1-48f9-bea5-9b091eb20515)

cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3

 ![WhatsApp Image 2025-09-12 at 18 14 11_11e062b1](https://github.com/user-attachments/assets/09159720-970f-4477-b4f0-d5dd95c15f51)

 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 ![WhatsApp Image 2025-09-12 at 18 12 20_831dc5b5](https://github.com/user-attachments/assets/1dfb0465-dede-4ba0-854f-05641d370473)

cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT
![WhatsApp Image 2025-09-12 at 18 11 07_4086de85](https://github.com/user-attachments/assets/5a270ce0-022e-41b1-ab12-cb5f0d97c7b0)
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 

![WhatsApp Image 2025-09-12 at 18 10 32_e2eab8cf](https://github.com/user-attachments/assets/5a76f785-bd5f-4ee6-af6b-2f820dd34335)

# RESULT:
The Commands are executed successfully.
