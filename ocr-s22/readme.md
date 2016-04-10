OCRed Using s22 Sanskrit traineddata 
===
created using tesstrain.sh without shape-clustering

with current 3.05-dev source

```
Following Devanagari Fonts were included in training

DEVANAGARI_FONTS=( \
    "AA_NAGARI_SHREE_L3" \
    "Aksharyogini2" \
    "Annapurna SIL" \
    "Asar" \
    "CDAC-GISTSurekh" \
    "CDAC-GISTYogesh" \
    "Chandas" \
    "Eczar" \
    "Ek Mukta" \
    "FreeSerif" \
    "Glegoo" \
    "Kalimati" \
    "Khula" \
    "Kokila Italic" \
    "Kokila" \
    "Lohit Devanagari" \
    "Madan2" \
    "Mangal" \
    "Martel" \
    "Nirmala UI" \
    "Noto Sans Devanagari" \
    "SHREE-DV0726-OT" \
    "Sahitya" \
    "Samanata" \
    "Sanskrit 2003," \
    "Sanskrit Text" \
    "Sarai" \
    "Siddhanta" \
    "Sumana" \
    "Utsaah Italic" \
    "Utsaah" \
    "Uttara" \
    "Vesper Libre" \
    "gargi Medium" \
    )
  ```  

Shreelipi accuracy is higher for s21

s22 with 600x600 tifs

```
$ time ./tessaccsummary  ../imagesslipi .. s22 tif
p001: 79.78%
p002: 80.67%
p003: 77.02%
p004: 80.75%
p005: 79.66%
p006: 77.66%
p007: 80.64%
p008: 80.31%
p009: 76.74%
p010: 82.11%
p011: 80.28%
p012: 81.03%
p013: 76.19%
p014: 71.36%
p015: 81.17%
average: 79.02%

real    8m46.651s
user    7m42.039s
sys     0m6.115s
```
s22 with 400x400 png files - recognition is better
```
$ time ./tessaccsummary  ../imagesslipi .. s22 png
p001: 82.78%
p002: 83.09%
p003: 82.03%
p004: 83.37%
p005: 80.67%
p006: 80.64%
p007: 82.73%
p008: 84.23%
p009: 83.94%
p010: 86.06%
p011: 84.06%
p012: 84.38%
p013: 80.32%
p014: 76.70%
p015: 83.37%
average: 82.56%

real    6m43.904s
user    6m25.136s
sys     0m6.996s
```
