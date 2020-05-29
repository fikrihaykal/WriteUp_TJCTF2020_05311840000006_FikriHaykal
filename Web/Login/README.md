# Login - 30 points

## Problem
Could you login into this [very secure site](https://login.tjctf.org/)? Best of luck!


## Solution
- Untuk login kali ini, tidak memerlukan SQL injection.
- Kita hanya perlu melihat javascript yang digunakan untuk menampilkan autentikasi login.
  ```
  var _0xb31c=['value','c2a094f7d35f2299b414b6a1b3bd595a','Sorry.\x20Wrong\x20username\x20or\x20password.','admin','tjctf{','getElementsByName','toString'];
  (function(_0xcd8e51, _0x31ce84) {
   var _0x55c419 = function(_0x56392e) {
    while (--_0x56392e) {
     _0xcd8e51['push'](_0xcd8e51['shift']());
    }
   };
   _0x55c419(++_0x31ce84);
  }(_0xb31c, 0x1e7));
  var _0x4a84 = function(_0xcd8e51, _0x31ce84) {
   _0xcd8e51 = _0xcd8e51 - 0x0;
   var _0x55c419 = _0xb31c[_0xcd8e51];
   return _0x55c419;
  };
  checkUsername = function() {
   username = document[_0x4a84('0x1')]('username')[0x0]['value'];
   password = document[_0x4a84('0x1')]('password')[0x0][_0x4a84('0x3')];
   temp = md5(password)[_0x4a84('0x2')]();
   if (username == _0x4a84('0x6') && temp == _0x4a84('0x4')) alert(_0x4a84('0x0') + password + '890898}');
   else alert(_0x4a84('0x5'));
  };
  ```
- Dapat diketahui bahwa kita harus login menggunakan username `admin` dan passwordnya adalah hasil decode md5 dari `c2a094f7d35f2299b414b6a1b3bd595a`
  ![alt_text](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Login1.png?raw=True)
- Setelah ditemukan, maka kita harus login untuk mengetahui flagnya.
  ![alt_text](https://github.com/fikrihaykal/WriteUp_TJCTF2020_05311840000006_FikriHaykal/blob/master/src/Login2.png?raw=True)
  
## Flag
```
tjctf{horizons890898}
```
