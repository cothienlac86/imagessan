# imagessan
Images and Ground Truth files in Sanskrit for OCR evaluation

## OCR Evaluation - Character Accuracy
Using https://github.com/Shreeshrii/ocr-evaluation-tools

#### Using Traineddaata from the Tesseract project 
from https://github.com/tesseract-ocr/tessdata

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

Sanskrit Traineddata without CUBE

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
```

#### Using Traineddata built with tesstrain.sh

```
$  time ./tessaccsummary  ../imagessan .. s22  tif
aanagarishreel3skttext: 86.67%
arialunicodeskttext: 84.67%
janasanskrittext: 69.93%
kalimatiskttext: 89.03%
mangalskttext: 68.40%
sanskrit2003skttext: 87.50%
shreeskttext: 80.31%
surekhskttext: 90.21%
yogeshskttext: 89.50%
average: 82.91%

real    3m49.120s
user    3m43.497s
sys     0m2.964s
```

## OCR Evaluation - Word Accuracy
Using https://github.com/Shreeshrii/ocr-evaluation-tools

#### Using Traineddaata from the Tesseract project 
from https://github.com/tesseract-ocr/tessdata

Hindi Traineddata with CUBE

```
$ time ./tessaccsummary -w ../imagessan .. hin  png
aanagarishreel3skttext: 46.51%
arialunicodeskttext: 43.02%
janasanskrittext: 13.95%
kalimatiskttext: 53.49%
mangalskttext: 22.09%
sanskrit2003skttext: 40.70%
shreeskttext: 23.26%
surekhskttext: 39.53%
yogeshskttext: 48.84%
average: 36.82%

real    32m27.702s
user    6m41.451s
sys     1m9.053s
```

Sanskrit Traineddata without CUBE
```
$ time ./tessaccsummary -w ../imagessan .. san png
aanagarishreel3skttext: 5.81%
arialunicodeskttext: 2.33%
janasanskrittext: 1.16%
kalimatiskttext: 8.14%
mangalskttext: 5.81%
sanskrit2003skttext: 5.81%
shreeskttext: 6.98%
surekhskttext: 3.49%
yogeshskttext: 5.81%
average: 5.04%

real    11m3.498s
user    7m58.471s
sys     0m2.837s
```

#### Using Traineddata built with tesstrain.sh

```
$  time ./tessaccsummary -w ../imagessan .. s22  tif
aanagarishreel3skttext: 54.65%
arialunicodeskttext: 58.14%
janasanskrittext: 39.53%
kalimatiskttext: 69.77%
mangalskttext: 31.40%
sanskrit2003skttext: 55.81%
shreeskttext: 53.49%
surekhskttext: 66.28%
yogeshskttext: 72.09%
average: 55.68%

real    3m46.474s
user    3m39.431s
sys     0m2.807s
```
