# Guida GitHub

## Guida brutale per utilizzare GitHub ad un livello *basso*.

Questa non sarà una guida efficiente o al 100% corretta se letta da un informatico puro, ma è stata fatta per avere un riferimento per degli studenti di Fisica che devono fare dei lavori di programmazione in condivisione. Ad esempio dei progetti informatici o lavori di analisi dati di laboratorio. Quindi, come già detto uno studioso o anche un appassionato di informatica potrebbe trovare questa guida sommaria o addirittura sbagliata, ma si vuole solamente fare un utilizzo **base** di *GitHub*.

In questa guida è spiegato come utilizzare *GitHub* insieme a *Visual studio Code* e sfruttanto l'interfaccia grafica del pc, ma è opportuno specificare che esistono altri modi di fare le stesse operazioni (ad esempio usando il terminale o l'applicazione *GitHub Desktop*). Questa guida si basa sui seguenti video tutorial: [Guida 1](https://www.youtube.com/watch?v=kjzp0ok38uo) che è fatto molto bene, oppure [Guida 2](https://www.youtube.com/watch?v=Ghf30bq7854) un pochino più rapida. Se si vogliono vedere i metodi *alterniativi* c'è la seguente guida [Guida alternativa](https://www.youtube.com/watch?v=v_1iqtOnUMg).

## Indice

- [Concetti base](#concetti-base)
- [Cosa installare](#cosa-installare)
- [Come clonare una repository](#come-clonare-una-repository)
- [Lavoriamo](#lavoriamo)
- [Nozioni aggiuntive](#nozioni-aggiuntive)
- [Soluzioni a possibili errori](#soluzioni-a-possibili-errori)


### Concetti base

*GitHub* è un servizio di condivisione online (sostanzialmente un servizio Cloud) utilizzato principalmente da programmatori per vedere, condividere e collaborare a progetti provenienti da tutto il mondo. È il concetto alla base dei progetti Open Source, ossia, c'è un file depositato in un qualche luogo e tutti i programmatori (e non) possono accederci scaricandolo o apportando modifiche al file sorgente. Quindi basandoci su questo discorso è ovvio che servirà qualcuno che possieda effettivamente il progetto originale e che lo carichi su *GitHub*, dovrà inoltre metterlo in condivisione con tutti (progetto **pubblico**) o solamente con un gruppo ristretto (progetto **privato**) in modo da poterci lavorare tutti insieme. Il bello di utilizzare *GitHub* è che non serve scaricare file, copiarli ed incollarli, ma con un semplice comando si possono *clonare* interi progetti sul proprio computer che con ulteriori semplici comandi possono aggiornare ed essere aggiornati rispetto al file originale.

La procedura di lavoro che seguiremo sarà:
1. Qualcuno crea il file sorgente
1. Condivide il progetto con i componenti del gruppo
1. Tutti i componenti *cloneranno* il progetto sul proprio pc
1. Ogni volta che si inizia a lavorare occorre sincronizzare il proprio progetto con quello caricato online (niente panico basta cliccare un icona)
1. Ogni volta che si finisce di lavorare si manda quello che si è fatto al file sorgente (un'altro tasto)


### Cosa installare

Fino a qui bravi tutti, ma abbiamo detto tutto e niente. Ci servono gli strumenti per lavorare. Per prima cosa occorre un posto in cui vedere e mettere i file condivisi, ovvero serve un accounti *GitHub*. Si può crearne uno sul sito [GitHub](github.com). 

Però questo non basta perché dobbiamo mettere in contatto il nostro pc con il servizio. Ora, tralasciando i dettagli tecnici, per poter parlare con i progetti su *GitHub* serve avere *Git* installato sul proprio pc. Scaricarlo da [Git](https://git-scm.com). 

A questo punto siamo felici perchè possiamo mandare e ricevere file, ma ci serve un posto che ci permetta di interagire con GitHub senza dover passare ogni volta dal terminale. *Visual Studio Code* (che è banalmente un editor, esattamente come *CodeBlocks*) permette di modificare progetti di *GitHub* direttamente al suo interno, quindi, occorre installarlo. Prendilo dal seguente link [VS Code](https://code.visualstudio.com/download). 

A questo punto manca un ultimo passaggio per essere pronti e inizare a lavorare. Dire a *Visual Studio* che si ha intenzione di utilizzare *GitHub* al suo interno. Occorre installare un'estensione. Si può scaricare dal seguente link [Estensione](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) oppure si può installare direttamente da *VS Code* andando nella sezione apposita delle estensioni nel menu sulla sinistra (evidenziato dal cerchio rosso) e poi cercare esplicitamente *GitHub Pull requests* e scaricarla.

![Download estensione VS Code](/Immagini_README/Download%20Estensione%20Vs%20Code.jpg)

Per vedere se è installata correttamente dovrebbe comparire il logo di *GitHub* nel menu sulla sinistra. Occorre successivamente fare il login su *VS Code* con l'account di *GitHub*. Basta andare nell'icona in basso a sinistra con l'immagine di un omino e cliccare *login*.

![Download estensione VS Code](/Immagini_README/Logo%20Per%20Fare%20L’accesso%20A%20GitHub%20Su%20VS%20Code.jpg)

Fatto ciò siamo pronti ad iniziare a programmare!!

### Come clonare una repository

Per prima cosa parliamo di come si crea un progetto e come si può avere a disposizione sul proprio computer.

Una **repository** può essere visto come un termine altro per dire *"cartella dove ci metto il mio progetto"* (in questo punto esatto chiedo scusa agli informatici😅). Quindi chiunque voglia utilizzare *GitHub* per un progetto condiviso deve prima creare una **repsitory** dove verranno tenuti tutti i file. Creare una **repository** è relativamente semplice, basta seguire i due passaggi illustrati nel seguente video [Come creare una repository su GitHub](https://www.youtube.com/watch?v=s_EmtWEGK5E). Ovviamente una volta creata vanno controllate le impostazioni della stessa per essere sicuri che persone esterne (oltre al proprietario) possano apportare modifiche ai file contenuti nella repository.

Prima abbiamo detto che una volta conosciuta la repository in cui c'è il progetto a cui dobbiamo lavorare occorre avere effettivamente il file **sul** nostro pc per poter concretamente fare qualcosa. Occorre, quindi, passsare attraverso il processo di **clonazione di una repository**.

> la procedura che si descrive in seguito sfrutta il terminale, ma come già detto si può fare la stessa cosa utilizzando tool diversi (GitHub Desktop).

Una buona pratica è quella di creare una cartella (directory) in cui si andranno a mettere tutti i progetti clonati.

Per prima cosa occorre andare nella pagina web di *GitHub* della repository e cliccare sul bottone verde con la scritta **code** e copiare l'indirizzo *HTTPS* della stessa con l'apposito pulsante.

![clonazione 1](/Immagini_README/clonazione%201.jpg)

Una volta fatto occorre aprire il terminale, spostarsi (con il comando `cd`) nella cartella scelta per i progetti *GitHub*, ed eserguire il seguente comando:

```
git clone <HTTPS della repository>
```

Ora, per controllare che sia tutto corretto basta semplicemente vedere con l'*esplora risorse* che sia comparsa una cartella con il nome della repository dentro la directory scelta per le clonazioni.

### Lavoriamo

Ora che abbiamo clonato la repository con il progetto di interesse sul nostro pc dobbiamo aprirlo per poterci lavorare su. Andare sul menu altro di *VS Code*, cliccare su *Apri cartella* e selezionare quella di interesse.

![lavoro 1](/Immagini_README/Apertura%20Cartella-1.jpg)

A questo punto si dovrebbe avere sul menù di destra tutto il contenuto clonato dalla repository di *GitHub*

![lavoro 1](/Immagini_README/Apertura%20Cartella%202-1.jpg)

Ora finalmente si è pronti a scrivere il codice!!

Immaginate di dover scrivere una macro per fare l'analisi dati di un'esperienza di laboratorio. Un vostro collega ha gia iniziato a scrivere il codice, ma ha fatto un fit indecente e voi volete fare un lavoro fatto bene. Chiedete al vostro collega di mandarvi il link della repository su *GitHub*, la clonate sul vostro pc, la aprite su *VS Code* e cominciate a modificare il programma. Scrivete un codice che vi soddisfa, eseguite un fit perfetto e volete farlo vedere al vostro collega. Gli dite di eseguire lui stesso la macro visto che *GitHub* è un servizio di Cloud e di conseguenza avete tutti i progetti **sincronizzati**. Lo sfortunato collega apre la macro, la esegue,ma non vede cambiamenti rispetto a prima che voi ci metteste mano.

Quello che è saltato in questa storia non troppo inventata (per alcuni) è che non avete **sincronizzato** le vostre modifiche con il progetto principale caricato sul CLoud. Questa operazione per *GitHub* si chiama **push**.

Ripartiamo dall'inizio. Clonate, aprite la repository del vostro collega e fate le modifiche che ritenete necessarie. Ora, dovete condividerle. Dopo aver fatto le modifiche dovete salvare il file, basta fare un `ctrl+s`. Una volta fatto dovrebbe uscire un numero sull'icona nel menù di sinistra.

![lavoro 2](/Immagini_README/Commit-push-1.jpg)

Se lo si apre compare la seguente situazione

![lavoro 3](/Immagini_README/Commit-push%202-1.jpg)

Compare l'elenco dei cambiamenti avvenuti rispetto alla versione del progetto esistente prima delle vostre modifiche. Compare il pulsante **Commit** che è la chiave di questo procedimento e in alto compare la possibilità, in realtà **obbligo** (altrimenti non esegue il comando) di mettere un messaggio di testo usato per descrivere i cambiamenti fatti, cosi da tener traccia del progresso del progetto.

Quindi inseriamo un messaggio di testo e premiamo su **Commit** che sostanzialmente è un'azione che prepara il nostro progetto prima di essere mandato in Cloud. Attenzione, non abbiamo ancora sincronizzato nulla. Una volta fatto il commit ci si ritroverà nella seguente situazione

![lavoro 4](/Immagini_README/Commit-push%203-1.jpg)

Il simbolo comparso al posto di **commit** è il simbolo del **push** che è l'operazione effettiva che *pusha* le nostre modifiche su *GitHub*. Una volta cliccato ritorna tutto vuoto e possiamo chiudere *VS Code* sereni che il nostro collega potrà vedere il codice aggiornato.

Quindi chiudete *VS Code*, spegnete il pc e andate a farvi i fatti vostri per un pomeriggio. Quando sentite il vostro collega il giorno dopo però lui vi dice che non vede ancora i vostri cambiamenti e che il fit è ancora orribile. A questo punto voi potete stare sereni perché avete fatto tutto il dovuto per fornirgli il materiale corretto, ma è lui che prima di iniziare a lavorare dovrebbe aggiornare la sua versione del progetto (che ovviamente ha clonato in locale) rispetto quella presente su *GitHub*. L'operazione che manca al vostro compagno di gruppo si chiama **fetch+pull** e serve sostanzialmente ad aggiornare i file presenti sul computer all'ultima versione presente su *GitHub*. Questa operazione è ovvio farla non appena si apre *VS Code* per lavorare su un progetto *GitHub* ed è banalissima, basta solamente cliccare sul pulsante (la doppia freccia che ruota) apposito in basso a sinistra

![lavoro 5](/Immagini_README/Fetch-pull-1.jpg)

Questo è tutto quello necessario per essere in grado di lavorare in team con altre persone con la comodità di avere un unico progetto condiviso e sincronizzato.

Qui si conclude la guida base.

Doveroso ringraziare uno specifico tutor del corso di *Introduzione alla Fisica Nucleare e Subnucleare* dell'Università degli studi di Torino che ha stimolato il mio gruppo di lavoro ad utilizzare *GitHub*.


## Nozioni aggiuntive

Ovviamente non è stato detto esplicitamente, ma non sempre si conosce il proprietario della repository su cui si lavora; oppure, si trova una repository relativa ad un progetto Open Source e si vuole contribuire. In questi casi il proprietario del progetto molto probabilmente non ha abilitato tutti gli utenti di *GitHub* a modificare il file, ma si può sempre fare una **pull-request**. Vuol dire che si manda una domanda al proprietario della repository di poter fare una specifica modifica. Questo è appunto la base dei progetti Open Source. Sostanzialmente, dopo il commit al posto di fare un push si fa una pull-request ad una repository esterna. Ovviamente il proprietario non è obbligato ad accettare modifiche esterne al suo progetto.

Nel caso in cui non si volesse fare una pull-request ad un progetto si possono comunque fare delle modifiche al progetto, ma al posto di condividerle si può creare un **branch**, ossia una repository parallela, le cui modifiche non intaccano in nessun modo la repository principale. Tendenzialmente questa cosa si fa per progetti molto complicati in cui non si è sicuri delle modifiche che si fanno e per evitare di *"sbagliare"* nella repository principale si creano questi branch dove si è più sicuri nel fare delle prove. Successivamente si possono fare dei **merge-pull-request** per unire i diversi branch in uno unico.

## Soluzioni a possibili errori

1. Se si sta lavorando su delle macro `root` non so bene il perché, ma non si riescono ad eseguire direttamente dal terminale presente in *VS Code*, ma bisogna eseguirle con il terminale esterno del pc.

1. Potrebbe capitare che due componenti dello stesso gruppo modifichino una stessa repository in intervalli di tempo sovrapposti. Quindi, capita che mentre si fa un push si debba fare anche un pull delle modifiche fatte da altri. In questa situazione *VS Code* non capisce più nulla e da errore bloccando tutto. Quello che si deve fare è inserire il seguente comando nel terminale

```
git config --global pull.rebase false
```

1. Se si utilizza un Mac e si prova ad eseguire un file C++ (potrebbe capitare anche per altri linguaggi, ma io ho riscontrato il problema per questo linguaggio specifico) *VS Code* potrebbe non riuscire ad eseguirlo. Occorre aprire un terminale direttamente in *VS Code* (basta farlo nel menù in alto) ed eseguire i seguenti comandi

```
g++ -o <dare un nome al progetto> main.cpp ...
```

dove i puntini di sospensione stanno a significare che si devono mettere i nomi di tutti i file cpp che vengono richiamati nel main.cpp (i file header non devono essere messi). Il nome al progetto (i "< >" non vanno messi) serve darlo solo per dare un'indicazione a *VS Code* di cosa dovrà eseguire. Successivamente si può eseguire

```
./<nome dato al progetto>
```

che eseguirà il programma.
