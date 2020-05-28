# Tap Dancing - 25 points

## Problem
My friend is trying to teach me to dance, but I am not rhythmically coordinated! They sent me a list of [dance moves](https://static.tjctf.org/518d6851c71c5482dbd5bbe812b678684238c8f4e9e9b3d95a188f7db83a0870_cipher.txt) but they're all numbers! Can you help me figure out what they mean so I can learn the dance? <br />
NOTE: Flag is not in flag format. 

```
1101111102120222020120111110101222022221022202022211
```

## Solution
- Dari cipher tersebut dapat diketahui bahwa cipher tersebut berupa sandi morse.
- Kita harus mengonversi nilai `0` menjadi `spasi`, `1` menjadi `-` dan `2` menjadi `.`
  ```
  -- ----- .-. ... . -. ----- -... ....- ... . ...--
  ```
- Setelah itu kita dapat melakukan `decode` sandi morse tersebut menjadi plaintext
  ```
  M0RSEN0B4SE3
  ```

## Flag
```
tjctf{M0RSEN0B4SE3}
```
