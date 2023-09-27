# Wave a flag

Category : General Skills

Point : 10

![images](images/Wave_a_flag.png)

## Description

Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...

## Solve

Pertama download file nya 

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/Wave_a_flag]
└─$ wget https://mercury.picoctf.net/static/cfea736820f329083dab9558c3932ada/warm
```

lalu untuk mencari flagnya kita gunakan fungsi strings dan grep

```console
┌──(rinto㉿LAPTOP-LUUOMDHF)-[~/CTF/pico/Wave_a_flag]
└─$ strings warm | grep "pico"
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_30e77291}
```

**picoCTF{b1scu1ts_4nd_gr4vy_30e77291}**

