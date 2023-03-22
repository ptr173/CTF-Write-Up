# Thinker
## Description
I always overthink about finding other part of myself, can you help me?
## Attachment
[confused.png](https://user-images.githubusercontent.com/123644468/226792393-ee34cb1b-6790-4b63-89a5-1539e8abbe5e.png)
## Steps

1. Pada attachment terdapat sebuah gamabar png bernama confused.png
2. Berikutnya saya mencoba menggunakan binwalk untuk mengetahui apakah terdapat file lain yang dimasukan kedalam gambar tersebut
3. Setelah dilakukan binwalk ternyata terdapat banyak file zip didalamnya dan berikutnya saya extract file tersebut
![image26](https://user-images.githubusercontent.com/123644468/226790408-acf83af5-7443-4376-96e1-75bc6ea5f6d6.png)
4. Setelah mengextract semua file zip didapatkan “e.txt”, “a.txt”, “s.txt”, dan “y.png”
5. Untuk file .txt berisikan pecahan dari flag
![image4](https://user-images.githubusercontent.com/123644468/226790912-a6b33e39-421d-42db-abde-9e000f1b3e91.png)
![image16](https://user-images.githubusercontent.com/123644468/226791061-66026683-d758-4401-9835-c21e95724686.png)
![image1](https://user-images.githubusercontent.com/123644468/226791072-bcd4ac50-ab36-4e64-aa32-0e46954f5f73.png)
6. Lalu saya merubah text tersebut dengan bantuan online tools dan mendapatkan hasil sebagai berikut:

    e.txt (base 64)
    QVJBMjAyM3s=  → ARA2023{

    a.txt (hex)
    35216D706C335F → 5!mpl3_ 

    s.txt (binary)
    01000011 00110000 01110010 01110010 01110101 01110000 01110100 00110011 01100100 01011111 → C0rrupt3d_
  
7. Sedangkan untuk y.png merupakan sebuah file .png yang corrupted
8. Berikutnya saya mencoba menganalisa file tersebut
![image24](https://user-images.githubusercontent.com/123644468/226791936-516ab776-2b6a-4d28-9f82-c4bead25d2bc.png)
9. Setelah dianalisa terdapat kesalahan pada bagian “!ZxR” (21 5A 78 52) yang seharusnya “.PNG” (89 50 4E 47) dan “RRH\” (52 52 48 5C) yang seharusnya “IHDR” (49 48 44 52) 
![image18](https://user-images.githubusercontent.com/123644468/226792182-6d938c15-13aa-4bb6-8a0d-78e78b2a83c8.png)
10. Setelah diperbaiki file y.png sudah dapat dibuka
![image9](https://user-images.githubusercontent.com/123644468/226792596-f0a70833-6516-4199-94a1-e90f23eb7a22.png)
11. Setelah dibuka terdapat serangkaian angka yang merupakan bilangan ascii dan jika ditranslate maka akan mendapatkan bagian flag terakhir
  49 109 52 103 101 53 125 → 1m4ge5}
12. Terakhir gabungkan semua bagian dan didapatkan flagnya
  
## Flag
ARA2023{5!mpl3_C0rrupt3d_1m4ge5}
