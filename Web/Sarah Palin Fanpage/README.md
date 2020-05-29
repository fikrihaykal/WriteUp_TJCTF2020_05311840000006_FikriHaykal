# Sarah Palin Fanpage - 35 points

## Problem
Are you a true fan of Alaska's most famous governor? Visit the [Sarah Palin fanpage](https://sarah_palin_fanpage.tjctf.org/).


## Solution
- Untuk problem ini sangat mudah, karena kita bisa mengatur sebuah cookie web tersebut.
  ```
  eyIxIjpmYWxzZSwiMiI6ZmFsc2UsIjMiOmZhbHNlLCI0IjpmYWxzZSwiNSI6ZmFsc2UsIjYiOmZhbHNlLCI3IjpmYWxzZSwiOCI6ZmFsc2UsIjkiOmZhbHNlLCIxMCI6ZmFsc2V9
  ```
- Selanjutnya menerjemahkan dari base64 menjadi plaintext
  ```
  {"1":false,"2":false,"3":false,"4":false,"5":false,"6":false,"7":false,"8":false,"9":false,"10":false}
  ```
- Ubah semua nilai menjadi true, lalu edit cookie pada browser dan reload page `VIP Member`.
  ```
  eyIxIjp0cnVlLCIyIjp0cnVlLCIzIjp0cnVlLCI0Ijp0cnVlLCI1Ijp0cnVlLCI2Ijp0cnVlLCI3Ijp0cnVlLCI4Ijp0cnVlLCI5Ijp0cnVlLCIxMCI6dHJ1ZX0=
  ```

## Flag
```
tjctf{wkDd2Pi4rxiRaM5lOcLo979rru8MFqVHKdTqPBm4k3iQd8n0sWbBkOfuq9vDTGN9suZgYlH3jq6QTp3tG3EYapzsTHL7ycqRTP5Qf6rQSB33DcQaaqwQhpbuqPBm4k3iQd8n0sWbBkOf}
```
