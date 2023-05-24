# ZUMNLP

Jako dataset przyjęty został zestaw danych zawierający artykuły, w którym wydźwięk autora na temat opisywanej osoby/tematu jest pozytywny, negatywny, bądź neutralny.
Dane pobierane są z repozytorium github za pośrednictwem url. Plik .csv został załączony do tego repo pokazowo.

Etapy znajdują sie w oddzielnych plikach. Dołączam również bezpośrednie linki do notebooków:

Etap2: https://colab.research.google.com/drive/1ClleW7d7mQiKVz7mc3-KendJsWguzvxf#scrollTo=Ny_JY0E6PJ_q

Etap3: https://colab.research.google.com/drive/1XYMOLt-o6TCxmdg9iArPe4oamxeEhdNA#scrollTo=iLp3B1lazjQr

Etap4: https://colab.research.google.com/drive/1gIJYazAcY7OY0YGTUJa5FV2MGG4aLSzV#scrollTo=X5Aphg6rSInA

W etapie 2 wybrane modele: Bernoulli Naive Bayes, SVC, Logistic Regression 

W etapie 3 wykorzystano sieć keras z dodatkową wektoryzacją z użyciem Glove. Fine-tuning został wykonany przy użyciu callbacks (ModelCheckpoint oraz EarlyStopping) z dodatkowym mrożeniem trenowania początkowych warstw modelu.

W etapie 4 użyto SiEBERT (English-Language Sentiment Classification) https://huggingface.co/siebert/sentiment-roberta-large-english

Ze względu na brak modeli uwzględniających sentyment neutralny, przyjęto wartości tylko pozytywne(positive i neutral) i negatywne.

Wyniki zapewne byłyby lepsze gdyby zestaw danych był trochę większy, zainteresował mnie on jednak ze względu na dużą ilość tekstu do ogólnego przewidzenia sentymentu. Zestaw miał przypisane sentymenty zarówno do całego dokumentu jak i poszczególnych paragrafów, ale w projekcie używałam całego tekstu by sama dokonać podziałów itp. 
