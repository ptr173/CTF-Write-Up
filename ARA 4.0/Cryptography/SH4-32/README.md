# SH4-32
## Description
Sze received an ecnrypted file and a message containing the clue of the file password from her friend.

The clue was a hash value : 9be9f4182c157b8d77f97d3b20f68ed6b8533175831837c761e759c44f6feeb8

Decrypt the file password!

## Attachment
[Dictionary.txt](https://github.com/ptr173/CTF-Write-Up/files/11037212/Dictionary.txt)

## Steps

1. Pada file attachment terdapat banyak strings di dalamnya
2. Lalu salah satu strings tersebut terlihat mencurigakan dan saya mencoba melakukan encrypt SHA-256 pada strings tersebut dan mencocokkannya dengan clue pada soal
    
    strings: 415241323032337b6834736833645f30525f6e4f545f6834736833647d
    
    ![image13](https://user-images.githubusercontent.com/123644468/226826962-0cf24937-f7e7-44f3-af41-a3f73d55a148.png)

3. Setelah dicocokkan dan hasilnya sama, kita telah menemukan hasil decryptnya dan setelah dilihat-lihat strings tersebut merupakan bilangan heksadesimal
4. Berikutnya saya mengubah bilangan hex tersebut ke ascii text dan didapatkanlah flagnya

![image21](https://user-images.githubusercontent.com/123644468/226827308-c199d0c3-b1a5-453f-9096-4e27c2827b91.png)

## Flag
ARA2023{h4sh3d_0R_nOT_h4sh3d}
