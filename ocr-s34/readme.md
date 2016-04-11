```
$  time ./tessaccsummary  ../imagesslipi .. s34 png
p001: 83.22%
p002: 82.48%
p003: 85.40%
p004: 84.40%
p005: 86.29%
p006: 84.31%
p007: 84.27%
p008: 84.45%
p009: 84.05%
p010: 85.48%
p011: 86.47%
p012: 86.79%
p013: 82.44%
p014: 79.89%
p015: 85.98%
average: 84.39%

real    3m48.776s
user    3m39.822s
sys     0m4.931s
```

```
$  time ./tessaccsummary  ../imagessan .. s34 png
aanagarishreel3skttext: 84.20%
arialunicodeskttext: 88.44%
janasanskrittext: 54.48%
kalimatiskttext: 89.74%
mangalskttext: 56.49%
sanskrit2003skttext: 86.67%
shreeskttext: 57.43%
surekhskttext: 89.03%
yogeshskttext: 85.97%
average: 76.94%

real    1m54.389s
user    1m49.167s
sys     0m2.723s
```

```
$  time ./tessaccsummary  ../imagesBIG .. s34 tif
Sahadeva: 91.46%
Siddhanta: 94.86%
average: 93.16%

real    10m4.135s
user    10m2.272s
sys     0m1.250s

$  time ./tessaccsummary -w  ../imagesBIG .. s34 tif
Sahadeva: 68.17%
Siddhanta: 80.45%
average: 74.31%

real    10m7.483s
user    10m4.631s
sys     0m1.030s
```
