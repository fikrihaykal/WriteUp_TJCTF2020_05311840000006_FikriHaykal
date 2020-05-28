# Titanic - 35 points

## Problem
I wrapped tjctf{} around the lowercase version of a word said in the 1997 film "Titanic" and created an MD5 hash of it: `9326ea0931baf5786cde7f280f965ebb`.

## Solution
- Yang harus dilakukan pertama kali adalah mengunduh subtitle atau script film titanic.
  ![alt_text](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Titanic3.png?raw=True)
- Setiap kata harus dibungkus dengan `tjctf{kata_kunci}` agar bisa menghasilkan hash yang sama.
- Setelah itu bisa menggunakan `MD5 Hash Generator` untuk mencari hasil hash yang sama dengan yang ada pada deskripsi.
  ![alt_text](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Titanic1.png?raw=True)
- Tentu akan ditemukan sebuah hasil hash yang sama dengan deskripsi, yang mana kata tersebut merupakan sebuah flag
  ![alt_text](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Titanic2.png?raw=True)

## Flag
```
tjctf{marlborough's}
```
