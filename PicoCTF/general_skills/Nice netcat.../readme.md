# Nice netcat...

Category : General Skills 
Point : 15 

![images](https://github.com/R1nto/CTF/blob/main/PicoCTF/general_skills/Obedient_Cat/images/Nice_Netcat.png)

## Description

There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 35652, but it doesn't speak English...

## Solve 

Jadi kita diberi sebuah nc lalu buka nc nya 

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/Wave_a_flag]
└─$ nc mercury.picoctf.net 35652
112 
105 
99 
111 
67 
84 
70 
123 
103 
48 
48 
100 
95 
107 
49 
116 
116 
121 
33 
95 
110 
49 
99 
51 
95 
107 
49 
116 
116 
121 
33 
95 
57 
98 
51 
98 
55 
51 
57 
50 
125 
10 
```

setelah melihat isi dari nc tersebut saya berkesimpulan bahwa ini harus di decrypt jadi saya ke tool andalan saya yaitu [cyberchef](https://gchq.github.io/CyberChef)

![images](https://github.com/R1nto/CTF/blob/main/PicoCTF/general_skills/Obedient_Cat/images/cyberchef.png)

**picoCTF{g00d_k1tty!_n1c3_k1tty!_9b3b7392}**
