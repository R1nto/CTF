# Tab, Tab, Attack

Category : General Skills

Point : 20 

![images](https://github.com/R1nto/CTF/blob/main/PicoCTF/general_skills/Tab%2C%20Tab%2C%20Attack/images/Tab_Tab_%20Attack.png)

## Description

Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: Addadshashanammu.zip

## Solve

jadi pertama saya unzip terlebih dahulu file nya 

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack]
└─$ unzip Addadshashanammu.zip 
```

setelah di unzip saya buka satu per satu folder yang diberikan didalam file zip tersebut 

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack]
└─$ cd Addadshashanammu

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu]
└─$ ls 
Almurbalarammi

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu]
└─$ cd Almurbalarammi/

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi]
└─$ ls
Ashalmimilkala

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi]
└─$ cd Ashalmimilkala/

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala]
└─$ ls
Assurnabitashpi

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala]
└─$ cd Assurnabitashpi/                                                      

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi]
└─$ ls
Maelkashishi

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi]
└─$ cd Maelkashishi/                                                         

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi]
└─$ ls                                                                       
Onnissiralis

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi]
└─$ cd Onnissiralis/                                                         

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis]
└─$ ls                                                                       
Ularradallaku

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis]
└─$ cd Ularradallaku/                                                        

┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ ls                                                                       
fang-of-haynekhtnamet
```

dan di folder terakhir saya lihat ada file dengan senjata andalan saya yaitu dengan strings

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/tab_tab_attack/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ strings fang-of-haynekhtnamet | grep "pico"
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_76266e38}
```

**picoCTF{l3v3l_up!_t4k3_4_r35t!_76266e38}**
