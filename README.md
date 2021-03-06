# imagessan
Images and Ground Truth text files in Sanskrit 
for evaluating Tesseract OCR (3.04) for Sanskrit language (Devanagari script)
are in the main folder.

Subfolders have additional results of the evaluation.

## OCR Evaluation Tools for Character & Word Accuracy
OCR evaluation was done using tools at https://github.com/Shreeshrii/ocr-evaluation-tools
* Changed tessaccsummary to use -psm 6

### OCR evaluation results using Traineddaata from the Tesseract project 

* Traineddata taken from https://github.com/tesseract-ocr/tessdata
* Hindi traineddata with CUBE v 3.02 (results in ocr-hin folder)
* Sanskrit Traineddata without CUBE v 3.04 (results in ocr-san folder)

### OCR evaluation using experimental Traineddata built by shreeshrii using tesstrain.sh
Mutiple versions of traineddata were created using different fonts, training texts, unicharambigs,exposure levels etc.

#### Different variations used while training using tesstrain.sh

* Removed fonts with incorrect rendering for Sanskrit eg. Sarai, Eczar, Rhodium Libre
* Removed fancy and old style fonts eg. Aparajita, Santipur OT etc.
* Remove Italic versions of fonts (Utsaah and Kokila)
* Used -1, 0, 1 exposure levels - gives thick, normal and thin variants of font
* Degradation is on by default - lines slope up and down on diff pages
* Removed orthographic syllables frequency list (sanskritweb) from training text
* Added more samples of characters ending in viraam 
* Added list of sanskrit ligatures (TITUS) to training text
* Add optional unicharambigs substitutions (one way only) - ma for bha, gha for dha etc

#### Sample Box/Tiff pairs for Sanskrit (Devanagri) along with other required input files
(trainingdata-s21 and trainingdata-s95 folders)

#### traineddata files for Sanskrit (devanagari)
(generated traineddata files for s000, s21, s22, s30, s34 and s95 are in tessdata folder)

#### OCR evaluation with different sets of input
(ocr-s21, ocr-s22, ocr-s30, ocr-s34, ocr-s95 folders have the accuracy results and reports)

#### Fonts used

* Used a number of Devanagari fonts including many from the Google fonts project

* List of some Devanagari Fonts that were included in training

```
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
