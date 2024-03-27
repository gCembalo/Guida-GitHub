# Guida GitHub

## Guida brutale per utilizzare GitHub ad un livello basso.

Questa non sarà una guida efficiente o al 100% corretta se letta da un informatico puro, ma è stata fatta per avere un riferimento per degli studenti di Fisica che devono fare dei lavori di programmazione in condivisione. Ad esempio dei progetti informatici o lavori di analisi dati di laboratorio. Quindi, come già detto uno studioso o anche un appassionato di informatica potrebbe trovare questa guida come sommaria o addirittura sbagliata, ma si vuole solamente fare un utilizzo **base** di *GitHub*.

In questa guida è spiegato come utilizzare *GitHub* insieme a *Visual studio Code* e sfruttanto l'interfaccia grafica del pc, ma è opportuno specificare che esistono altri modi di fare le stesse operazioni (ad esempio usando il terminale o l'applicazione *GitHub Desktop*). Questa guida si basa sui seguenti video tutorial: [Guida 1](https://www.youtube.com/watch?v=kjzp0ok38uo) che è fatto molto bene, oppure [Guida 2](https://www.youtube.com/watch?v=Ghf30bq7854) un pochino più rapida. Se si vogliono vedere i metodi *alterniativi* c'è la seguente guida [Guida alternativa](https://www.youtube.com/watch?v=v_1iqtOnUMg).


### Concetti base

*GitHub* è un servizio di condivisione online (sostanzialmente un servizio Cloud) utilizzato principalmente da programmatori per vedere, condividere e collaborare a progetti provenienti da tutto il mondo. È il concetto alla base dei progetti Open Source, ossia, c'è un file depositato in un qualche luogo e tutti i programmatori (e non) possono accederci scaricandolo o apportando modifiche al file sorgente. Quindi basandoci su questo discorso è ovvio che servirà qualcuno che possieda effettivamente il progetto originale, che dovrà caricare su *GitHub* messo in condivisione con tutti (progetto **pubblico**) o solamente con un gruppo ristretto (progetto **privato**), cosi da poterci lavorare tutti insieme. Il bello di utilizzare *GitHub* è che non serve scaricare file, copiare ed incollare, ma con un semplice comando si possono *clonare* interi progetti sul proprio computer che con semplici comandi aggiornano e possono essere aggiornati rispetto al file originale.

La procedura di lavoro che seguiremo sarà:
1. Qualcuno crea il file sorgente
1. Condivide il progetto con i componenti del gruppo
1. Tutti i componenti *cloneranno* il progetto sul proprio pc
1. Ogni volta che si inizia a lavorare occorre sincronizzare il proprio progetto con quello caricato online (niente panico basta cliccare un icona)
1. Ogni volta che si finisce di lavorare si manda quello che si è fatto al file sorgente (un'altro tasto)


### Cosa installare

Fino a qui bravi tutti, ma abbiamo detto tutto e niente. Ci servono gli strumenti per lavorare. Per prima cosa occorre un posto in cui vedere e mettere i file condivisi, ovvero serve un accounti *GitHub*. Si può crearne uno sul sito [GitHub](github.com). 

Però questo non basta perché dobbiamo mettere in contatto il nostro pc con il servizio. Ora, tralasciando i dettagli tecnici, per poter parlare con i progetti su *GitHub* serve avere *Git* installato sul proprio pc. Scaricarlo da [Git](https://git-scm.com). 

A questo punto siamo felici perchè possiamo mandare e ricevere file, ma ci serve un posto che capisca il modo di interagire con noi di GitHub senza dover passare ogni volta dal terminale. *Visual Studio Code* (che è banalmente un editor, esattamente come *CodeBlocks*) permette di modificare progetti di *GitHub* direttamente al suo interno, quindi, occorre installarlo. Prendilo dal seguente link [VS Code](https://code.visualstudio.com/download). 

A questo punto manca un ultimo passaggio per essere pronti e inizare a lavorare. Dire a *Visual Studio* che si ha intenzione di utilizzare *GitHub* al suo interno. Occorre installare un'estensione. Si può scaricare dal seguente link [Estensione](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) oppure si può installare direttamente da *VS Code* andando nella sezione apposita delle estensioni nel menu sulla sinistra (evidenziato dal cerchio rosso) e poi cercare esplicitamente *GitHub Pull requests* e scaricarla.

![Download estensione VS Code](/Immagini_README/Download%20Estensione%20Vs%20Code.jpg)

Per vedere se è installata correttamente dovrebbe comparire il logo di *GitHub* nel menu sulla sinistra. Occorre successivamente fare il login su *VS Code* con l'account di *GitHub*. Basta andare nell'icona in basso a sinistra con l'immagine di un omino e cliccare *login*.

![Download estensione VS Code](/Immagini_README/Logo%20Per%20Fare%20L’accesso%20A%20GitHub%20Su%20VS%20Code.jpg)

Fatto ciò siamo pronti ad iniziare a programmare!!

### Come si utilizzano gli strumenti

Per prima cosa parliamo di come si crea un progetto e come si può avere a disposizione sul proprio computer.

Una **repository** può essere visto come un termine altro per dire *cartella dove ci metto il mio progetto* (in questo punto esatto chiedo scusa agli informatici😅).