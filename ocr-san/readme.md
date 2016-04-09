OCRed with san.traineddata from 3.04 release
===

```
$ time ./tessaccsummary ../imagesBIG .. san tif
Sahadeva: 78.37%
Siddhanta: 75.57%
average: 76.97%

real    59m12.086s
user    58m32.754s
sys     0m3.735s

$ time ./tessaccsummary -w ../imagesBIG .. san tif
Sahadeva: 13.80%
Siddhanta: 12.98%
average: 13.39%

real    98m3.378s
user    88m7.457s
sys     0m8.223s
```

```
$ time ./tessaccsummary ../imagessan .. san png
aanagarishreel3skttext: 49.88%
arialunicodeskttext: 46.70%
janasanskrittext: 41.27%
kalimatiskttext: 66.27%
mangalskttext: 29.72%
sanskrit2003skttext: 63.68%
shreeskttext: 52.36%
surekhskttext: 23.11%
yogeshskttext: 59.20%
average: 48.02%

real    42m7.727s
user    4m42.928s
sys     0m2.516s

$ time ./tessaccsummary ../imagessan .. san png
aanagarishreel3skttext: 49.88%
arialunicodeskttext: 46.70%
janasanskrittext: 41.27%
kalimatiskttext: 66.27%
mangalskttext: 29.72%
sanskrit2003skttext: 63.68%
shreeskttext: 52.36%
surekhskttext: 23.11%
yogeshskttext: 59.20%
average: 48.02%

real    42m7.727s
user    4m42.928s
sys     0m2.516s
```
