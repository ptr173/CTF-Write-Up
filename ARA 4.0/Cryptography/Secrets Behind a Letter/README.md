# Secrets Behind a Letter

## Description
Melon and Edith went to an labyrinth and they should break the code written on a letter in a box in order to escape the labyrinth.

Open the letter and break the code

## Attachment
[Letter.txt](https://github.com/ptr173/CTF-Write-Up/files/11037132/Letter.txt)

## Steps

1. Pada file attachment tersebut terdapat serangkaian angka

![image](https://user-images.githubusercontent.com/123644468/226823241-a946b0a6-5301-4952-ac92-482e133cd902.png)

2. Setelah dilihat p,q,c,e merupakan bagian dari RSA, tetapi untuk RSA membutuhkan value n yang saya dapatkan dengan mengkalikan p dan q
    
    hasil dari n:
    157160024420901491275151303069558764137050893302421347934387021008089237099810507796321179096121981028783897823233363219558663447491261939665357360882456316085702311589787337774153460302744843626838158086562582492360568567614325107754450077486851324804696560335578971886327235046960425388107307559439500825931

3. Setelah mendapatkan n, saya menggunakan online tool untuk men-decrypt RSA dan didapatkan lah flagnya

![image6](https://user-images.githubusercontent.com/123644468/226824105-c4266f31-bca9-443b-9237-18f5e7caa068.png)

## Flag
ARA2023{1t_turn5_0ut_to_b3_an_rsa}
