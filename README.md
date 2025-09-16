# Childhood as it appears in the Iranian Press

As part of a study on the history of children and childhood in modern Iran, this project aims to create a database of Iranian newspapers from the late 19th and early 20th centuries, to train an OCR model able to read Persian, and locate and augment the references to children and childhood in this corpus.

Escriptorium Tools:

1. Colab Tutorial of Prof. Daniel Stockl: https://colab.research.google.com/drive/1hyBDa55mPolZve4Ih1qpXd94i6f8Xno-
2. Additional functions: https://colab.research.google.com/drive/1\_NXUDOfe2i42G7EwEUHkkhbYFd7TbaP9



Kraken training commands:

1. OCR train command: ketos train -f binary -d cuda:0 -r 0.0001 --resize both -i persian\_best.mlmodel -o second\_model dataset.arrow



2\. Region model train command: ketos segtrain -d cuda:0 -f xml -t C:\\Users\\User\\PycharmProjects\\PersianChildhood\\output\_alto.txt  --suppress-baselines --resize both -i blla.mlmodel -o Models/region\_model\_11\_10\_24 -q fixed -N 100

