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

