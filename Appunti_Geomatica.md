# DISPENSA COMPLETA DI GEOMATICA

## 01. INTRODUZIONE

### Definizione di Geomatica

La Geomatica (nota anche come tecnologia geospaziale) è la disciplina che si occupa della raccolta, memorizzazione, elaborazione e distribuzione di informazioni geografiche, o informazioni riferite spazialmente.

La Geomatica è un termine scientifico relativamente nuovo, coniato da Pollock e Wright nel 1969, con l'intenzione di combinare i termini geodesia e geoinformatica. Include gli strumenti e le tecniche utilizzate in:
- Rilevamento topografico
- Telerilevamento
- Cartografia
- Sistemi Informativi Geografici (GIS)
- Sistemi globali di navigazione satellitare (GPS, GLONASS, Galileo, Compass)
- Fotogrammetria
- Geografia e forme correlate di mappatura terrestre

<div style="page-break-after: always;"></div>

### Struttura del corso

#### 01. Introduzione
- 01.01 Elementi di cartografia
- 01.02 Telerilevamento: fotografia aerea
- 01.03 Telerilevamento: immagini satellitari

#### 02. Acquisizione dati telerilevati
- 02.01 LIDAR: laser scanner terrestre
- 02.02 LIDAR aereo
- 02.03 I droni per il rilievo di informazioni territoriali

#### 03. Sistemi Informativi Geografici
- 03.01 Cartografia digitale e banche dati territoriali
- 03.02 Formati dei file, georeferenziazione, features
- 03.03 GIS open source (Quantum GIS)

#### 04. Sistemi di Posizionamento Globale (GPS)
- 04.01 Storia dei diversi sistemi
- 04.02 I segmenti e la trilaterazione
- 04.03 Precisione, accuratezza, errori e correzioni

#### 05. Rilevamento digitale
- 05.01 Mobile GIS
- 05.02 Tablet PC
- 05.03 GPS per il mobile GIS

#### 06. Modellazione multidimensionale
- 06.01 Cartografia e sezioni geologiche (2D)
- 06.02 DEM e DTM (2.5D)
- 06.03 Modelli 3D e n-dimensionali

### Struttura delle lezioni
- Lezioni canoniche
- Workshop al chiuso
- Workshop all'aperto: lavoro sul campo
- Esami

<div style="page-break-after: always;"></div>

## 01.01 FONDAMENTI DI CARTOGRAFIA

### Definizione di Cartografia

La cartografia (dal greco Χάρτης, khartes = papiro (carta) e graphein = scrivere) è lo studio e la pratica di creare mappe. Combinando scienza, estetica e tecnica, la cartografia si basa sul presupposto che la realtà possa essere modellata in modi che comunicano efficacemente informazioni spaziali.

### Scala della Mappa

Una mappa rappresenta una porzione della superficie terrestre. Poiché una mappa accurata rappresenta il territorio, ogni mappa ha una "scala" che indica la relazione tra una certa distanza sulla mappa e la distanza sul terreno.

#### Frazione Rappresentativa (RF)
Indica quante unità sulla superficie terrestre equivalgono a un'unità sulla mappa. Può essere espressa come 1/100.000 o 1:100.000. In questo esempio, un centimetro sulla mappa equivale a 100.000 centimetri (1 chilometro) sulla terra.

#### Scala Grafica
È semplicemente una linea segnata con la distanza sul terreno.

#### Grande scala o piccola scala
Una mappa a grande scala si riferisce a una che mostra maggiori dettagli perché la frazione rappresentativa (ad es. 1/25.000) è una frazione più grande rispetto a una mappa a piccola scala che avrebbe una RF di 1/250.000 a 1/7.500.000. Le mappe a grande scala avranno una RF di 1:50.000 o superiore (cioè 1:10.000). Quelle tra 1:50.000 e 1:250.000 sono mappe a scala intermedia.

- 1:25.000 (es. IGMI)
- 1:10.000 (es. CTR regionale)

### Proiezioni

- Una proiezione cartografica è qualsiasi metodo per rappresentare la superficie di una sfera o di un altro corpo tridimensionale su un piano.
- Tutte le proiezioni cartografiche distorcono la superficie in qualche modo. A seconda dello scopo della mappa, alcune distorsioni sono accettabili e altre no; quindi esistono diverse proiezioni cartografiche per preservare alcune proprietà del corpo simile a una sfera a scapito di altre proprietà.
- Non c'è limite al numero di possibili proiezioni cartografiche.

Molte proprietà possono essere misurate sulla superficie terrestre:
- Area
- Forma
- Direzione
- Angoli
- Distanza

Le proiezioni cartografiche possono essere costruite per preservare una o più di queste proprietà, anche se non tutte simultaneamente. Lo scopo della mappa determina quale proiezione dovrebbe costituire la base per la mappa.

#### Tipi di proiezioni
- **Conformi**: preservano gli angoli localmente (es. UTM: Universal Transversal Mercator)
- **Equivalenti**: preservano l'area (es. Lambert)
- **Equidistanti**: preservano la distanza da un punto o linea standard

### Coordinate

#### Latitudine
(abbreviazione: Lat., φ, o phi) di un punto sulla superficie terrestre è l'angolo tra il piano equatoriale e una linea che passa attraverso quel punto ed è normale alla superficie di un ellissoide di riferimento che approssima la forma della Terra.

#### Longitudine
(abbreviazione: Long., λ, o lambda) di un punto sulla superficie terrestre è l'angolo est o ovest da un meridiano di riferimento a un altro meridiano che passa attraverso quel punto.

### Sistema di Riferimento delle Coordinate (CRS)

Un CRS è un sistema di coordinate basato su base locale, regionale o globale utilizzato per localizzare entità geografiche. I CRS possono essere referenziati utilizzando i codici EPSG definiti dall'European Petroleum Survey Group.

#### Sistema di Riferimento delle Coordinate in Italia

**Gauss-Boaga** è stato proposto dal prof. Giovanni Boaga - Capo dell'Istituto Geografico Militare - nel 1940. Il sistema Gauss-Boaga definisce anche il sistema geodetico Roma 40. La mappa IGM alla scala 1:25.000 è stata pubblicata in coordinate Gauss-Boaga, poi trasformate in UTM.

Sono coordinate metriche che esprimono un punto come distanza dal vertice geodetico di Monte Mario. Le 2 zone principali sono chiamate fuso Ovest e fuso Est.

L'evoluzione della cartografia italiana ha adottato il sistema di coordinate UTM.

- Gauss-Boaga EPSG 3003 (fuso Ovest)
- Gauss-Boaga EPSG 3004 (fuso Est)

**Universal Transverse Mercator (UTM)** è un sistema di coordinate geografiche che utilizza un sistema di coordinate cartesiane bidimensionale per fornire posizioni sulla superficie terrestre. Il sistema UTM divide la Terra in sessanta zone, ciascuna una fascia di longitudine di sei gradi, e utilizza una proiezione trasversa di Mercatore secante in ciascuna zona. L'Italia è compresa in due fasce principali UTM 32 e UTM 33 (+34).

**World Geodetic System WGS 84** è il sistema di coordinate di riferimento utilizzato dal Global Positioning System.

### Simbologia

- **Orografia**: Isoipse e punti con altimetria. Alla scala 1:25.000 le curve di livello hanno equidistanza 25 m. Alla scala 1:10.000 le curve di livello hanno equidistanza 10 m.
- **Idrografia**: Fiumi, torrenti, sorgenti, laghi, mare, ecc.
- **Amministrazione**: Confini di Stato, Regione, Provincia, Comune.
- **Urbano**: Edifici e così via.
- **Strade**: Autostrade, ferrovie, ponti, sentieri...
- **Vegetazione**: Vari tipi di alberi rappresentati con simboli specifici.
- **Geodetici**: Punti di riferimento geodetici.

### Leggere una Mappa

#### Primo passo
- Posizione geografica dell'area di studio
- Scala e dimensioni
- Equidistanza delle curve di livello

#### Secondo passo
- Prima definizione dei principali elementi orografici
- Pendenza
- Interpretazione analitica di orografia e idrografia
- Affioramenti rocciosi
- Idrologia e i suoi modelli
- Tipi di vegetazione
- Caratteristiche antropiche

#### Terzo passo
- Interpretazione della forma e dei processi
- Geomorfologia
- Attività umane
- Caratteristiche seminaturali
- Confronto con altri fonti: mappe tematiche, dati statistici, bibliografia, ...

<div style="page-break-after: always;"></div>

## 01.02 TELERILEVAMENTO: FOTOGRAFIA AEREA

### Definizione

Il Telerilevamento in generale può essere definito come la raccolta di informazioni da un oggetto o superficie senza contatto diretto. Il telerilevamento (Look-Look, No Touch) è un campo molto più ampio di quello che verrà discusso in queste lezioni. Ci concentreremo sulla parte del telerilevamento che si occupa delle SCIENZE DELLA TERRA E AMBIENTALI.

### Storia

- 1858: Il pallonista G. Tournachon fece fotografie di Parigi dal suo pallone.
- La fotografia aerea sistematica si sviluppò per scopi militari e di ricognizione a partire dalla Prima Guerra Mondiale, raggiungendo il culmine durante la Guerra Fredda.
- I satelliti artificiali nella seconda metà del XX secolo.

### Telerilevamento Attivo vs Passivo

- **Passivo**: RS che utilizza la radiazione solare riflessa; RS che utilizza la radiazione emessa dagli oggetti.
- **Attivo**: Il sensore emette la propria energia e registra la risposta (es. RADAR, LIDAR).

### Elementi di Interpretazione delle Immagini

#### Forma
Molte caratteristiche naturali e artificiali hanno forme uniche. Vengono spesso utilizzati aggettivi come lineare, curvilineo, circolare, ellittico, radiale, quadrato, rettangolare, triangolare, esagonale, a stella, allungato e amorfo.

#### Ombra
La riduzione dell'ombra è importante nel telerilevamento perché le ombre tendono a oscurare oggetti che altrimenti potrebbero essere rilevati. Tuttavia, l'ombra proiettata da un oggetto può essere l'unico indizio reale per la sua identificazione. Le ombre possono anche fornire informazioni sull'altezza di un oggetto in modo qualitativo o quantitativo.

#### Tonalità e Colore
Una banda di radiazione elettromagnetica registrata da uno strumento di telerilevamento può essere visualizzata su un'immagine in sfumature di grigio che vanno dal nero al bianco. Queste sfumature sono chiamate "tonalità" e possono essere riferite qualitativamente come scure, chiare o intermedie (gli esseri umani possono vedere 40-50 tonalità). La tonalità è correlata alla quantità di luce riflessa dalla scena in uno specifico intervallo di lunghezza d'onda (banda).

#### Texture
La texture si riferisce alla disposizione della tonalità o del colore in un'immagine. È utile perché le caratteristiche terrestri che mostrano tonalità simili spesso mostrano texture diverse. Aggettivi includono liscio (uniforme, omogeneo), intermedio e ruvido (grossolano, eterogeneo).

#### Altezza e Profondità
Come discusso, le ombre possono spesso offrire indizi sull'altezza degli oggetti. A loro volta, le altezze relative possono essere utilizzate per interpretare gli oggetti. In modo simile, le profondità relative possono spesso essere interpretate. Le descrizioni includono alto, intermedio e basso; profondo, intermedio e poco profondo.

#### Associazione
Questo è molto importante quando si cerca di interpretare un oggetto o un'attività. L'associazione si riferisce al fatto che certe caratteristiche e attività sono quasi sempre correlate alla presenza di certe altre caratteristiche e attività.

### Fotogrammetria Aerea

**Vantaggi:**
- Molto precisa
- Rappresentazione 3D
- Efficiente in termini di tempo
- Conveniente
- Basata su algoritmi ben consolidati e testati
- Minimo sforzo manuale
- Maggiore fedeltà geografica

### Cos'è la Fotogrammetria?

"La fotogrammetria è la tecnica di misurare oggetti da fotografie." "L'arte, la scienza e la tecnologia per ottenere informazioni spaziali affidabili su oggetti fisici e l'ambiente attraverso i processi di registrazione, misurazione e interpretazione dei dati dell'immagine."

### Tipi di Fotogrammetria

- **Fotogrammetria Aerea**: La fotocamera è montata su un aeromobile e di solito è puntata verticalmente verso il suolo. Vengono scattate più foto sovrapposte del terreno mentre l'aereo vola lungo una traiettoria di volo. Queste foto vengono elaborate in uno stereo-plotter (uno strumento che consente a un operatore di vedere due foto contemporaneamente in una vista stereo). Queste foto vengono anche utilizzate nell'elaborazione automatizzata per la creazione di Modelli Digitali di Elevazione (DEM).

- **Fotogrammetria a Corto Raggio**: La fotocamera è vicina al soggetto e di solito è tenuta in mano o su un treppiede. Di solito questo tipo di lavoro fotogrammetrico è non-topografico - cioè l'output non sono prodotti topografici come modelli del terreno o mappe topografiche, ma disegni e modelli 3D. Le fotocamere di tutti i giorni vengono utilizzate per modellare edifici, strutture ingegneristiche, veicoli, scene forensi e di incidenti, set cinematografici, ecc.

<br>
<br>
<br>

### Fotografia Stereo

Le foto aeree adiacenti ma sovrapposte sono chiamate coppie stereo e sono necessarie per determinare la parallasse e la visione stereo/3D.

- **Endlap**: ~60%
- **Sidelap**: ~20-30%

### Vecchie Pellicole
- a. Pancromatica
- b. Infrarosso B/N
- c. Pancromatico a colori
- d. Infrarosso a colori

### Interpretazione
Esempi di patterns corrispondenti ai principali reticoli idrografici:
- A = Dendritico
- B = Subdendritico
- C = Pettinato
- D = Parallelo
- E = Subparallelo
- F = Rettangolare o angolato
- G = Angolare
- H = Radiale
- I = Anulare
- L = Intrecciato
- M = Meandriforme
- N = A doline

### Estrazione di Feature Digitali
- Edifici
- Caratteristiche di trasporto
- Caratteristiche idrografiche
- Utilità
- Vegetazione
- Breaklines
- Punti DTM
- Ponti

### Vettoriale vs Raster
- I dati raster sono descritti da una griglia di celle, un valore per cella.
- I dati vettoriali utilizzano punti, linee e poligoni per rappresentare le feature.

<br>

### Curve di Livello
Le curve di livello sono linee tracciate su una mappa che collegano punti di uguale elevazione. Le curve di livello sono utili perché ci permettono di mostrare la forma della superficie terrestre (topografia) su una mappa. Questa spaziatura verticale è chiamata intervallo delle curve di livello. Se l'intervallo delle curve di livello è di 10 m, ogni curva di livello sarà un multiplo di 10 m (cioè 0, 10, 20, 30). Nelle aree con alto rilievo, l'intervallo delle curve di livello è solitamente più ampio.

### Estrazione (falsa) 3D: DTM e DEM

Non c'è un uso comune dei termini Modello Digitale di Elevazione (DEM), Modello Digitale del Terreno (DTM) e Modello Digitale di Superficie (DSM) nella letteratura scientifica. Nella maggior parte dei casi:
- Il termine Modello Digitale di Superficie rappresenta la superficie terrestre (compresi edifici, vegetazione, ecc.)
- Il Modello Digitale del Terreno rappresenta la superficie del suolo nudo
- Il termine Modello Digitale di Elevazione è spesso usato come termine generico per DSM e DTM, rappresentando solo informazioni di altezza senza ulteriore definizione sulla superficie.

### Modellazione 3D della Città

### Generazione di Ortofoto
L'output della fotogrammetria è tipicamente una mappa, un disegno o un modello 3D di una scena o oggetto del mondo reale. Molte delle mappe che usiamo oggi sono create con la fotogrammetria e fotografie scattate da aerei.

Le ortofoto solitamente hanno alcune limitazioni geometriche: mostrano solo gli elementi situati al livello di altezza del DEM utilizzato nella posizione corretta. Gli edifici non inclusi nel DEM vengono spostati con la posizione dei tetti a seconda della tangente dell'angolo nadir della posizione dell'immagine moltiplicata per l'altezza dell'edificio. Se il valore di altezza del tetto è incluso in un DEM dettagliato, il tetto viene mostrato nella posizione corretta corrispondente a una proiezione cartografica ortogonale.

<div style="page-break-after: always;"></div>

## 01.03 TELERILEVAMENTO: IMMAGINI SATELLITARI

### Sistemi Ottici: Telerilevamento Passivo

Il telerilevamento ottico utilizza sensori nel visibile, nel vicino infrarosso e nell'infrarosso a onde corte per formare immagini della superficie terrestre rilevando la radiazione solare riflessa dagli obiettivi sul terreno.

### Orbite Satellitari

Il percorso seguito da un satellite è definito orbita. I satelliti geostazionari si trovano ad altitudini di circa 329.000 km e ruotano a velocità che corrispondono alla rotazione terrestre. La maggior parte delle piattaforme satellitari di telerilevamento oggi si trova in orbite quasi polari, il che significa che il satellite viaggia verso nord su un lato della Terra e poi verso il polo sud nella seconda metà della sua orbita. Queste sono chiamate rispettivamente passaggi ascendenti e discendenti.

### Immagini Satellitari

- **Panoramiche**: Un sensore a canale singolo viene utilizzato per rilevare la radiazione. Se l'intervallo di lunghezza d'onda e l'intervallo visibile coincidono, l'immagine apparirà come una fotografia in bianco e nero scattata dallo spazio.
- **Multispettrali**: Utilizzano un rilevatore multicanale e registrano la radiazione con un intervallo ristretto. Sono disponibili informazioni sulla luminosità e sul colore.

### Risoluzione Spaziale
Area minima sul terreno visibile al sensore. Esempio: Quickbird Pancromatico – 293 cm di risoluzione.

### Risoluzione Radiometrica
La risoluzione radiometrica di un sistema di imaging descrive la sua capacità di discriminare differenze molto sottili di energia. Più fine è la risoluzione radiometrica di un sensore, più è sensibile nel rilevare piccole differenze nell'energia riflessa o emessa.

### Risoluzione Spettrale
Descrive la capacità di un sensore di definire intervalli di lunghezza d'onda fini. Più fine è la risoluzione spettrale, più ristretto è l'intervallo di lunghezza d'onda per un particolare canale o banda.

### Risoluzione Temporale
La risoluzione temporale di un sistema di telerilevamento per acquisire immagini della stessa identica area con lo stesso angolo di visualizzazione una seconda volta è uguale a questo periodo.

<div style="page-break-after: always;"></div>

### Satelliti

#### Landsat
7 bande con le seguenti caratteristiche:

| Banda No. | Intervallo di lunghezza d'onda (μm) | Risposta Spettrale | Risoluzione (m) |
|-----------|--------------------------------------|---------------------|-----------------|
| 1 | 0.45 - 0.52 | Blu-Verde | 30 |
| 2 | 0.52 - 0.60 | Verde | 30 |
| 3 | 0.63 - 0.69 | Rosso | 30 |
| 4 | 0.76 - 0.90 | Vicino Infrarosso | 30 |
| 5 | 1.55 - 1.75 | Medio-Infrarosso | 30 |
| 6 | 10.40 - 12.50 | Infrarosso Termico | 120 |
| 7 | 2.08 - 2.35 | Medio-Infrarosso | 30 |

### Software per l'Analisi di Immagini

**OPTICKS** è una piattaforma software espandibile per il telerilevamento e l'analisi di immagini, gratuita e open source.
- Supporta i seguenti formati di file: NITF 2.0/2.1, GeoTIFF, ENVI, ASPAM/PAR, CGM, DTED, Generic RAW, ESRI Shapefile, HDF5, AVI, MPEG, JPEG, GIF, PNG, BMP
- Zoom, pan, rotazione di grandi dataset spaziali
- Sovrapposizione rapida di feature GIS, annotazioni, risultati e altre informazioni sui dati
- Molti controlli di visualizzazione delle immagini come colormap, istogramma, trasparenza, ecc.
- Supporto per dataset più grandi di quattro gigabyte
- Supporto per l'elaborazione dei dati nel suo interleave nativo di BIP, BSQ o BIL

### RADAR

**RADAR** (RAdio Detection And Ranging): Sistema di rilevamento di oggetti che utilizza onde elettromagnetiche per determinare la distanza, la direzione o la velocità.

**SAR** (Synthetic-Aperture Radar): Forma di radar la cui caratteristica distintiva è l'uso del movimento relativo tra un'antenna e la sua regione target per fornire variazioni di segnale coerenti a lungo termine, che vengono sfruttate per ottenere una risoluzione spaziale più fine di quanto sia possibile con i mezzi di scansione a fascio convenzionali.

I dati SAR in ampiezza non sono (quasi) influenzati dall'illuminazione solare e/o dalle condizioni meteorologiche.

<div style="page-break-after: always;"></div>

### Interferometria a Passaggi Ripetuti: Rilevamento del Movimento del Target

**Generazione di Interferogrammi Differenziali**

Ingredienti: 2 immagini SAR V1, V2 e un DEM

Procedura:
1. V1 e V2 vengono moltiplicate in modo incrociato per formare un interferogramma.
2. Il DEM viene utilizzato per generare un interferogramma sintetico che, naturalmente, contiene solo il contributo topografico.
3. L'interferogramma sintetico viene sottratto (moltiplicato in modo incrociato) dall'interferogramma V1-V2 per rimuovere il contributo di fase topografica ed evidenziare possibili contributi di fase dovuti a deformazione del terreno.

### Tecnica dei Riflettori Permanenti (PS)
Utilizza lunghe serie temporali di dati SAR per identificare bersagli radar coerenti (PS) dove i contributi di movimento e atmosfera possono essere separati e possono essere eseguite misurazioni molto accurate.

**Applicazioni:**
- Rilevamento e monitoraggio di frane (lente)
- Subsidenza
- Dinamica delle faglie

<div style="page-break-after: always;"></div>

## 02.01-02.02 LIDAR

### LIDAR (Light Detection And Ranging)

Il LIDAR è una tecnologia che permette di determinare la distanza di un oggetto mediante emissioni laser.

**LASER** – Light Amplification by Simulated Emission of Radiation.

### Come Funziona il LIDAR?

Ogni volta che il laser viene pulsato:
- Il laser genera un impulso ottico
- L'impulso viene riflesso da un oggetto e ritorna al ricevitore del sistema
- Un contatore ad alta velocità misura dall'impulso di inizio all'impulso di ritorno
- La misurazione del tempo viene convertita in una distanza (la distanza dal bersaglio e la posizione dello scanner laser vengono quindi utilizzate per determinare l'elevazione e la posizione)
- È possibile misurare ritorni multipli per ogni impulso
- Viene misurato tutto ciò che è visibile dalla posizione

### LIDAR vs Fotogrammetria Tradizionale

| LIDAR | Fotogrammetria |
|-------|---------------|
| Acquisizione di dati di giorno o di notte | Raccolta solo di giorno |
| Acquisizione diretta di raccolta 3D | Procedure complicate e talvolta inaffidabili |
| L'accuratezza verticale è migliore di quella planimetrica | L'accuratezza planimetrica è migliore di quella verticale |
| La nuvola di punti è difficile da cui derivare informazioni semantiche; tuttavia, i valori di intensità possono essere utilizzati per produrre un prodotto simile a un'immagine visivamente ricca | Ricca di informazioni semantiche |

### Due Tipi Principali

- **Laser Scanner Terrestre (Ground-based)**
- **Laser Scanner Aereo (Airborne)**

### Laser Scanner Terrestre

**Principio**: Il dispositivo emette un impulso laser che viene riflesso dall'oggetto e ritorna al ricevitore. La distanza viene calcolata in base al tempo di volo.

**Acquisizione finale:**
- Una nuvola di punti
- Ogni punto ha coordinate x, y, z relative all'emettitore/ricevitore
- Ogni punto ha anche proprietà riflettenti legate al colore, rugosità, umidità - riflettanza

**Applicazioni:**
- Architettura
- Archeologia
- Geologia (es. monitoraggio di frane, analisi di affioramenti)
- Calcolo di volumi
- Industriale
- Deformazione

### LIDAR Aereo

**Componenti del sistema:**
- Aeromobile
- Unità emettitore-ricevitore laser a scansione
- GPS differenzialmente corretto
- Unità di misura inerziale (IMU)
- Computer

**Applicazioni:**
- Geologia
- Forestale
- Agricoltura
- Idrologia
- Rilevamento marino
- Copertura del suolo e uso del suolo
- Scopi militari

**Accuratezza complessiva:**
- Posizione (X,Y,Z) di ogni ritorno: 50-100 cm orizzontale, 10-15 cm verticale
- Superficie del suolo (superficie del suolo nudo): cos'è il suolo (erba, rocce, ceppi)?
- Altezze degli alberi: sottostima dell'altezza degli alberi da 0,5 a 2 m (l'errore dipende dalla specie)

**Prodotti derivati dal LIDAR aereo:**
- Modelli Digitali di Elevazione (DEM)
- Modelli Digitali del Terreno (DTM) (dati di elevazione del suolo nudo)
- Reti Irregolari Triangolate (TIN)
- Breaklines - una linea che rappresenta una caratteristica che si desidera preservare in un TIN (esempio: torrente o cresta)
- Curve di livello
- Rilievo ombreggiato
- Pendenza ed Esposizione

### Echi Multipli del LIDAR Aereo

Il LIDAR può registrare più ritorni da un singolo impulso laser, permettendo di distinguere tra il primo ritorno (ad esempio, dalla chioma degli alberi) e l'ultimo ritorno (dal suolo).

### DEM vs DTM vs DSM

- **DEM (Digital Elevation Model)**: Termine generico per rappresentare l'elevazione.
- **DTM (Digital Terrain Model)**: Rappresenta la superficie del suolo nudo ("Ground").
- **DSM (Digital Surface Model)**: Rappresenta la superficie superiore ("top surface"), inclusi edifici e vegetazione.

In terreno aperto, la separazione tra superficie e suolo nudo è chiara. Il DEM è diverso dai punti laser misurati per due ragioni principali:
1. Filtraggio: classificazione dei punti in terreno e fuori terreno.
2. Base per la generazione del DTM, rilevamento di oggetti topografici.

### Visualizzazione

Il rilievo ombreggiato e l'illuminazione del DEM possono essere utilizzati come semplice tecnica di visualizzazione. Questi metodi sono soggettivi e sensibili ai parametri hardware.

### Ulteriori Analisi e Validazione a Terra

Una volta disponibile il DTM o DEM, il GIS può essere utilizzato per ulteriori analisi e modellazioni sistematiche. La valutazione dell'accuratezza dovrebbe essere sempre tentata (l'approccio migliore è fare una validazione a terra).

<div style="page-break-after: always;"></div>

## 02.03 DRONI (UAV - Unmanned Aerial Vehicle)

### Nascita Militare

Nel 1849 l'Austria inviò palloni senza pilota riempiti di bombe per attaccare Venezia. Le innovazioni dei UAV iniziarono all'inizio del 1900 e inizialmente si concentrarono sulla fornitura di bersagli per l'addestramento del personale militare. Lo sviluppo dei UAV continuò durante la Prima Guerra Mondiale, quando la Dayton-Wright Airplane Company inventò un siluro aereo senza pilota che sarebbe esploso in un tempo preimpostato.

### Due Tipi Principali

#### Ala Fissa (Fixed Wing)
Vantaggi: più produttivi, capacità di planare e quindi di accendere e spegnere i motori permette al velivolo di rimanere più tempo in quota. Ciò si traduce in più ettari misurati in ogni singola missione. Questo tipo di drone è anche più veloce nella navigazione. Si possono montare sensori fotografici, termici, multispettrali. Il limite principale rispetto a un multirotore è la possibilità di stazionare su un punto per analizzare con calma un oggetto.

#### Multi-rotore
Vantaggi:
- Capacità di rimanere sopra un punto o muoversi lentamente; questa caratteristica consente di fare analisi e acquisire informazioni aggiuntive.
- La fotocamera può essere ruotata in più direzioni; poter ruotare la fotocamera da verticale a orizzontale consente di misurare anche tutti gli oggetti verticali.
- Sul multirotore è possibile inserire più sensori: sensore fotografico, termografico, multispettrale e persino scanner laser 3D.

### Pianificazione del Volo

Workflow:
- Selezionare l'area di rilevamento da una mappa come Google
- Impostare le caratteristiche della fotocamera montata sul drone
- Impostare l'altitudine di volo

Il software mostrerà:
- Percorso del drone con traiettorie
- Tempo di volo
- Numero di fotografie e loro posizione
- Dimensione del pixel sul terreno

### Fotogrammetria con Droni

Dopo l'acquisizione, le immagini verranno caricate sul PC ed elaborate con un software di fotogrammetria.

**Vantaggi della fotogrammetria digitale moderna:**
- Consente di eseguire rapidamente grandi quantità di fotogrammi limitando le spese e i tempi di sviluppo.
- Il tecnico ha la possibilità in "tempo reale" di valutare la qualità delle immagini evitando lunghe attese e il rischio di dover tornare sul sito in un secondo momento.
- Gli automatismi disponibili oggi consentono un'autonomia quasi completa nell'ottenere modelli 3D con nuvole di punti molto simili a quelle ottenute con uno scanner laser.
- Semplicità d'uso, mentre in passato erano necessarie competenze specifiche per i voli.
- Il software durante l'elaborazione non ha bisogno della presenza del tecnico.
- Possibilità di avere un risultato unico descritto in una nuvola di punti.
- Il costo totale dell'strumentazione Hardware (fotocamera) e Software è decine di volte inferiore rispetto al costo di uno dei 2 singoli articoli acquistati 10/15 anni fa.

### Elaborazione delle Immagini: Orientamento Interno

In passato, la prima operazione consisteva nell'inserire nel software un certificato di calibrazione della fotocamera. I software moderni calcolano automaticamente questi valori grazie alla capacità di riconoscere automaticamente lo stesso punto reale e misurato su più fotogrammi, utilizzando la correlazione di pixel omologhi. Questa fase è chiamata "orientamento interno".

### Elaborazione delle Immagini: Orientamento Esterno

Il processo di orientamento esterno relativo permette di calcolare la posizione di un'immagine rispetto all'altra al momento dello scatto. Questa operazione, che in passato veniva eseguita manualmente riconoscendo una dozzina di punti in comune tra una foto e l'altra, ora avviene automaticamente. Utilizzando una correlazione digitale dei pixel dell'immagine, il software estrapola una quantità di punti considerevolmente superiore.

### Elaborazione delle Immagini: Modellazione 3D

Una volta ottenute le posizioni di scatto, siamo in grado di ottenere un modello 3D. La posizione del punto a terra viene calcolata proiettando lo stesso pixel per la distanza focale fino a quando non si incrociano. Questo processo è completamente automatico e viene eseguito su ogni pixel.

### Elaborazione delle Immagini: Orientamento Assoluto

Il modello 3D ottenuto è ancora fuori scala. Inserendo punti di controllo, con valori di coordinate X Y Z misurati con strumentazione grafica come GPS o Stazione Totale e riconoscendoli nelle immagini o nelle nuvole di punti, possiamo riportare il modello alle dimensioni effettive.

La quantità di punti è proporzionale all'area di lavoro, e la loro dislocazione dovrebbe essere progettata in modo da distribuire i punti nel modo più omogeneo possibile mantenendoli il più distanti possibile.

<div style="page-break-after: always;"></div>

## 03.00 SISTEMI INFORMATIVI GEOGRAFICI (GIS)

### GIS? Cos'è?

Un sistema per memorizzare, recuperare, ordinare e confrontare dati spaziali per supportare un processo analitico.

- **Informazione Geografica/Geospaziale**: Informazioni su luoghi sulla superficie terrestre; conoscenza su "cosa è dove quando" (non dimenticare il tempo!)
- **GIS – cosa c'è nella S?**
  - **Systems**: la tecnologia
  - **Science**: i concetti e la teoria
  - **Studies**: il contesto sociale

### Sistemi GIS, Scienza e Studi

- **Sistemi**: tecnologia per l'acquisizione e la gestione di informazioni spaziali.
- **Scienza**: comprensione dei problemi concettuali sottostanti la rappresentazione di dati e processi nello spazio-tempo; la teoria e i concetti alla base della tecnologia.
- **Studi**: comprensione delle questioni sociali, legali ed etiche associate all'applicazione del GIS.

### Definizione di GIS

Un GIS è un sistema (hardware + motore del database) progettato per assemblare, archiviare, aggiornare, analizzare, manipolare e visualizzare in modo efficiente informazioni geograficamente referenziate (dati identificati dalla loro posizione). Un GIS include anche le persone che gestiscono il sistema e i dati che vi confluiscono.

### Componenti del GIS

- **Hardware**: Computer, reti, stampante, plotter, scanner
- **Software**: Software GIS, software database, software OS, software di rete
- **Dati**: Dati vettoriali, dati raster, immagini, attributi
- **Persone**: Amministratori, gestori, tecnici GIS, utenti
- **Regole**: Linee guida, standard, procedure

### Modello Dati GIS: Scopo

Permette di rappresentare e memorizzare digitalmente le caratteristiche geografiche del mondo reale in un database, in modo che possano essere presentate in forma astratta (mappa analogica) e possano essere manipolate per affrontare un problema specifico.

### Astrarre il Mondo Reale

Il GIS rappresenta il mondo reale attraverso modelli digitali composti da layer (strati) tematici.

### Esempio di Modello Dati GIS

Tre layer o temi:
- Strade
- Idrologia (acqua)
- Topografia (elevazione del terreno)

Possono essere relazionati perché coordinate geografiche precise sono registrate per ogni tema. I layer sono composti da due tipi di dati:
- Dati spaziali che descrivono la posizione (dove)
- Dati attributo che specificano cosa, quanto, quando

I layer possono essere rappresentati in due modi:
- Formato vettoriale come punti e linee
- Formato raster (o immagine) come pixel

Tutti i dati geografici hanno 4 proprietà: proiezione, scala, accuratezza e risoluzione.

### Il GIS Collega le Caratteristiche Grafiche ai Dati Tabulari

Il GIS collega le caratteristiche grafiche (entità) ai dati tabulari (attributi).

### Analisi GIS

- Classificazione dei dati
- Confronto dei dati
- Intersezione di caratteristiche grafiche
- Operazioni topologiche
- Statistiche spaziali
- Modellazione spaziale
- Data mining

### Output GIS

- Mappe
- Diagrammi
- Report
- Modelli n-dimensionali

<div style="page-break-after: always;"></div>

## 03.01 CARTOGRAFIA DIGITALE E BANCHE DATI

### Analogico vs Digitale

**Analogico:**
- Mappe cartacee
- Fotografie aeree stampate
- Tabelle di statistiche
- Scala fissa
- Necessità di conversione in formato digitale

**Digitale:**
- File di dati digitali
- Immagini da telerilevamento
- File di output GPS
- Scala 'libera'/flessibile
- Formato file predeterminato
- Download o copia

### Mappe Dinamiche

- Muoversi sulla mappa con pan/zoom/jump
- Cambiare simboli: linee/colori/icone/font
- Visualizzare più dati e mappe contemporaneamente
- Attivare/disattivare informazioni

### Selezioni GIS

- Selezione grafica
- Query di selezione

### Il GIS Collega le Entità agli Attributi

Il GIS collega elementi grafici al database:
- Coordinate spaziali
- Simboli
- Dati/Informazioni

### Metadati

Il termine metadati è spesso spiegato come "dati sui dati". I metadati si trovano tradizionalmente nei cataloghi delle biblioteche. Con l'informazione sempre più digitale, i metadati sono anche utilizzati per descrivere i dati digitali utilizzando standard di metadati specifici per una particolare disciplina. Descrivendo il contenuto e il contesto dei file di dati, la qualità dei dati/file originali viene notevolmente aumentata.

#### Metadati Geospaziali
I metadati geospaziali (o semplicemente metadati se usati in un contesto geografico) sono un tipo di metadati applicabile a oggetti che hanno un'estensione geografica esplicita o implicita, cioè sono associati a una posizione sulla superficie del globo.

**ISO 19115 "Informazioni Geografiche - Metadati"**: Questo standard internazionale fornisce informazioni sull'identificazione, l'estensione, la qualità, lo schema spaziale e temporale, il riferimento spaziale e la distribuzione dei dati geografici digitali.

**INSPIRE**: Un'iniziativa dell'UE per stabilire un'infrastruttura per informazioni spaziali in Europa che aiuterà a rendere le informazioni spaziali o geografiche più accessibili e interoperabili per un'ampia gamma di scopi a sostegno dello sviluppo sostenibile. La direttiva INSPIRE è entrata in vigore il 15 maggio 2007. Affronta 34 temi di dati spaziali necessari per le applicazioni ambientali.

<div style="page-break-after: always;"></div>

## 03.02 FORMATI FILE, GEOREFERENZIAZIONE, FEATURES

### Raster vs Vettoriale

**Vantaggi del Raster:**
- Il formato di dati più comune
- Facile eseguire operazioni matematiche e di sovrapposizione
- Le informazioni satellitari sono facilmente incorporate
- Rappresenta meglio i dati di tipo "continuo"

**Vantaggi del Vettoriale:**
- Informazioni posizionali accurate, ideali per memorizzare caratteristiche tematiche discrete (es. strade, linee di costa, caratteristiche del fondale marino)
- Requisiti di archiviazione dati compatti
- Possibilità di associare un numero illimitato di attributi a caratteristiche specifiche

### Elementi Spaziali

- Raster: griglia di celle (pixel)
- Vettoriale: punti, linee, poligoni
- Mondo Reale

### Formato Raster

Memorizza le immagini come righe e colonne di numeri con un Valore Digitale/Numero (DN) per ogni cella. Le unità sono solitamente rappresentate come celle quadrate uniformi per dimensione. I dati sono classificati come "continui" (come in un'immagine) o "tematici" (dove ogni cella denota una caratteristica).

#### Principali Formati Raster
- ADRG, BIL, CADRG, CIB, Digital Raster Graphic (DRG), ECRG
- ECW (Enhanced Compression Wavelet)
- Esri grid
- **GeoTIFF**: Variante TIFF arricchita con metadati GIS rilevanti
- IMG (ERDAS IMAGINE)
- JPEG2000
- MrSID (Multi-Resolution Seamless Image Database)

#### Geo-TIFF
GeoTIFF è uno standard di metadati di dominio pubblico che consente di incorporare informazioni di georeferenziazione all'interno di un file TIFF. Il formato GeoTIFF è pienamente conforme a TIFF 6.0.

Il Geo-TIFF è composto da almeno due file: .TIF/.TIFF e .TFW. A volte necessita di un altro file .PRJ (file di proiezione/CRS).

### Attributi

- Nel modello di dati raster, il valore della cella (Numero Digitale) è l'attributo. Esempi: luminosità, codice di copertura del suolo, SST, ecc.
- Per i dati vettoriali, i record degli attributi sono collegati a caratteristiche puntuali, lineari e poligonali. È possibile memorizzare più attributi per caratteristica. Le caratteristiche vettoriali sono collegate agli attributi da un numero univoco di caratteristica.

### Formato Vettoriale: Shapefile

Lo shapefile è un formato proprietario sviluppato da ESRI. Memorizza le informazioni sulla geometria e sugli attributi per i set di dati spaziali.

Uno shapefile è composto da 3 file obbligatori:
- **.shp** — formato della forma; la geometria della caratteristica stessa
- **.shx** — formato dell'indice delle forme; un indice posizionale della geometria delle caratteristiche
- **.dbf** — formato degli attributi; attributi colonnari per ogni forma, in formato dBase IV

**File opzionali:**
- .prj — formato di proiezione; informazioni sul sistema di coordinate e proiezione
- .sbn e .sbx — indice spaziale delle caratteristiche
- .shp.xml — metadati geospaziali in formato XML
- .cpg — utilizzato per specificare la code page (solo per .dbf)

**Problemi con lo Shapefile:**
- È un formato piuttosto obsoleto.
- Non è un singolo file; almeno tre file sono richiesti.
- I nomi degli attributi non possono superare i 10 caratteri.
- I campi di tipo stringa non possono memorizzare più di 255 caratteri.
- Non gestisce informazioni topologiche.
- Limite di 2 GB di dati.

### Formato Vettoriale: Spatialite

Spatialite è un formato open source sviluppato da Alessandro Furrieri. Supporta un tipo di dati Geometry conforme allo standard internazionale OGC-SFS (Open Geospatial Consortium - Simple Feature SQL). Spatialite supporta un driver Virtual Shapefile per l'accesso SQL (sola lettura) a uno shapefile esterno.

#### Geometrie (Sottoclassi)

- **Point**: {x,y}
- **LineString**: semplice, non-semplice, chiusa
- **Polygon**: anello esterno, anelli interni
- **MultiPoint**
- **MultiLineString**
- **MultiPolygon**
- **GeometryCollection**: qualsiasi raccolta arbitraria di sottoclassi elementari (raramente utilizzata).

### Combinare Mappe Raster e Vettoriali

### Georeferenziazione

Georeferenziare qualcosa significa definire la sua esistenza nello spazio fisico, stabilendo la sua posizione in termini di proiezioni cartografiche o sistemi di coordinate.

**Applicazioni:**
- Fondamentale per rendere utili le immagini aeree e satellitari per la mappatura.
- Combina o confronta dati prodotti in periodi di tempo diversi.
- Combina e sovrappone mappe con diversi sistemi di proiezione.
- Stabilisce il rapporto tra risultati di indagini sociali e aree geografiche.

#### Ground Control Points (GCP)
Un GCP è un punto sulla superficie terrestre di posizione nota (cioè fissato all'interno di un sistema di coordinate stabilito) utilizzato per georeferenziare fonti di dati immagine. Mentre solo pochi GCP sono necessari (normalmente due-quattro) per ortocorreggere le mappe, è essenziale ottenere un minimo di 12 punti, anche se 15-20 punti sarebbero un obiettivo preferibile. Questi punti dovrebbero essere distribuiti in tutta l'immagine.

#### Georeferenziazione con QGIS
La georeferenziazione in QGIS viene eseguita tramite il plugin 'Georeferencer'.

<div style="page-break-after: always;"></div>

## 03.03 QGIS (QUANTUM GIS)

### Perché QGIS?

QuantumGIS è:
- Un software open source e multipiattaforma (Linux, MS Windows, Mac OS X) per GIS
- Collaborativo, stabile, maturo e ben documentato
- Molto personalizzabile
- Gratuito!

### Avviare un Nuovo Progetto

Ogni volta che si apre QGIS, viene avviato un nuovo progetto. È possibile caricare i layer (raster e vettoriali). Quando si salva un progetto, tutti i dati vengono salvati in un file .qgs contenente i layer e le loro proprietà, proiezioni (SR).

### Gestione dei Sistemi di Riferimento delle Coordinate (CRS/SR)

Quando si importano mappe raster o vettoriali, viene visualizzata una finestra per selezionare il CRS.

Per la CTR italiana si sceglie EPSG:3004 Monte Mario / Italy zone 2.

### Aggiungere File Raster

Tramite il menu Layer > Aggiungi livello > Aggiungi livello raster... o l'apposito pulsante della barra degli strumenti.

### Aggiungere File Vettoriali

Tramite il menu Layer > Aggiungi livello > Aggiungi livello vettoriale... o l'apposito pulsante.

### Visualizzare Dati Vettoriali: Cambiare Stile

Fare doppio clic sul layer nel pannello Livelli per aprire le Proprietà del layer, quindi selezionare la scheda Stile.

### Visualizzare Dati Vettoriali: Etichette

Nelle Proprietà del layer, selezionare la scheda Etichette.

### Aggiungere Altri Layer Raster

Ripetere la procedura di aggiunta.

### Aggiungere WMS

Aggiungere un WMS (Web Mapping Service) dal menu o dalla barra degli strumenti (Layer > Aggiungi livello > Aggiungi layer WMS/WMTS...). È necessario essere connessi a Internet.

### Creare Nuovi Layer

Esercizio: creare un nuovo layer "strade" e colorarlo per le sue proprietà.
Esercizio: creare un nuovo layer "Palazzi" e colorarlo per le sue proprietà.

<div style="page-break-after: always;"></div>

## 04. SISTEMI DI POSIZIONAMENTO GLOBALE (GPS/GNSS)

### Panoramica

- Finanziato e controllato dal Dipartimento della Difesa degli Stati Uniti
- Fornisce segnali radio appositamente codificati che possono essere elaborati in un ricevitore GPS
- Posizione, velocità, tempo
- Tutto dipende da una tempistica altamente accurata

**Satelliti**: 31+/- satelliti in orbita a circa 12.000 miglia (11.000 Nm o 20.000 km) di altezza. 6 percorsi, eliosincroni, ogni satellite orbita intorno alla Terra 2 volte al giorno. Operativo nel 1995, massimo 32 satelliti.

### Storia

- Studi di fattibilità iniziati negli anni '60.
- Il Pentagono stanzia fondi nel 1973.
- GLONASS iniziò nell'Unione Sovietica nel 1976.
- Primo satellite lanciato nel 1978.
- Sistema dichiarato pienamente operativo nell'aprile 1995.
- Il Pentagono ridusse S/A (Selective Availability) a zero metri di errore, maggio 2000.
- Galileo 2016.

### Componenti

**3 Segmenti:**

1. **Segmento di Controllo**: Comprende 5 stazioni che misurano le distanze dei satelliti soprastanti ogni 1,5 secondi e inviano i dati corretti al Master Control, dove vengono determinati l'orbita del satellite, le prestazioni dell'orologio e la salute del satellite. Queste informazioni vengono inviate alle tre stazioni di uplink.

2. **Segmento Spaziale**: 24 satelliti GPS (Space Vehicles - SVs). I satelliti orbitano intorno alla Terra in 12 ore. 6 piani orbitali inclinati di 55 gradi rispetto all'equatore. Questa costellazione fornisce da 5 a 8 satelliti da qualsiasi punto della Terra.

3. **Segmento Utente**: Consiste in ricevitori che decodificano i segnali dei satelliti. Il ricevitore esegue le seguenti attività: selezione di uno o più satelliti, acquisizione dei segnali GPS, misurazione e tracciamento, recupero dei dati di navigazione.

### Applicazioni Utente

- Militari
- Ricerca e soccorso
- Soccorso in caso di catastrofi
- Topografia
- Navigazione marittima, aeronautica e terrestre
- Guida di veicoli robotici e telecomandati
- Posizionamento e tracciamento satellitare
- Trasporto marittimo
- GIS
- Ricreazione

### Come Funziona il GPS?

**Requisiti:**
- Trilaterazione da satellite
- Misurazione della distanza attraverso il tempo di percorrenza dei segnali radio
- Tempistica molto accurata richiesta
- Per misurare la distanza, è necessario conoscere anche la posizione del satellite
- Infine, i ritardi devono essere corretti

Misurazioni dei tempi di arrivo della fase del codice da almeno quattro satelliti vengono utilizzate per stimare quattro quantità: posizione in tre dimensioni (X, Y, Z) e tempo GPS (T).

### Trilaterazione

La posizione viene calcolata dalla misurazione della distanza. Matematicamente abbiamo bisogno di quattro satelliti, ma tre sono sufficienti scartando la risposta assurda.

### Misurazione della Distanza

La distanza da un satellite viene determinata misurando quanto tempo impiega un segnale radio a raggiungerci dal satellite. Assumendo che gli orologi del satellite e del ricevitore siano sincronizzati, il ritardo del codice nel ricevitore moltiplicato per la velocità della luce ci dà la distanza.

#### Tempo Perfetto
Se gli orologi sono perfettamente sincronizzati, le distanze dei satelliti si intersecheranno in un singolo punto. Ma se imperfetti, i quattro satelliti non si intersecheranno nello stesso punto. Il ricevitore cerca una correzione comune che faccia intersecare tutti i satelliti nello stesso punto.

#### Problemi di Relatività
Misurare il tempo con un orologio sulla Terra e un altro in movimento nel cielo produce problemi legati alla Teoria della Relatività.

### Diluizione della Precisione (DOP)

La geometria dei satelliti può influenzare la qualità dei segnali GPS e l'accuratezza della trilaterazione del ricevitore. Il DOP riflette la posizione di ciascun satellite rispetto agli altri satelliti accessibili da un ricevitore.

- **PDOP** – Posizione (Est, Nord e Alto)
- **GDOP** – Geometrica (E,N,U e Tempo)
- **VDOP** – Verticale (Alto)
- **TDOP** – Tempo (Tempo)

**GDOP ideale**: Un satellite direttamente sopra con un'abbondanza di satelliti aggiuntivi distribuiti uniformemente nel cielo.
**GDOP scarso**: Satelliti raggruppati.

### Segnale Satellite GPS

- **L1** (1575.42 Mhz): trasporta il codice SPS e il messaggio di navigazione.
- **L2** (1227.60 Mhz): utilizzato per misurare i ritardi della ionosfera dai ricevitori PPS.
- **Codice C/A** (Coarse/Acquisition)
- **Codice P** (Precision)
- **Messaggio di navigazione**: segnale a 50 Hz costituito dalle orbite dei satelliti GPS, correzioni dell'orologio e altri parametri di sistema.

### Errori

#### Errori del satellite
- Errori nella modellazione dell'offset dell'orologio
- Errori nella rappresentazione kepleriana dell'effemeride
- Latenza nel tracciamento

#### Errori di propagazione atmosferica
- Attraverso la ionosfera: la fase della portante subisce un'anticipazione di fase e il codice subisce un ritardo di gruppo.
- Dipendenti da: latitudine geomagnetica, ora del giorno, elevazione del satellite.
- Gli errori atmosferici possono essere rimossi utilizzando misurazioni a doppia frequenza (confrontando i ritardi di L1 e L2).

#### Troposfera
Causa ritardi nel codice e nella portante, ma non sono dipendenti dalla frequenza. Gli errori sono modellati con successo.

#### Altri errori
- Multicammino (Multipath)
- Rumore del ricevitore
- Forze sul satellite GPS (gravità non uniforme della Terra, attrazione di altri corpi celesti, resistenza, radiazione solare)

### Fonti di Errore (Tipico ammontare per satellite)

- Errori dell'orologio atomico del satellite (corretti periodicamente)
- Errori dell'orbita del satellite (corretti periodicamente)
- Ionosfera terrestre (particelle cariche)
- Troposfera terrestre (umidità)
- Rumore del ricevitore
- Errori di multicammino
- Geometria satellitare scarsa (GDOP)
- Errori dell'orologio del ricevitore (corretti dal 4° satellite in poi)

### Correzione Differenziale

Confronta il file di dati GPS dal Rover (unità portatile) con un file di dati da una Stazione Base (in una coordinata nota) per lo stesso periodo di tempo. Si basa sul fatto che i ricevitori situati relativamente vicini tra loro registreranno errori simili dalla stessa costellazione di satelliti. Utilizza l'errore apparente del file della stazione base per correggere l'errore corrispondente del file del Rover.

- Può migliorare l'accuratezza fino a 20 m (50-90%).
- Richiede una stazione base locale (entro 100 miglia).
- Richiede "post-processing" (in laboratorio) o può essere fatto in tempo reale (Real-Time DGPS).

#### WAAS/EGNOS
Wide Area Augmentation System. Con S/A impostato a zero e in condizioni ideali, un ricevitore GPS senza WAAS può raggiungere un'accuratezza di quindici metri. In condizioni ideali, un ricevitore GPS con WAAS può raggiungere un'accuratezza di tre metri il 95% delle volte.

#### Accuratezza
- GPS originale (civile): 100 metri (con S/A attivo)
- GPS tipico: 15 metri (con S/A disattivato)
- DGPS con correzione differenziale: < 5 metri
- WAAS GPS: < 5 metri
- Ricevitori da topografi: < 5 millimetri

### Precisione vs Accuratezza

- (A) Misurazioni successive hanno valori simili (sono precise)
- (B) La precisione è inferiore ma l'accuratezza è maggiore

### Waypoint

Un waypoint si basa su coordinate inserite nella memoria del ricevitore GPS. Può essere una posizione fissa salvata o coordinate inserite dall'utente. Una volta inserito e salvato, un waypoint rimane invariato nella memoria del ricevitore fino a quando non viene modificato o cancellato.

### Protocollo NMEA

Molti ricevitori GPS possono trasmettere i dati di posizione a un PC o altro dispositivo utilizzando il protocollo NMEA 0183. Esempi di messaggi di output:
- GGA: Dati di fissaggio GPS
- GSA: DOP GPS e satellite attivo
- GSV: Satellite GPS in vista
- RMC: Dati GPS minimi raccomandati

### Altri Sistemi Globali di Navigazione Satellitare

- **GLONASS** (Russia): 23 satelliti operativi, 3 piani orbitali separati da 120 gradi, orbite inclinate di 65 gradi, periodo orbitale 11h 15m.
- **GALILEO** (Europa): Operativo dal 2016. 30 satelliti (inclusi 3 di riserva), altitudine orbitale 23.222 km, 3 piani orbitali, inclinazione di 56°.
- **COMPASS** (Cina): 14 satelliti operativi.

### GPS per Dispositivi Mobili

Molti smartphone e tablet sono anche ricevitori GPS di qualità abbastanza buona per localizzare e navigare. Un gran numero di app sfrutta le informazioni GPS.

<div style="page-break-after: always;"></div>

## 05.01 TECNICHE DI MAPPATURA DIGITALE

### Perché Abbiamo Scelto la Mappatura Digitale?

- Abbiamo esperienza nella mappatura sul campo.
- Abbiamo esperienza con precedenti software commerciali: MapIT.
- Crediamo che ci siano molti vantaggi nell'andare sul campo in modo digitale.

### Cosa Riteniamo Importante sul Campo?

**Mantenere il modo tradizionale di mappare**: Metodo penna-su-carta → Tecnologia Digital-Ink. Minima educazione "digitale".

**Acquisizione veloce con strumenti semplici**:
- Numero minimo di attivazioni sulle barre degli strumenti con procedure performanti.
- Facile connessione di altri dispositivi digitali (antenna GPS, fotocamera, bussola digitale, ecc.).
- Nessun problema di sistema/driver/IT.
- Interfaccia umana giusta (dimensioni, leggibilità).

**Migliorare l'accuratezza/precisione senza esagerare**:
- Tenendo conto delle limitazioni (incertezze, triangolazioni, scala) della mappatura "cartacea", il posizionamento GPS può migliorare la precisione e la qualità dei dati.
- Valutazione delle incertezze conoscendo la copertura dell'area di rilevamento (controllo sul lavoro sul campo).
- Terza e quarta dimensione.

**Archiviare tutti i dati insieme e gestirli**:
- Tutti i dati/info nella stessa cartella.
- Portare sul campo anche altri documenti utili (mappe, articoli, libri, ecc.).
- Differenziare i dati/info acquisiti e le interpretazioni post-elaborazione (diversi layer).

**Trasferire e/o Condividere Dati/Informazioni**:
- Possibilità di trasferire tutti i dati/info in altre applicazioni/strumenti.
- Facile comunicazione di dati/info tramite web (e-mail, cloud) o telefono mobile.
- Consentire il lavoro di gruppo.

### Pro e Contro della Mappatura Tradizionale

**Pro:**
- Metodo ben noto e testato
- Bassi costi iniziali (strumenti comuni)
- Nessuna educazione "digitale" richiesta
- Espressione personale (ARTE della mappatura)

**Contro:**
- Dati e interpretazioni sono scarsamente distinguibili
- Poche tracce del percorso interpretativo
- Riduzione dei dati nella mappa finale (dall'affioramento alla scala della mappa)
- Limitazioni e incertezze legate alla scala scelta
- Scarsa quantificazione dell'incertezza

### Pro e Contro della Mappatura Digitale

**Pro:**
- Catturare, aggiornare e gestire i dati sul campo, anche per il lavoro di gruppo
- Dati archiviati personalmente dal rilevatore (perdita minima di informazioni)
- Valutazione dei dati con GIS e altri software mentre vengono raccolti
- Controllo del lavoro sul campo
- Importazione di qualsiasi tipo di informazione e sua georeferenziazione (schizzi, foto, pensieri)
- Archiviazione di dati e interpretazioni in diversi layer
- Mantenere la terza dimensione (con il GPS)
- Migliore quantificazione dell'incertezza

**Contro:**
- Fase iniziale del metodo
- Alti costi di avvio (ogni anno si stanno abbassando)
- Strumenti pesanti (ogni anno sono più leggeri)
- Educazione "digitale", a diversi livelli, richiesta
- Visualizzazione standardizzata (nessuna ARTE)

### Workflow per la Mappatura Digitale

#### 1 - Preparazione del lavoro sul campo
- Caricare tutti i documenti: mappe, database, altri progetti, applicazioni
- Preparare un Progetto GIS con tutti i layer e i relativi database (moduli, tabelle, ecc.)
- Considerare tutti i dispositivi che possono essere utilizzati: fotocamera, bussola, GPS, strumenti ad-hoc, batterie supplementari, borsa da trasporto, ecc.
- Non dimenticare di portare anche mappe cartacee e il taccuino da campo (se il sistema digitale va in sciopero)

#### 2 - Sul campo
- Impostare tutti i dispositivi (GPS, Fotocamera, ecc.)
- Rilevare il percorso con il GPS
- Acquisire caratteristiche (punti, linee, poligoni) tramite GPS o "manualmente"
- Catturare dati/info tramite moduli pre-organizzati o tramite tabelle del database
- Descrivere le caratteristiche con note, schizzi, immagini, note vocali...
- Controllare il lavoro in corso e fare backup del progetto frequentemente
- Inviare dati/info a un server centrale o a un operatore indoor se necessario
- Creare layer ad-hoc per caratteristiche inaspettate da mappare

#### 3 - Di nuovo in laboratorio
- Valutare i dati/info acquisiti e verificarne la coerenza
- Creare nuovi layer nel progetto GIS per l'elaborazione e l'interpretazione dei dati/info: in questo modo i dati e l'interpretazione possono essere tenuti separati
- Disegnare mappe e/o esportare dati/info in altre applicazioni per un'elaborazione appropriata
- Valutare se tornare sul campo per verificare o migliorare l'acquisizione dei dati

### Importante

In tempi di "transizione", dagli anni '80 a oggi, il rilevatore sul campo ha lavorato con carte (al massimo con un GPS) e dopo le sue elaborazioni ha passato mappe e dati a un impiegato GIS in grado di digitalizzare, georeferenziare e disegnare una mappa digitale o qualcosa di simile.

Oggi il rilevatore può elaborare il suo progetto finale con molti risultati positivi:
- Molti errori di trascrizione possono essere evitati
- Alcune elaborazioni possono essere meglio sviluppate dalla persona che ha ottenuto direttamente i dati/info
- Se necessario, l'operatore può tornare per verificare o acquisire nuovi dati
- Il tempo di consegna dell'elaborazione finale può essere ridotto

### Strumenti Open Source: BeeGIS

BeeGIS è stato costruito su uDig (User-friendly Desktop Internet GIS), un framework applicativo desktop open source, costruito con la tecnologia Rich Client di Eclipse.

**Plugin di BeeGIS:**
- **beeGPS**: plugin per il GPS
- **beePen**: plugin per disegnare e scrivere a mano libera
- **beeJou**: plugin per il diario di campo
- **beePict**: plugin per geolocalizzare le foto (file EXIF) utilizzando il loro timestamp e la traccia GPS
- **beeDip**: plugin per importare (e future esportazioni) file GeoPackage da BeeDIP, una bussola geologica per Android

### Geopaparazzi per Android

Applicazione per il rilevamento sul campo su dispositivi Android.

<div style="page-break-after: always;"></div>

## 05.02 TABLET PC

### Perché un Tablet PC?

- Si può lavorare con uno stilo, dando una sensazione simile al lavoro tradizionale con matita-su-carta.
- I dispositivi più piccoli (PDA, telefoni cellulari) non sono abbastanza grandi per disegnare o visualizzare un'area sufficiente del territorio; utilizzabili solo quando si devono raccogliere punti o tracce.
- CPU e RAM sono in grado di gestire anche file pesanti di mappe e immagini.

### Quale Tipo di Tablet PC?

Due categorie principali:
- **Convertibile**: con tastiera e schermo rotante
- **Slate**: senza tastiera

**Rugged o ruggedizzato**: se costruiti per un uso intensivo, spesso devono essere conformi agli standard militari (MIL-STD).

### Requisiti per un Buon Tablet PC

- **Buona RAM e CPU**: per gestire file pesanti di mappe TIFF e ortofoto.
- **Schermo abbastanza grande**: almeno 10", ma se troppo grande diventa difficile da gestire sul campo.
- **Alta luminosità e leggibilità dello schermo**: importante sotto il sole.
- **Porte USB, lettori di schede SD**: per backup frequenti del progetto e importazione da fotocamera.
- **Connessione Bluetooth** (anche WiFi direct): per connettere facilmente l'antenna GPS esterna senza cavi.
- **Meglio se RUGGED**: può essere più pesante ma pioggia e polvere sono nemiche del lavoro.

### Borse da Trasporto

Le borse da trasporto sono importanti quando si usano questi PC portatili, perché dopo un po' il peso diventa molto fastidioso. Inoltre, una buona borsa può aiutare a evitare la luce solare diretta sullo schermo e protegge da piccoli urti e graffi.

<div style="page-break-after: always;"></div>

## 05.03 GPS PER IL MOBILE GIS

### Due Metodi Digitali

1. **GPS Professionale con Correzione Differenziale**: Accuratezza sub-metrica.
2. **GPS Personale collegato a Tablet PC**: Accuratezza da 1 a 15 metri.

### Ora

Le antenne GPS collegate via Bluetooth sono più facili da usare (unico problema: i driver). Le ultime generazioni di ricevitori GPS contano 51 canali (Navstar conta solo 31 satelliti) e alcuni di essi possono ricevere anche i segnali Glonass e Galileo. Questi ricevitori possono funzionare anche se tenuti in tasca. WAAS + EGNOS migliorano l'accuratezza.

### GPS nel Tablet Android

La maggior parte dei tablet Android integra un ricevitore GPS.

<div style="page-break-after: always;"></div>

## 06.00 MODELLAZIONE PER LE SCIENZE GEOLOGICHE

### Cos'è la GeoModellazione?

La Modellazione Geologica o GeoModellazione è la scienza applicata che crea rappresentazioni computerizzate di porzioni della crosta terrestre basate su osservazioni geofisiche e geologiche fatte sulla e sotto la superficie terrestre.

La GeoModellazione è comunemente usata per la gestione delle risorse naturali e dei rischi naturali e per quantificare i processi geologici, con applicazioni principali a giacimenti di petrolio e gas, acquiferi e giacimenti minerari.

### Workflow Generale

1. Analisi preliminare del contesto geologico del dominio di studio.
2. Interpretazione dei dati e delle osservazioni disponibili come insiemi di punti o linee poligonali.
3. Costruzione di un modello strutturale che descrive i principali confini rocciosi (faglie, orizzonti, discordanze).
4. Definizione di una mesh tridimensionale che rispetta il modello strutturale per supportare la rappresentazione volumetrica dell'eterogeneità (Geostatistica).

### Geostatistica

Una parte importante della modellazione geologica è legata alla geostatistica. Per rappresentare i dati osservati, spesso non su griglie regolari, dobbiamo utilizzare alcune tecniche di interpolazione. La tecnica più utilizzata è il kriging che utilizza la correlazione spaziale tra i dati e intende costruire l'interpolazione tramite semi-variogrammi. Per riprodurre una variabilità spaziale più realistica e aiutare a valutare l'incertezza spaziale tra i dati, viene spesso utilizzata la simulazione geostatistica.

### Tecnologia

La GeoModellazione e il CAD condividono molte tecnologie comuni. Il software è solitamente implementato utilizzando tecnologie di programmazione orientata agli oggetti in C++, Java o C#. L'interfaccia utente grafica consiste generalmente in una o più finestre grafiche 3D e 2D per visualizzare dati spaziali, interpretazioni e output della modellazione.

### Applicazioni

- Esplorazione e sfruttamento di idrocarburi
- Valutazione degli acquiferi
- Geologia ingegneristica (cava, stabilità, gallerie, ecc.)
- Inquinamento terrestre e marino

<div style="page-break-after: always;"></div>

## 06.01 MODELLAZIONE 2D

### 2D MOVE

2D MOVE è un programma per la modellazione della geologia in 2 dimensioni:
- Mappe
- Sezioni
- Analisi strutturale

### Mappe: Workflow per l'Importazione di Dati

1. **Dati sul campo**: convertire i dati sul campo raccolti con GIS (punto.shape → .mve; linea.shape → .mve).
2. **Proiettare i Dati di Immersione (punti) sul DEM** → 3Dmove.
3. **Controllare e ricampionare i Limiti (linee)** → 2Dmove.
4. **Costruire le sezioni trasversali e disegnarle** - 2Dmove.
5. **Utilizzare i nuovi limiti e/o le sezioni trasversali per costruire il modello 3D**.

### Mappe: Importazione di Mappe Topografiche

La CTR regionale ha formato vettoriale .DWG in due versioni:
- **2D**: linee e punti non hanno attributi di altitudine, ma hanno la giusta simbologia.
- **3D**: ogni caratteristica ha anche attributi di altitudine (preferibile per la modellazione). Convertire .DWG → .DXF.

### Sezioni

Le sezioni da mappa e dati possono essere generate utilizzando 2D Move. La sezione raccoglie l'intersezione di curve di livello, confini geologici, faglie, ecc.

### Analisi Strutturale: Restauro e Bilanciamento

- Utilizzare algoritmi "Move on fault" per ripristinare i dislocamenti delle faglie.
- Utilizzare algoritmi di "Unfolding" per recuperare la deformazione duttile.

<div style="page-break-after: always;"></div>

## 06.02 MODELLAZIONE 2.5D

### Modellazione 2.5D

Articolo: "Describing the dimensionality of geospatial data in the earth sciences—Recommendations for nomenclature" (Jones et al., Geosphere, 2008).

Un piano è considerato 2D, una superficie irregolare (dimensione topologica tradizionale anch'essa 2D) copre più spazio 3D rispetto al piano, ma non riempie completamente un volume 3D: quindi la sua dimensione frattale è compresa tra 2 e 3.

I set di dati DEM sono spesso descritti come "2½D". I valori di altezza del DEM vengono utilizzati per estendere un'immagine aerea 2D (foto o dati satellitari) lungo l'asse Z per dare un "drappeggio 2½D". Un fattore chiave è che le comuni strutture di dati DEM spesso non sono in grado di accogliere valori Z multipli.

### Da 2D MOVE a 3D MOVE

- Importare una mappa con attributi di elevazione associati alle sue caratteristiche.
- Importare le caratteristiche (linee e punti) nel DEM.
- I dati 2D dal livello 0 alla superficie DEM.

### Drappeggio di Immagini sul DEM

<div style="page-break-after: always;"></div>

## 06.03A MODELLAZIONE 3D

### 3D MOVE

3D MOVE è un programma per la modellazione della geologia in 3 dimensioni:
- Importare e inserire dati
- DEM e sezioni
- Creare superfici

### Creare una Superficie

1. Selezionare "Create Surface".
2. Selezionare "PolyLine" o "VertexCloud".
3. DEM → "Mesh" → selezionare la superficie appena creata.

### Importare Sezioni Trasversali

Le sezioni possono mostrare dati di immersione (cerchi) e caratteristiche geologiche (linee) come confini di formazioni, strati chiave, faglie, ecc. Le sezioni sono georeferenziate e importate direttamente nelle giuste posizioni.

### Costruire una Mappa 3D

- Importare elementi lineari dalla mappa.
- Disegnare una mappa geologica sul DEM (2.5 dimensioni).
- Creare superfici.

### Modellazione Strutturale 3D

- Move on fault.

<div style="page-break-after: always;"></div>

## 06.03B MODELLAZIONE N-DIMENSIONALE

### Nuove Dimensioni nella Modellazione

Più dimensioni rispetto alle solite dimensioni spaziali possono migliorare il lavoro di modellazione:
- Tempo
- Denaro
- Rischio per siti contaminati
- Ecc.

### Tempo

**Restauro Sequenziale (4D Restoration)**: miglioramento del back-stripping di successivi restauri 3D nel tempo (3D + tempo = 4D).
- Controllo di qualità dell'interpretazione sismica o del modello strutturale.
- Derivare l'evoluzione della deformazione nel tempo.

#### Back-stripping
- Modo tradizionale per ripristinare la geometria del bacino nel tempo geologico.
- Assume che tutta la deformazione sia lungo l'asse verticale.
- Fornisce la geometria nel passato.
- Non gestisce le faglie come discontinuità.
- Viene calcolato con il minimo sforzo da parte dell'utente.

#### Restauro 2D o 3D
- Gestisce la geometria 2D o 3D di faglie e orizzonti.
- Appiattisce un orizzonte e annulla il movimento della faglia.

#### Restauro 4D
- Gestisce la geometria 2D o 3D di faglie e orizzonti.
- Appiattisce un orizzonte e annulla il movimento della faglia.
- Risultati: geometria di faglie e strati nel tempo, possibilità di individuare aree interpretate erroneamente, modelli di deformazione.

### Denaro

Valutazione dei costi per la costruzione di un tunnel ferroviario negli Appennini.

### Analisi Statistica: Da Pixel a Voxel

- **Voxel**: elemento volumetrico (Volumetric Pixel o Volumetric Picture Element).
- Siti contaminati: ogni voxel ha attributi diversi (es. litologia).
- Con l'analisi statistica delle caratteristiche di ogni voxel (porosità, permeabilità, densità, ecc.) si può stimare la diffusione degli inquinanti.

<div style="page-break-after: always;"></div>

## GIS E WEBGIS

### GIS: Sistema Informativo Geografico

Un sistema informativo geografico (GIS) è un sistema informatico utilizzato per raccogliere, archiviare, processare e analizzare dati spaziali/geografici, ovvero dati che possono essere riferiti a una particolare posizione sulla Terra (Longitudine + Latitudine + SR* oppure X + Y [+ Z] + SR*).

* SR: Sistema di Riferimento delle Coordinate

### Database Spaziale

Un Sistema Informativo (SI) gestisce dati testuali, numerici e data+datetime (database non-spaziali). L'introduzione del tipo di dato geografico o geometrico ('geography' data type o 'geometry' data type) e delle funzionalità necessarie per gestirlo, ha portato allo sviluppo dei database spaziali gestiti mediante Sistemi Informativi Geografici (GIS).

- **geography**: per memorizzare dati con coordinate sferiche (Longitudine e Latitudine).
- **geometry**: per memorizzare dati con coordinate piane (X e Y).

### WebGIS

Un WebGIS è una forma avanzata di Sistema Informativo Geografico disponibile su piattaforme web. Utilizza la tecnologia Web per mettere in comunicazione un Server GIS e un Client (browser Web o applicazione desktop/mobile). La comunicazione avviene tramite HTTP/HTTPS.

**Servizi standard OGC (Open Geospatial Consortium):**
- **WMS (Web Map Service)**: servizio di visualizzazione, navigazione, zoom, pan, sovrapposizione di set di dati territoriali.
- **WFS (Web Feature Service)**: servizio di download di copie di set di dati territoriali (formato GML).
- **WCS (Web Coverage Service)**: servizio di download di dati continui (coverage).

### Middleware

Software che operano come livelli intermedi tra client e server e tra software e database.

- **Geoserver**: scritto in Java, condivide, elabora e modifica dati geospaziali. Pubblica dati da tutti i principali formati utilizzando standard aperti.
- **QGIS Server**: implementazione open source di WMS, WFS, WFS3 e WCS che utilizza le funzionalità cartografiche di QGIS.
- **Apache Tomcat**: server web per applicazioni Java.

### Software Client

- **QGIS**: software GIS desktop che funziona con le principali versioni di sistemi operativi e dispositivi. Scritto in C++, Python e Qt. È anche client di QGIS Server e Geoserver.

### Utility a Riga di Comando

- **GDAL/OGR**: librerie per la lettura e scrittura di formati di dati geospaziali raster e vettoriali.
- **Shp2pgsql**: strumento per la conversione di shapefile in SQL per l'inserimento in database PostGIS/PostgreSQL.

### Librerie JavaScript

- **Leaflet**: libreria leggera per lo sviluppo di mappe interattive sul web.
- **OpenLayers**: libreria per inserire mappe dinamiche in pagine web, può visualizzare mappe e dati vettoriali da qualsiasi fonte, può essere connessa a Geoserver.

<div style="page-break-after: always;"></div>

## I FORMATI DEI FILE GIS

### Formati File nei GIS

Un formato file GIS è uno standard di codifica delle informazioni geografiche in un file digitale. Ne esistono di diversi tipi per memorizzare dati vettoriali e raster. Anche i dati non spaziali (tabelle senza geometrie) hanno i loro formati: .txt, .csv, .dbf, .xlsx.

### Formati Vettoriali: Shapefile

Lo shapefile è un formato ideato da ESRI, reso pubblico per semplificare lo scambio di dati. È composto da diversi file con lo stesso nome ma estensioni diverse:

- **.shp**: memorizza le forme geometriche (punti, linee, poligoni).
- **.dbf**: memorizza la tabella degli attributi associati agli elementi geometrici.
- **.shx**: contiene l'indice dei record della tabella e degli elementi geometrici.

**File opzionali:**
- .prj: informazioni sul sistema di riferimento.
- .sbn, .sbx, .qix: indici spaziali.
- .shp.xml: metadati.

**Limitazioni dello Shapefile:**
- Nomi degli attributi massimo 10 caratteri.
- Campi di tipo stringa massimo 255 caratteri.
- Non gestisce informazioni topologiche.
- Aumento dei tempi di visualizzazione con molti elementi.
- Massimo 2 GB di dati.

### Formati Vettoriali: GeoPackage

Il GeoPackage (.gpkg) è un formato per dati geopaziali vettoriali aperto, non proprietario, indipendente dalla piattaforma. È diventato il formato predefinito di QGIS.

- Può contenere più dataset vettoriali e anche raster.
- Può contenere tabelle non spaziali.
- È un singolo file che memorizza un numero ipoteticamente infinito di layer di tipo diverso.
- È un database in senso stretto, con tabelle e relazioni.

### Altri Formati Vettoriali

- **GML (.gml)**: Geography Markup Language, formato standard aperto leggibile come testo, descrive oggetti geografici.
- **KML (.kml, .kmz)**: Keyhole Markup Language, formato specifico per Google Earth e Google Maps, può contenere informazioni tridimensionali.
- **CSV (.csv)**: comma-separated values, formato di testo tabellare contenente coordinate x e y di punti (un punto = una riga). Tipico file in uscita da strumenti di monitoraggio e rilievo.

### Formati Raster

- **TIFF (.tif)**: formato molto diffuso, utilizzato soprattutto per cartografia in bianco e nero o con pochi colori. Nei GIS, un file .tif è associato al worldfile (.tfw o .wld) per la georeferenziazione. **GeoTIFF**: versione che archivia al suo interno anche le informazioni di georeferenziazione.
- **JPEG (.jpg)**: ideale per immagini a molti colori, permette una notevole compressione. Nei GIS, accompagnato dal worldfile (.jpw o .wld). **JPEG2000 (.jp2, .j2f)**: garantisce una minor perdita di qualità con la compressione.
- **ECW (.ecw)**: Enhanced Compression Wavelet, formato proprietario per immagini satellitari e foto aeree, alta compressione con bassa perdita di qualità.
- **MrSID (.sid)**: Multi-Resolution Seamless Image Database, formato ottimizzato per raster di grandi dimensioni, alta compressione e velocità di visualizzazione.
- **ESRI GRID**: formato proprietario ESRI, esiste in binario (ARC/INFO GRID, .adf) e ASCII (ARC/INFO ASCII GRID, .asc), utilizzato per analisi spaziali e geoprocessamento.

### Formato Raster ASCII (.asc)

È un file di testo, leggibile con un editor di testo. Contiene:
- ncols: numero di colonne
- nrows: numero di righe
- xllcorner, yllcorner: coordinate dell'angolo di ancoraggio georiferito
- cellsize: dimensione della cella
- valori delle celle (riga per riga)