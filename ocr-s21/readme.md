s21
===

OCRed text and character accuracy and word accuracy reports 

using sanskrit traineddata created using 
tesstrain.sh automated training process 

```
ocrevalutf8 wordacc ground.txt ocr.txt | awk '$3 != 100 {print $0}' > results.txt 
ocrevalutf8 accuracy ground.txt ocr.txt | awk '$3 != 100 {print $0}' > results.txt 
```
The accuracy reports do not include the 100% correct items to reduce size of report
