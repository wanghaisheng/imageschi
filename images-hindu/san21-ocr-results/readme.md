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

===
```
$ time ./tessaccsummary  ../imagesslipi .. s21 tif
p001: 84.22%
p002: 84.30%
p003: 83.55%
p004: 83.26%
p005: 83.03%
p006: 81.21%
p007: 79.54%
p008: 81.88%
p009: 80.51%
p010: 86.64%
p011: 85.09%
p012: 82.49%
p013: 78.81%
p014: 75.91%
p015: 84.00%
average: 82.30%

real    7m7.169s
user    6m51.328s
sys     0m5.192s
```
