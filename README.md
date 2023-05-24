# ZUMNLP

Jako dataset przyjęty został zestaw danych zawierający artykuły, w którym wydźwięk autora na temat opisywanej osoby/tematu jest pozytywny, negatywny, bądź neutralny.
Dane pobierane są z repozytorium github za pośrednictwem url. Plik .csv został załączony do tego repo pokazowo.

Etapy znajdują sie w oddzielnych plikach. Dołączam również bezpośrednie linki do notebooków:

Etap2: https://colab.research.google.com/drive/1ClleW7d7mQiKVz7mc3-KendJsWguzvxf#scrollTo=Ny_JY0E6PJ_q

Etap3: https://colab.research.google.com/drive/1XYMOLt-o6TCxmdg9iArPe4oamxeEhdNA#scrollTo=iLp3B1lazjQr

Etap4:

W etapie 2 wybrane modele: Bernoulli Naive Bayes, SVC, Logistic Regression 

W etapie 3 wykorzystano sieć keras z dodatkową wektoryzacją z użyciem Glove. Fine-tuning został wykonany przy użyciu callbacks (ModelCheckpoint oraz EarlyStopping) z dodatkowym mrożeniem trenowania początkowych warstw modelu.

W etapie 4 użyto BERT
