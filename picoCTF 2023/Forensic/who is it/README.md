# who is it

## Description
Someone just sent you an email claiming to be Google's co-founder Larry Page but you suspect a scam.
Can you help us identify whose mail server the email actually originated from?
Download the email file [here](https://github.com/ptr173/CTF-Write-Up/files/11128688/email-export.zip)
. Flag: picoCTF{FirstnameLastname}

## Hints
1. whois can be helpful on IP addresses also, not only domain names.

## Steps
1. Dari attachment tersebut diberikan email dalam bentuk plain text atau eml file

![image](https://user-images.githubusercontent.com/123644468/229271570-41bdcb2b-b220-4648-9df1-04b8c37aa86b.png)

2. Jika dibuka menggunakan notepad atau text editor lainnya maka kita dapat menemukan IP address pengirim pada bagian recieved

![image](https://user-images.githubusercontent.com/123644468/229271782-95e55316-6d05-46e2-8445-6c49fb95167a.png)

3. Dari IP address tersebut kita bisa mendapatkan first name dan last name nya dengan mencari di web whois

![image](https://user-images.githubusercontent.com/123644468/229272038-321b87b9-5335-4d6b-8d32-5a32bbdf9454.png)

4. Setelah mencari IP address pada web who is tersebut didapatkanlah first name dan last name yang merupakan flagnya

## Flag
picoCTF{WilhelmZwalina}
