OCRed with hin.traineddata 3.02 release
===
```
$ time ./tessaccsummary ../imagesBIG .. hin tif
Sahadeva: 82.03%
Siddhanta: 83.08%
average: 82.56%

real    62m46.753s
user    52m19.393s
sys     9m35.295s
```
Hindi traineddata with CUBE
```
$ time ./tessaccsummary ../imagessan .. hin png
aanagarishreel3skttext: 79.48%
arialunicodeskttext: 76.18%
janasanskrittext: 59.08%
kalimatiskttext: 81.72%
mangalskttext: 62.26%
sanskrit2003skttext: 78.54%
shreeskttext: 57.43%
surekhskttext: 73.00%
yogeshskttext: 79.36%
average: 71.89%

real    3m59.359s
user    3m27.654s
sys     0m28.844s
```
