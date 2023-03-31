# FindAndOpen

## Description
Someone might have hidden the password in the trace file.
Find the key to unlock this file. This tracefile might be good to analyze.

## Hint
1. Download the pcap and look for the password or flag.
2. Don't try to use a password cracking tool, there are easier ways here.

## Steps
1. Dari hint pertama dikatakan dalam file pcap tersebut terdapat password ataupun flag
2. Setelah membuka dan mencari pada file pcap tersebut terdapat data dalam bentuk base 64

![image](https://user-images.githubusercontent.com/123644468/229022893-e74ded8e-8108-4b04-9c18-a7529944474f.png)

3. Setelah diterjemahkan didapatkan lah secret atau pecahan dari flag tersebut

![image](https://user-images.githubusercontent.com/123644468/229023010-da50706b-94fd-44be-8b48-6afdf4878bce.png)

4. Berikutnya dari pecahan flag tersebut saya gunakan sebagai password dari file zip yang diberikan 

![image](https://user-images.githubusercontent.com/123644468/229023208-ad8dcb8f-67f6-41a9-8d86-45e953a1ddd1.png)

5. Setelah di extract terdapat file yang didalamnya berisikan flag tersebut

![image](https://user-images.githubusercontent.com/123644468/229023415-67667a47-f7a9-4867-833c-6f2c6ccd06d5.png)

## Flag
picoCTF{R34DING_LOKd_fil56_succ3ss_419835ef}
