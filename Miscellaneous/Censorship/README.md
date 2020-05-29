# Censorship - 30 points

## Problem
My friend has some top-secret government intel. He left a message, but the government censored him! They didn't want the information to be leaked, but can you find out what he was trying to say?
<br />
`nc p1.tjctf.org 8003`

## Solution
  ![censorship](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Censorship1.jpg?raw=True)
- Yang harus dilakukan pertama kali adalah membuka aplikasi `wireshark` pada linux dan rekam salah satu `wired interface` yang tersedia.
- Jalankan perintah `nc p1.tjctf.org 8003` pada terminal.
- Jawab pertanyaan yang ada, sehingga wireshark akan mendapatkan paket baru.
- Export paket dengan cara `File - Export Packet Disserctions - As Plain Text...`
- Setelah itu buka file, dan kemudian flag akan ditemukan

## Flag
```
tjctf{TH3_1llum1n4ti_I5_R3aL}
```
