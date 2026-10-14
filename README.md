# proiect-1-ml

Pasul 1 - Explorarea datelor
Dimensiune (7043), Valori lipsa (11), distributie tinta (churn), 3 Grafice
Explicatii: Este vorba despre o clasificare; se observa din grafic ca exista o proportionalitate intre durata contractului si retinerea clientilor; greseala mai scumpa este in cazul in care modelul atribuie cuiva care pleaca faptul ca ar fi ramas, si ar fi un client pierdut.

Pasul 2 - Pregatirea datelor
Impartirea pe train si test: datele de testare pentru model, pe care nu le-a mai intalnit.

Pasul 3 - Baseline
Ne arata ce scor am obtine pe un model daca nu il invatam nimic. S-a obtinut 0.73 accuracy.

Pasul 4 - 2 modele
Logistic regression: accuracy 81% / recall 56%
Random forest: accuracy 79% / recall 51%
Imbunatatire la recall.

Pasul 5 - Evaluare set de date
Este important ce se intampla la recall, asta merita imbunatatit, pentru ca acolo exista un cost mai mare la pierderea clientilor.

Pasul 6 - Concluzie
Class_weight="balanced" - am spus modelului ca este un cost mai mare cu un client care pleaca (logistic regression imbunatatit)
GridSearchCV - era important ca modelul sa nu memoreze (overfitting).
