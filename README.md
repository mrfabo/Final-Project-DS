# Final-Project-DS
### Progetto di scoring del rischio di credito
Quando riceviamo una richiesta di prestito dobbiamo assicurarci che, se concediamo il denaro, il cliente sarà in grado di restituirlo. Ogni richiesta comporta un rischio di insolvenza ossia di mancata restituzione del denaro.
Vorremmo ridurre al minimo questo rischio: prima di accettare di concedere un prestito vogliamo assegnare un punteggio al cliente e valutare le probabilità di insolvenza. Se è troppo alta, rifiutiamo la richiesta, questo processo si chiama "credit risk scoring".
L'apprendimento automatico può essere utilizzato per calcolare il rischio, a tal fine, abbiamo bisogno di un set di dati con prestiti, dove per ogni richiesta sappiamo se è stata rimborsata con successo o meno. Utilizzando questi dati possiamo costruire un modello per prevedere la probabilità di insolvenza e usarlo per valutare il rischio che i futuri mutuatari non rimborsino il denaro.
Il piano per il progetto è il seguente:
* Per prima cosa, ottenere i dati ed eseguiamo una pre-elaborazione iniziale.
* Successivamente, addestrare un modello ad albero decisionale da Scikit-learn per prevedere la probabilità di default.
* stabilire quali sono i parametri del modello e regolare questi parametri per ottenere le migliori prestazioni.
* combinare più alberi decisionali in un unico modello, random forest. Esamine i parametri e metterli a punto per ottenere le migliori prestazioni predittive.
* Utilizzare XGBoost e mettere a punto i parametri.

Lo scoring del rischio di credito è un problema di classificazione binaria: l'obiettivo è positivo ("1") se il cliente è inadempiente e negativo ("0") altrimenti. Per valutare la soluzione, utilizzeremo l'AUC (area sotto la curva ROC). L'AUC descrive la capacità del modello di separare i casi positivi da quelli negativi.


Per vedere il progetto apire il file Progetto scoring rischio di credito.ipynb
