# Chord Encoder - 40 points

## Problem
I tried creating my own [chords](https://static.tjctf.org/67be5bd036a4be8323314d1da6ad2e673963f76634a62ec47d53fb07a04a3722_chords.txt), but my [encoded sheet music](https://static.tjctf.org/c29857b8d4d1b2dfe502b5053d73844a08358ae681b2af8de6829b765dc2c28e_notes.txt) is a little hard to read. Please play me my song!
<br />
[chord_encoder.py](https://static.tjctf.org/da36df431da358250884ff9765e8c0c5f054b845aff31b85e37229159176bb9f_chord_encoder.py)


## Solution
- Disini saya menggunakan cara manual untuk menerjemahkan chord tersebut.
  ```
  1121112111211002112101121121001001210000101221121011200102000110120200101100100111211011001020020010111012011202001011112110121121011211211002112110020200101111210112020010111121010112102001121100211211011020020001010
  ```
- Pertama kita harus mengubah encoded sheet music menjadi berbentuk huruf seperti chords.
  ```
  FFFcFAFGGbGaFAGDGCEfGGFfGDEfCAEfFCFAFcFcEfFAEfFdFEFcFfDDGd
  ```
- Sesuai dengan scrypt python yang ada, huruf kapital diminta untuk diubah menjadi sebuah angka.
  ```
  666c61677b7a6174735f776f745f315f63616c6c5f615f6d656c6f447d
  ```
- Langkah terakhir adalah menerjemahkan dari base64 menjadi plaintext

## Flag
```
flag{zats_wot_1_call_a_meloD}
```
