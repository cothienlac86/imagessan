# imagessan
Images and Ground Truth files in Sanskrit along with OCR results 
for Tesseract OCR evaluation fro Sanskrit language (Devanagari script)

## OCR Evaluation Tools for Character & Word Accuracy
was done using tools at https://github.com/Shreeshrii/ocr-evaluation-tools

* Changed tessaccsummary to use -psm 6

### OCR evaluation results using Traineddaata from the Tesseract project 
from https://github.com/tesseract-ocr/tessdata

* Hindi traineddata with CUBE (ocr-hin)
* Sanskrit Traineddata without CUBE (ocr-san)

### OCR evaluation using experimental Traineddata built with tesstrain.sh
Mutiple versions using different fonts, training texts, unicharambigs,exposure levels etc.

#### Box/Tiff pairs for Sanskrit (Devanagri) along with other required input files
(trainingdata-s21 and trainingdata-s95 folders)

#### traineddata files for Sanskrit (devanagari)
(tessdata folder has the traineddata files for s000, s21, s22, s30, s34 and s95)

#### OCR evaluation with different sets of input
(ocr-s21, ocr-s22, ocr-s30, ocr-s34, ocr-s95 folders have the accuracy results and reports)

### Different variations used while training using tesstrain.sh

* Remove fonts with incorrect rendering for Sanskrit eg. Sarai, Eczar, Rhodium Libre
* Removed fancy and old style fonts eg. Aparajita, Santipur OT etc.
* Remove Italic versions of fonts (Utsaah and Kokila)
* Used -1, 0, 1 exposure levels - gives thick, normal and thin variants of font
* Degradation is on by default - lines slope up and down on diff pages
* Removed orthographic syllables frequency list (sanskritweb) from training text
* Added more samples of characters ending in viraam 
* Added list of sanskrit ligatures (TITUS) to training text
* Add optional unicharambigs substitutions (one way only) - ma for bha, gha for dha etc


