# Rap God - 40 points

## Problem
My rapper friend Big Y sent me his [latest track](https://static.tjctf.org/302ed01b56ae5988e8b8ad8d9bba402a2934c71508593f5dc9e95aed913d20cf_BigYAudio.mp3) but something sounded a little off about it. Help me find out if he was trying to tell me something with it. Submit your answer as tjctf{message}

## Solution
- Tidak ada flag dalam metadatanya, oleh karena itu kita harus mencoba melihat frekuensi dan spectrogramnya
- Saat melihat spectrogramnya, ditemukan beberapa simbol wingdings
![flag_image](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/RapGod1.jpg?raw=True)
- Selanjutnya adalah menerjemahkan simbol tersebut kedalam plaintext
![flag_image](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/RapGod2.jpg?raw=True)

## Flag
```
tjctf{QUICKSONIC}
```
