OCRed with hin.traineddata 3.02 release
https://github.com/tesseract-ocr/tessdata/blob/master/hin.traineddata
and other hin.* cube files from https://github.com/tesseract-ocr/tessdata/
===
Hindi traineddata with CUBE

Character and Word Accuracy Reports
```
$ time ./tessaccsummary ../imagesBIG .. hin tif
Sahadeva: 82.03%
Siddhanta: 83.08%
average: 82.56%

real    62m46.753s
user    52m19.393s
sys     9m35.295s

$ time ./tessaccsummary -w ../imagesBIG .. hin tif
Sahadeva: 51.09%
Siddhanta: 53.96%
average: 52.53%

real    106m15.490s
user    74m20.393s
sys     15m56.727s
```

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
