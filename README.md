# Final-Project-DS
### Progetto di scoring del rischio di credito
Immaginiamo di lavorare in una banca. Quando riceviamo una richiesta di prestito, dobbiamo assicurarci che, se concediamo il denaro, il cliente sarà in grado di restituirlo. Ogni richiesta comporta un rischio di insolvenza, ossia di mancata restituzione del denaro.
Vorremmo ridurre al minimo questo rischio: prima di accettare di concedere un prestito, vogliamo assegnare un punteggio al cliente e valutare le probabilità di insolvenza. Se è troppo alta, rifiutiamo la richiesta. Questo processo si chiama "credit risk scoring".
L'apprendimento automatico può essere utilizzato per calcolare il rischio. A tal fine, abbiamo bisogno di un set di dati con prestiti, dove per ogni richiesta sappiamo se è stata rimborsata con successo o meno. Utilizzando questi dati, possiamo costruire un modello per prevedere la probabilità di insolvenza e usarlo per valutare il rischio che i futuri mutuatari non rimborsino il denaro.
Utilizzare l'apprendimento automatico per calcolare il rischio di insolvenza. Il piano per il progetto è il seguente:
•	Per prima cosa, otteniamo i dati ed eseguiamo una pre-elaborazione iniziale.
•	Successivamente, addestriamo un modello ad albero decisionale da Scikit-learn per prevedere la probabilità di default.
•	In seguito, spieghiamo come funzionano gli alberi decisionali e quali sono i parametri del modello e mostriamo come regolare questi parametri per ottenere le migliori prestazioni.
•	Poi combiniamo più alberi decisionali in un unico modello, una foresta casuale. Esaminiamo i suoi parametri e li mettiamo a punto per ottenere le migliori prestazioni predittive.
•	Infine, esploriamo un modo diverso di combinare gli alberi decisionali: il gradient boosting. Utilizziamo XGBoost, una libreria altamente efficiente che implementa il gradient boosting. Addestriamo un modello e ne mettiamo a punto i parametri.
Lo scoring del rischio di credito è un problema di classificazione binaria: l'obiettivo è positivo ("1") se il cliente è inadempiente e negativo ("0") altrimenti. Per valutare la nostra soluzione, utilizzeremo l'AUC (area sotto la curva ROC). L'AUC descrive la capacità del nostro modello di separare i casi positivi da quelli negativi. L'AUC descrive la capacità del nostro modello di separare i casi in positivi e negativi.
