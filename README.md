# imagessan
Images and Ground Truth files in Sanskrit along with OCR results 
for OCR evaluation

#### OCR Evaluation Tools for Character & Word Accuracy
Using https://github.com/Shreeshrii/ocr-evaluation-tools

* Changed tessaccsummary to use -psm 6

#### Using Traineddaata from the Tesseract project 
from https://github.com/tesseract-ocr/tessdata

* Hindi traineddata with CUBE
* Sanskrit Traineddata without CUBE

#### Using experimental Traineddata built with tesstrain.sh

Mutiple versions using different fonts, training texts, unicharambigs etc.

* Removed fancy and old style fonts eg. Aparajita, Santipur OT etc.
* Removed orthographic syllables frequency list (sanskritweb) from training text
* Added more samples of characters ending in viraam 
* Added list of sanskrit ligatures (TITUS) to training text
* Add optional unicharambigs substitutions (one way only) - ma for bha, gha for dha etc


