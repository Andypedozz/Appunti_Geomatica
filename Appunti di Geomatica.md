# Introduzione

## Geomatica
La geomatica è la disciplina di raccolta, salvataggio, elaborazione e consegna di informazioni geografiche, o spazialmente referenziate.

E' un termine relativamente recente, coniato da Pollock e Wright nel 1969. Essa include strumenti e tecniche usate nello studio del territorio, remote sensing, cartografia, sistemi GIS, sistemi di satelliti globali, fotogrammetria, geografia e altre forme di mappatura della Terra.

# Cartografia

## Definizione
La cartografia è lo studio e la pratica di produrre mappe. Combinando scienza, estetica e tecnica, la cartografia si basa sul fatto che la realtà può essere modellata in modi che comunichino le informazioni spaziali efficientemente.

## Scale delle mappe
Una mappa rappresenta una porzione della superficie terrestre. Dato che una mappa accurata rappresenta il terreno, ogni mappa ha una "scala" che indica il rapporto tra una certa distanza sulla mappa e la distanza sul suolo reale.

### Representative Fraction (FR)
Indica a quanto un certo numero di unità della superficie terrestre corrispondano sulla mappa. Può essere espressa cpme 1/100.000 o 1:100.000. In quwesto esempio, un centimetro sulla mappa equivale a 100.000 centimetri (1 chilometro) sulla terra.

### Graphic Scale
E' una rappresentazione visuale della scala della mappa.

### Larga scala o piccola scala
Una mappa in larga scala è una mappa che mostra maggiore dettaglio in quanto la frazione rappresentativa (come 1/25.000) è una frazione maggiore rispetto a una mappa in piccola scala, che avrebbe una frazione da 1/250.000 a 1/7.500.000. Le mappe a larga scala hanno una frazione rappresentativa di 1/50.000 o anche 1/10.000. Quelle tra 1/50.000 e 1/250.000 si dicono mappe a scala intermedia.

### Mappa Topografica

<div style="page-break-after: always;"></div>

### Proiezioni
Una proiezioni di una mappa è un qualsiasi metodo di rappresentazione della superficia di una sfera o di un altro oggetto tridimensionale, su un piano.

Tutte le proiezioni di mappe distorcono la superficie originale in qualche modo. A dipendenza dallo scopo della mappa, alcune distorsioni sono accettabili e altre no; perciò diverse proiezioni esistono per preservare alcune proprietà di interesse del corpo studiato, a spese di altre.

Non c'è limite al numero possibile di proiezioni di una mappa.

Molte proprietà possono essere misurate sulla superficie terrestre:
* Area
* Forma
* Direzione
* Angoli
* Distanze
Le proiezioni di mappe possono essere costruite per preservare una o molteplici di queste proprietà, ma non tutte simultaneamente.

Lo scopo della mappa determina quale proiezione dovrebbe costituire la base per la mappa. Dato che una mappa può avere molti scopi diversi, molte diverse proiezioni sono state create per soddisfare questi scopi.

* Conformal: preserva gli angoli localmente (i.e UTM - Universal Transversal Mercator)
![alt text](image-1.png)
* Equal-Area: preserva le aree<br>
![alt text](image-2.png)
* Equidistant: preserva la distanza da un punto o una linea standard
![alt text](image-3.png)

<div style="page-break-after: always;"></div>

## Coordinate
![alt text](image.png)

### Latitudine
La latitudine di un punto sulla terra indica il valore dell'angolo tra il piano equatoriale e una linea che passa attraverso quel punto ed è normale alla superficie di un elissoide di riferimento che approssima la forma della terra.

### Longitudine
La longitudine di un punto sulla terra indica l'angolo est o ovest da un meridiano di riferimento a un altro meridiano che passa attraverso quel punto.

### Coordinate Polari (sferoide)<br>
![alt text](image-4.png)

<div style="page-break-after: always;"></div>

## Sistema di Riferimento a Coordinate
Un CRS è un sistema globale, regionale o locale, basato su coordinate, per localizzare entità geografiche.

Ci si può riferire a un CRS usando codici EPSG definiti dall' European Petroleum Surbey Group.

## Sistemi di Riferimento in Italia
Il sistema Gauss-Boaga è stato proposto dal prof. Giovanni Boaga, capo dell'Istituto Geografico Militare, nel 1940. Il sistema Gauss Boaga definisce anche il sistema geodetico Roma 40. Le mappe IGM a scala 1:25.000 sono state pubblicate usando le coordinata Gauss-Boaga, poi trasformate in UTM.
Sono coordinate metriche che esprimono un punto come una distanza dal vertice geodetico di Monte Mario.
Ci sono due zone principali in questo sistema, ovvero il fuso Ovest e il fuso Est. L'evoluzione della cartografia italiana ha poi adottato il sistema di coordinate UTM.

L'EPSG mantiene dati nei propri database di quasi tutti i CRS:
* Gauss-Boaga
* EPSG 3003 (fuso Ovest)
* EPSG 3004 (fuso Est)

L'Universal Transverse Mercator (UTM) usa un sistema cartesiano bidimensionale per localizzare entità sulla superficie Terrestre.

Il sistema UTM non è una singola proiezione cartografica. Il sistema invece divide la Terra in sessanta zone, ciascuna una fascia di sei gradi di longitudine, e utilizza una proiezione di Mercatore trasversa secante in ogni zona.

L'Italia è compresa in due principali fasce, l'UTM 32 e l'UTM 33 (+34).

Latitudine e longitudine vengono espresse in angoli (gradi, minuti e secondi).

### WGS
Il WGS 84 (World Geodetic System) è un sistema di riferimento a coordinate usato dal GPS (Global Positioning System).

## Simbologia
* Orografia
* Idrografia
* Amministrazione
* Urbanistica
* Strade
* Vegetazione
* Geodetica

### Orografia
* Isolinee e punti con altimetria
* Alla scala di 1:25.000 le curve di livello hanno un'equidistanza di 25 m.
* Alla scala di 1:10.000 le curve di livello hanno un'equidistanza di 10 m
![alt text](image-5.png)

### Idrografia
Fiumi, torrenti, sorgenti, laghi, mare, ecc.

### Amministrazione
Confini:
![alt text](image-6.png)

### Urbanistica
Costruzioni e molto altro...

<div style="page-break-after: always;"></div>

## Leggere una mappa
1 Step
* Posizione geografica dell'area di studio
* Scala e dimensioni
* Equidistanza e linee di contorno

2 Step
* Prima definizione dei principali elementi di orografia
* Pendenza dei versanti
* Interpretazione analitica dell'orografia e dell'idrografia
* Affioramenti rocciosi
* idrologia e suoi modelli
* tipi di vegetazione
* elementi antropici

3 step
* Interpretazione delle forme e dei processi
    * geomorfologia
    * attività umane
    * elementi seminaturali
        * confronto con altre fonti: carte tematiche, dati statistici, bibliografia...

<div style="page-break-after: always;"></div>

# 01.02 TELERILEVAMENTO

**TELERILEVAMENTO**
* Definizione
* Storia
* Tipi
* Applicazioni
* Tecniche
* Fotogrammetria aerea e fotointerpretazione
* Immagini e dati satellitari
* Sistemi LiDAR

## Definizione
Il telerilevamento, in generale, può essere definito come la raccolta di informazioni da un oggetto o una superficie senza contatto diretto.

Il telerilevamento (osservare-osservare, senza contatto) è un campo molto più ampio di quanto verrà trattato in questo corso. Ci concentreremo su quella parte del telerilevamento che riguarda le
**SCIENZE DELLA TERRA E DELL’AMBIENTE**

Rilevamento tramite suono e onde radio

## Storia
1858: il balloonista G. Tournachon realizzò fotografie di Parigi dal suo pallone.

* La fotografia aerea sistematica si sviluppò per scopi militari e di ricognizione a partire dalla Prima Guerra Mondiale, raggiungendo il massimo durante la Guerra Fredda.
* Satelliti artificiali nella seconda metà del XX secolo.

## Applicazioni
* Geologia
* Silvicoltura
* Agricoltura
* Idrologia
* Rilievo marino
* Copertura e uso del suolo
* Scopi militari …

## Tipi

* **Telerilevamento passivo**
Fotografia
* Radiometri
* Infrarosso

* **Telerilevamento attivo**
RADAR
* LiDAR

## Elementi di interpretazione delle immagini

**Forma:**
Molte caratteristiche naturali e artificiali hanno forme uniche.
Si usano spesso aggettivi come lineare, curvilineo, circolare, ellittico, radiale, quadrato, rettangolare, triangolare, esagonale, a stella, allungato e amorfo.

**Ombra:**
La riduzione delle ombre è importante nel telerilevamento perché le ombre tendono a nascondere oggetti che altrimenti potrebbero essere rilevati.
Tuttavia, l’ombra proiettata da un oggetto può essere l’unico indizio reale della sua identità.
Le ombre possono anche fornire informazioni sull’altezza di un oggetto, sia qualitativamente che quantitativamente.

**Tono e colore:**
Una banda di radiazione elettromagnetica registrata da uno strumento di telerilevamento può essere rappresentata in un’immagine in scale di grigio dal nero al bianco.
Queste scale sono chiamate “toni” e possono essere descritti qualitativamente come scuri, chiari o intermedi (l’uomo può distinguere 40-50 tonalità).
Il tono è legato alla quantità di luce riflessa dalla scena in un determinato intervallo di lunghezze d’onda (banda).

**Texture:**
La texture si riferisce alla disposizione dei toni o dei colori in un’immagine.
È utile perché elementi della superficie terrestre con toni simili spesso presentano texture diverse.
Aggettivi: liscia (uniforme, omogenea), intermedia e ruvida (grossolana, eterogenea).

**Altezza e profondità:**
Come discusso, le ombre possono fornire indizi sull’altezza degli oggetti.
Le altezze relative possono quindi essere usate per interpretare gli oggetti.
In modo simile, anche le profondità relative possono essere interpretate.
Descrizioni: alto, medio, basso; profondo, medio, superficiale.

**Associazione:**
Molto importante nell’interpretazione di un oggetto o attività.
Si riferisce al fatto che alcune caratteristiche e attività sono quasi sempre associate alla presenza di altre caratteristiche e attività.

**Tecniche**
* Fotogrammetria aerea e fotointerpretazione
* Immagini satellitari
* Interferometria radar
* Sistemi LiDAR

### Fotogrammetria aerea

**Molto precisa**
* Rappresentazione 3D
* Efficiente in termini di tempo
* Economica
* Basata su algoritmi consolidati e testati
* Minore sforzo manuale
* Maggiore fedeltà geografica

**Cos’è la fotogrammetria**
Photos – luce
Gramma – disegnare
Metron – misurare

“La fotogrammetria è la tecnica di misurare oggetti a partire da fotografie”

“L’arte, la scienza e la tecnologia per ottenere informazioni spaziali affidabili su oggetti fisici e sull’ambiente attraverso i processi di registrazione, misurazione e interpretazione dei dati di immagine.”

### Tipi di fotogrammetria

**Fotogrammetria aerea:**
La camera è montata su un velivolo e generalmente orientata verticalmente verso il suolo. Vengono scattate più foto sovrapposte lungo la traiettoria di volo.
Queste immagini sono elaborate con uno stereoplotter (strumento che consente la visione stereoscopica).
Sono usate anche per la creazione automatica di Modelli Digitali di Elevazione (DEM).

**Fotogrammetria a distanza ravvicinata:**
La camera è vicina al soggetto ed è spesso portatile o su treppiede.
Generalmente non produce prodotti topografici, ma disegni e modelli 3D.
Utilizzata per edifici, strutture ingegneristiche, veicoli, scene forensi, set cinematografici, ecc.

**Fotografia stereoscopica**
Le foto aeree adiacenti ma sovrapposte sono chiamate coppie stereoscopiche e servono per determinare la parallasse e la visione 3D.

**Sovrapposizioni:**
* Endlap ~60-80% (nota: nel testo ~480% probabilmente errore)
* Sidelap ~20-30%

**Vecchie pellicole**
a. pancromatica
b. infrarosso b/n
c. pancromatica a colori
d. infrarosso a colori

**Estrazione digitale delle caratteristiche**
* Edifici
* Trasporti
* Idrografia
* Servizi
* Vegetazione
* Breaklines
* Punti DTM
* Ponti

### Vettoriale vs Raster
I dati raster sono descritti da una griglia di celle, un valore per cella

Vettore: punto, linea, poligono
Raster: zona di celle

### Curve di livello (isoipse)
Le curve di livello sono linee che collegano punti di uguale quota.
Sono utili per rappresentare la forma della superficie terrestre (topografia).
La distanza verticale tra curve è l’intervallo di livello.
Se è 10 m, le curve saranno multipli di 10 (0, 10, 20…).
In zone con forte rilievo l’intervallo è maggiore.

### Estrazione (pseudo) 3D – DTM & DEM
Non esiste una definizione univoca di DEM, DTM e DSM.

* DSM: rappresenta la superficie terrestre (inclusi oggetti)
* DTM: rappresenta il terreno nudo
* DEM: termine generico per l’altitudine

**Modellazione 3D urbana**

**Generazione di ortofoto**
Il risultato della fotogrammetria è generalmente una mappa, un disegno o un modello 3D di un oggetto o scena reale.
Molte mappe moderne sono create con fotogrammetria e fotografie aeree.

**Limitazioni delle ortoimmagini**
Le ortoimmagini hanno limitazioni geometriche: mostrano correttamente solo elementi alla quota del DEM utilizzato.
Gli edifici non inclusi nel DEM risultano spostati in base all’angolo di vista e alla loro altezza.
Se l’altezza del tetto è inclusa nel DEM, esso appare nella posizione corretta.
Questo però può causare perdita di informazioni per parti precedentemente nascoste.

**Correzione delle ortoimmagini**
* Posizione edificio non corretta vs corretta
* Correzione di ponti rispetto alla strada sottostante

# 01.03 TELERILEVAMENTO: dati satellitari

## Immagini satellitari

### Sistema ottico: telerilevamento passivo
Il telerilevamento ottico utilizza sensori nel visibile, nel vicino infrarosso e nell’infrarosso a onde corte per creare immagini della superficie terrestre rilevando la radiazione solare riflessa dagli oggetti al suolo.

### Orbite dei satelliti
Il percorso seguito da un satellite è chiamato orbita.

Le orbite geostazionarie, a circa 329.000 km di altitudine, ruotano a velocità tali da eguagliare la rotazione terrestre.

La maggior parte dei satelliti per telerilevamento oggi si trova in orbite quasi polari: il satellite si muove verso nord su un lato della Terra e verso sud nell’altra metà dell’orbita.
Questi passaggi sono chiamati rispettivamente passaggi ascendenti e discendenti.

### Immagini satellitari

**Pancromatica**
* Viene utilizzato un sensore a canale singolo per rilevare la radiazione
* Se l’intervallo di lunghezze d’onda coincide con il visibile, l’immagine appare come una fotografia in bianco e nero scattata dallo spazio

**Multispettrale**
* Utilizza un rilevatore multicanale
* Registra la radiazione in intervalli ristretti
* Fornisce informazioni su luminosità e colore

**Risoluzione spaziale**
Area minima al suolo visibile dal sensore

**Quickbird: pancromatica – risoluzione 293 cm**

**Risoluzione radiometrica**
Descrive la capacità di un sistema di distinguere piccole differenze di energia.
Maggiore è la risoluzione radiometrica, maggiore è la sensibilità nel rilevare piccole variazioni di energia riflessa o emessa.

**Risoluzione spettrale**
Descrive la capacità del sensore di distinguere intervalli di lunghezza d’onda molto piccoli.
Maggiore è la risoluzione spettrale, più stretta è la banda di lunghezze d’onda per ciascun canale.

**Risoluzione temporale**
È il tempo necessario affinché il sistema osservi di nuovo la stessa area con lo stesso angolo.

Esempio:
2 luglio → 18 luglio → 3 agosto
129 giorni

Oppure:
1 luglio → 12 luglio → 23 luglio → 3 agosto
11 giorni

**Missioni satellitari**

1. **Terra:**
   Landsat (1-29) (1973); Seasat (1978); HCMM (1978); SPOT (Francia) (1-3);
   RESURS (Russia) (1985); IRS (India); ERS (1-2) (1991);
   JERS (Giappone) (1992); Radarsat (Canada) (1995); ADEOS (Giappone).
   (Nota: SIR-A, SIR-B, SIR-C).

2. **Meteo:**
   TIROS, Nimbus, ESSA, ATS, DMSP, Kosmos, Meteor, ITOS, SMS, GOES, NOAA,
   GMS (Giappone), Meteosat (Europa), Bhaskura (India), Insat, ERBS, MOS, UARS, TRMM.
   (Nota: g = geostazionario).

3. **Oceanografia:**
   Seasat, Nimbus 7 (CZCS), Topex-Poseidon, SeaWiFS.

**Esempio**

**Landsat**

**Software per analisi di immagini**

**OPTICKS**
Piattaforma open source per analisi di immagini e telerilevamento.

Supporta formati: NITF, GeoTIFF, ENVI, HDF5, JPEG, PNG, BMP ecc.

* Zoom, pan e rotazione di grandi dataset
* Sovrapposizione di dati GIS
* Controlli avanzati (colormap, istogrammi, trasparenza)
* Supporto per file > 4 GB
* Procedure guidate per analisti
* Supporto formati BIP, BSQ, BIL
* Estensioni per nuove funzionalità

[www.opticks.org](http://www.opticks.org)

**Sistema RADAR**
* RAdio Detection And Ranging
* Sistema che utilizza onde elettromagnetiche per determinare distanza, direzione o velocità

### SAR (Radar ad apertura sintetica)
È un tipo di radar che utilizza il movimento relativo tra antenna e bersaglio per ottenere alta risoluzione spaziale grazie alla coerenza del segnale nel tempo.

### SAR su satelliti
Dati SAR (ampiezza) non sono quasi influenzati da illuminazione solare o condizioni meteo.

### SATELLITI

**Vecchia generazione**
Sensori semplici, capaci di creare archivi storici.

**Nuova generazione**
Macchine potenti (es. Envisat: 2.3 miliardi USD)
Molto complesse, con molte modalità di acquisizione
Nessuna politica di acquisizione standard

**Radarsat: copertura italiana**
* >2000 acquisizioni pianificate
* >1000 immagini disponibili
* Passaggi ascendenti e discendenti

### Interferometria Repeat-Pass
Rilevamento del movimento del suolo tramite confronti temporali

Problemi:
* Effetti atmosferici
* Differenze geometriche

### Generazione interferogramma differenziale

Ingredienti: 2 immagini SAR + DEM

Procedura:

1. Creazione interferogramma
2. Generazione interferogramma sintetico dal DEM
3. Sottrazione per isolare deformazioni

Problemi:
* Precisione del DEM
* Allineamento immagini
* Effetti atmosferici

### Esempio: terremoto Landers (1992)
Interferogramma differenziale ERS
Topografia compensata
Georeferenziato

### Tecnica degli scatter permanenti (PS)
Utilizza serie temporali lunghe di dati SAR per identificare punti stabili e misurare deformazioni con alta precisione.

### Esempi di PS
* Tralicci elettrici
* Tetti metallici
* Impianti idroelettrici
* Danni strutturali

### Processamento PS
* Stima DEM
* Selezione PS
* Analisi pixel per pixel
* Interpolazione e filtraggio
* Analisi temporale
* Output GIS

### Movimenti verticali
* Fronte di subsidenza
* Fronte di sollevamento

### Monitoraggio frane (lento)
Velocità media LOS [mm/anno]
+7 / -7 mm/anno
Punto di riferimento stabile

### Subsidenza
Classi:
< -3 mm/anno fino a > +3 mm/anno

I dati PS possono essere sovrapposti a immagini ottiche ad alta risoluzione.
Serie temporali di spostamento (1993–2000).

### Dinamica delle faglie
Esempio: Baia di San Francisco (California)

### Applicazioni
* Protezione civile
* Pubbliche amministrazioni e ricerca
* Compagnie assicurative
* Industrie petrolifere
* Ingegneria
* Utenti finali

# 02. LIDAR

## SCANSIONE LASER

## LIDAR

### LIDAR
Il LIDAR (LIght Detection And Ranging) è una tecnologia che consente di determinare la distanza da un oggetto tramite emissioni laser.

* LASER – Amplificazione della luce mediante emissione stimolata di radiazione

### LIDAR: Come funziona?

Ogni volta che il laser emette un impulso:

* Il laser genera un impulso ottico
* L’impulso viene riflesso da un oggetto e ritorna al ricevitore
* Un contatore ad alta velocità misura il tempo tra impulso emesso e ricevuto
* Il tempo viene convertito in distanza (la distanza dal bersaglio e la posizione dello scanner permettono di determinare quota e posizione)
* È possibile registrare più ritorni per ogni impulso
* Tutto ciò che è visibile dalla posizione dello strumento viene misurato

### LIDAR vs Fotogrammetria tradizionale

**LiDAR**
* Acquisizione dati giorno e notte
* Acquisizione diretta 3D
* Maggiore accuratezza verticale rispetto a quella planimetrica
* Nuvole di punti difficili da interpretare semanticamente, ma con valori di intensità utili per immagini

**Fotogrammetria**
* Solo acquisizione diurna
* Procedure complesse e talvolta poco affidabili
* Accuratezza planimetrica maggiore di quella verticale
* Ricca di informazioni semantiche

### Due tipi principali
* Scanner laser terrestre
* Scanner laser aerotrasportato

### Scanner laser terrestre

**Principio**
Velocità = spazio / tempo
Spazio = velocità × tempo / 2

Componenti:
* Diodo laser (emettitore)
* Fotodiodo (ricevitore)
* CPU
* Clock

**Risultato finale dell’acquisizione**

* Una **nuvola di punti**
* Ogni punto ha coordinate x, y, z rispetto allo strumento
* Ogni punto ha proprietà di riflettanza (colore, rugosità, umidità)

**Applicazioni**
* Architettura
* Archeologia
* Geologia (es. monitoraggio frane, analisi affioramenti)
* Calcolo volumi
* Industria
* Analisi deformazioni

**Esempio**
Rilievo delle Grotte di Frasassi

### LIDAR aereo

**Applicazioni**
* Geologia
* Silvicoltura
* Agricoltura
* Idrologia
* Rilievo marino
* Copertura e uso del suolo
* Scopi militari

**Componenti del sistema LIDAR aereo**
* Aeromobile
* Unità laser (emettitore-ricevitore)
* GPS differenziale
* Unità di misura inerziale (IMU)
* Computer

**Accuratezza complessiva**

* Posizione (X,Y,Z) di ogni punto:

* 50–100 cm orizzontale
* 10–15 cm verticale

* Superficie del terreno (bare earth):

* Problema di definizione (erba, rocce, ceppi?)

* Altezza degli alberi:

* Sottostima di 0.5–2 m
* Errore dipendente dalla specie

**Prodotti derivati dal LIDAR aereo**

I sistemi topografici LiDAR producono dati di elevazione (x, y, z).
Da questi si derivano vari prodotti:

* Modelli digitali di elevazione (DEM)
* Modelli digitali del terreno (DTM)
* Reti triangolari irregolari (TIN)
* Breaklines (linee caratteristiche, es. creste o fiumi)
* Curve di livello
* Rilievo ombreggiato
* Pendenza e esposizione

**Echi multipli**
Il LiDAR può registrare più ritorni dallo stesso impulso (es. vegetazione + suolo).

**Prodotti derivati (definizioni)**

* DEM / DTM: superficie del terreno (“ground”)
* DSM: superficie superiore (“top surface”)

In terreno aperto: separazione tra aria e suolo

Il DEM differisce dai punti laser misurati per vari motivi:

1. Filtraggio (classificazione punti terreno/non terreno)
2. Base per generare DTM e identificare oggetti topografici

**Visualizzazione**

* Rilievo ombreggiato e illuminazione DEM sono tecniche semplici
* Metodi soggettivi
* Sensibili ai parametri hardware

**Analisi successive e validazione a terra**

* Una volta disponibile il DTM/DEM, si può usare il GIS per analisi e modellazione

* Corsi d’acqua
* Frane

* È sempre necessario valutare l’accuratezza (idealmente con verifica sul campo)

## UAV

## Velivolo Senza Equipaggio

## Nascita militare

Nel 1849 l'Austria inviò palloni senza equipaggio carichi di bombe per attaccare Venezia. Le innovazioni dei UAV iniziarono all'inizio del 1900 e si concentrarono originariamente sulla fornitura di bersagli per l'addestramento del personale militare.

Lo sviluppo dei UAV continuò durante la Prima Guerra Mondiale, quando la Dayton-Wright Airplane Company inventò un siluro aereo senza pilota che sarebbe esploso in un tempo preimpostato.

## 2 tipi principali

●Ala fissa
●Multi-rotore

## Ala fissa

Le ali fisse o "droni a tutt'ala" hanno il vantaggio di essere più produttivi, infatti la capacità di planare e quindi di accendere e spegnere i motori consente al velivolo di rimanere più tempo in quota. Questo si traduce in più ettari rilevati in ogni singola missione. Questo tipo di drone è anche più veloce nella navigazione. Finora possiamo montare su droni ad ala fissa sensori fotografici, termici, multispettrali. Il grande limite rispetto a un multirotore è la possibilità di stazionare su un punto per analizzare con calma un oggetto.

## Multi-rotore

I multi-rotori possono avere da 3 a 8 eliche e presentano diversi vantaggi tra cui:
- la capacità di rimanere sopra un punto o muoversi lentamente; questa caratteristica consente di eseguire analisi e acquisire informazioni aggiuntive. Ad esempio, se è necessario misurare pannelli solari, un dettaglio strutturale di un ponte o una turbina eolica, con un drone ad ala fissa non sarebbe possibile.
- la fotocamera può essere ruotata in più direzioni; potendo ruotare la fotocamera dalla posizione verticale a quella orizzontale è possibile misurare anche tutti gli oggetti verticali. Esempio: monumenti, una cava verticale, ecc.
- sul multirotore è possibile inserire più sensori: sensore fotografico, termografico, multispettrale e persino scanner laser 3D

## Piano di volo

## Flusso di lavoro

●selezionare l'area di rilevamento da una mappa come google
●impostare le caratteristiche della fotocamera montata sul drone
●impostare l'altitudine di volo.

https://pix4d.com/product/pix4dcapture/

## Rilevamento di volo

Il software mostrerà:
●Percorso del drone con traiettorie
●Tempo di volo
●Numero di fotografie e loro posizione
●Dimensione del pixel a terra.

## Fotogrammetria

Dopo l'acquisizione, le immagini verranno caricate nel PC ed elaborate con un software di fotogrammetria

Principi di funzionamento del software dell'ultima generazione e loro utilizzo, sia con foto da drone che con foto scattate manualmente a terra.

Con l'avvento delle fotocamere digitali, supportato da una notevole evoluzione del software fotogrammetrico, il rilievo fotogrammetrico sta tornando di moda.

Il "digitale" infatti consente di eseguire rapidamente un'elevata quantità di fotogrammi limitando le spese e i tempi di sviluppo.

Inoltre il tecnico ha la possibilità in "tempo reale" di valutare la qualità delle immagini evitando lunghe attese e il rischio di dover tornare sul sito in un momento successivo.

A livello software, le automatizzazioni oggi disponibili consentono un'autonomia quasi completa nell'ottenere modelli 3D con nuvole di punti molto simili a quelle ottenute da uno scanner laser.

Il primo vantaggio è la semplicità d'uso, mentre in passato erano necessarie competenze specifiche di volo.

Un altro "vantaggio" è che il sw durante l'elaborazione non ha bisogno della presenza del tecnico, che si limiterà a verificare i risultati, accertarli o modificare i parametri di lavoro.

L'altra cosa molto importante per la diffusione di questi sistemi è anche la possibilità di avere un risultato unico descritto in nuvola di punti. In passato, lavorare con immagini stereoscopiche richiedeva molta esperienza e il rischio di interpretare le quote in modo non univoco era molto alto.

Ciò implicava anche che la formazione di un tecnico restitutore potesse richiedere mesi o addirittura anni.

Non ultimo, è il costo totale della strumentazione Hardware (fotocamera) e Software. Rispetto ad oggi, il costo di un sistema completo è decine di volte inferiore al costo di uno solo dei 2 singoli elementi acquistati 10/15 anni fa.

## orientamento interno

In passato, la prima operazione che veniva eseguita era l'inserimento nel sw di un certificato di calibrazione della fotocamera. Questo certificato, che per costruzione è unico per ogni combinazione fotocamera-ottica, veniva fornito dal produttore.

Le camere avevano alcune precauzioni come l'ottica bloccata su una singola lunghezza focale o come le pellicole che venivano spinte con un apposito carrello al fotogramma per evitare qualsiasi deformazione dello stesso. Il certificato era quindi un foglio contenente tutti gli errori e le imperfezioni della fotocamera in modo che questi potessero essere corretti digitalmente dal computer.

In dettaglio venivano riportati:
. Dimensione della lastra emotiva
. Deviazione del centro di proiezione focale sulla lastra dal centro reale
. Distorsione dell'ottica

Il software moderno calcola questi valori automaticamente grazie alla capacità di riconoscere automaticamente lo stesso punto reale e misurato su più fotogrammi, utilizzando la correlazione dei pixel omologhi.

Questa fase si chiama appunto "orientamento interno"

## orientamento esterno

Il processo di orientamento esterno relativo ci permette di calcolare la posizione di un'immagine rispetto all'altra al momento dello scatto.

Questa operazione, che in passato veniva eseguita manualmente riconoscendo una decina di punti in comune tra una foto e l'altra, ora avviene automaticamente.

Utilizzando sempre una correlazione digitale dei pixel dell'immagine, il sw estrapola una quantità di punti considerevolmente superiore a quella che si potesse immaginare in passato.

## Nuvola di punti 3D. questi sono i punti utilizzati dal sw per calcolare le posizioni di scatto (in azzurro), che è sia la loro posizione nello spazio come coordinata xyz sia la loro rotazione sugli assi.

## Modellazione 3D

Una volta ottenute le posizioni di scatto, siamo in grado di recuperare un modello 3D

La posizione del punto a terra viene calcolata proiettando lo stesso pixel per la distanza focale fino a quando non si incrociano.

Naturalmente questo processo oggi è completamente automatico e viene eseguito su ogni pixel dell'immagine.

## Calcolo di un punto "P" a partire dalla sua posizione su 2 lastre fotografiche

Il risultato è un modello 3D molto definito.

## orientamento assoluto

Il modello 3D ottenuto è comunque ancora fuori scala.

Inserendo punti di controllo, con valori di coordinate X Y Z misurati con strumentazione grafica come GPS o Stazione Totale e riconoscendoli in immagini o nuvole di punti possiamo riportare il modello alle dimensioni reali.

Naturalmente la quantità dei punti è proporzionale all'area di lavoro, e la loro dislocazione dovrebbe essere progettata in modo da distribuire i punti nel modo più omogeneo possibile mantenendoli il più possibile distanti tra loro.

In questa fase il software può mostrare una tabella con:
. Coordinate x y z reali (misurate con strumentazione topografica)
. Coordinate x y z del modello (calcolate automaticamente dal sw sul modello fuori scala)
. Divergenze tra i 2 modelli nei punti noti

## Tutorial

Video di Maurizio Marra (in italiano)
https://www.youtube.com/watch?v=bY8iq0F-pWA

Manuale di Agisoft Photoscan (in italiano)
http://www.agisoft.com/pdf/manuals_other/pscan_pro_it_1-2.pdf


### 03 SISTEMI INFORMATIVI GEOGRAFICI

**SISTEMI INFORMATIVI GEOGRAFICI**


### GIS? Che cos’è?

**Sistema informativo**
+
**Posizione geografica**

Un mezzo per archiviare, recuperare, ordinare e confrontare dati spaziali per supportare un processo analitico.



### GIS? Che cos’è?

Non esiste più una risposta semplice

* **Informazione geografica/geospaziale**

  * informazione sui luoghi sulla superficie terrestre
  * conoscenza di “che cosa si trova dove e quando” (non dimenticare il tempo!)
  * geografico/geospaziale: sinonimi

* **GIS — cosa significa la S?**

  * Systems (Sistemi): la tecnologia
  * Science (Scienza): i concetti e la teoria
  * Studies (Studi): il contesto sociale



### Sistemi, Scienza e Studi GI

* **Sistemi**
  tecnologia per l’acquisizione e la gestione delle informazioni spaziali

* **Scienza**
  comprendere le questioni concettuali alla base della rappresentazione dei dati e dei processi nello spazio-tempo
  la teoria e i concetti dietro la tecnologia
  introdurre abbastanza teoria per applicare correttamente i sistemi e comprenderne capacità e limiti

* **Studi**
  comprendere gli aspetti sociali, legali ed etici legati all’applicazione dei GIS



### Definizione di GIS

* Un GIS è un sistema (hardware + motore di database) progettato per assemblare, memorizzare, aggiornare, analizzare, manipolare e visualizzare in modo efficiente informazioni georeferenziate (dati identificati dalla loro posizione).

* Un GIS include anche le persone che lo utilizzano e i dati inseriti nel sistema.



### Componenti di un GIS

* **Hardware**

  * Computer
  * Reti
  * Stampanti, plotter, scanner

* **Software**

  * Software GIS
  * Software di database
  * Sistema operativo
  * Software di rete

* **Persone**

  * Amministratori
  * Manager
  * Tecnici GIS
  * Utenti

* **Dati**

  * Dati vettoriali
  * Dati raster
  * Immagini
  * Attributi

* **Regole**

  * Linee guida
  * Standard
  * Procedure



### Componenti del GIS

Persone
Software
Dati
Hardware
Procedure



### Modello dei dati GIS: scopo

Permette che le caratteristiche geografiche del mondo reale siano rappresentate digitalmente e memorizzate in un database, in modo da poter essere presentate in forma cartografica (analogica) e manipolate per risolvere problemi.



### Astrazione del mondo reale



### Modello GIS

* Modellazione dei dati spaziali
* Visualizzazione dei dati spaziali
* Analisi spaziale
* Modellazione spaziale
* Dati attributo
* Sistema di gestione di database



### Modello dei dati GIS: esempio

Abbiamo tre livelli (layer) o temi:

* strade
* idrologia (acqua)
* topografia (elevazione del terreno)

Possono essere correlati perché per ciascun tema sono registrate coordinate geografiche precise.

I layer comprendono due tipi di dati:

* dati spaziali (dove)
* dati attributo (cosa, quanto, quando)

I layer possono essere rappresentati in due modi:

* formato vettoriale (punti e linee)
* formato raster (pixel/immagini)

Tutti i dati geografici hanno 4 proprietà:

* proiezione
* scala
* accuratezza
* risoluzione



### Collegamento tra entità spaziali e attributi

Dati spaziali (funzioni ARC)
Dati attributo (funzioni INFO o TABLE)



### Sistema Informativo Geografico

Il GIS collega elementi grafici (entità) a dati tabellari (attributi).



### Analisi GIS

* Classificazione dei dati
* Confronto dei dati
* Intersezione di elementi grafici
* Operazioni topologiche
* Statistica spaziale
* Modellazione spaziale
* Data mining



### Output GIS

* Mappe
* Diagrammi
* Report
* Modelli n-dimensionali



### Output GIS

**VISUALIZZAZIONE**



### Materiali e testi del corso

* Appunti del corso e slide
* Manuale QGIS ([http://qgis.org/documentazione/manuali.html?lang=it](http://qgis.org/documentazione/manuali.html?lang=it))
* GIS Open Source (Dario Flaccovio Editore)



**Geomatica**
informatica applicata
Urbino Worldwide Campus

### 03.01 CARTOGRAFIA DIGITALE E DATABASE

**CARTOGRAFIA DIGITALE E DATABASE**
Mauro De Donatis
Dipartimento DISPEA di Scienze Pure e Applicate



### ANALOGICO vs. DIGITALE

**Analogico**

* mappe cartacee
* fotografie aeree stampate
* tabelle statistiche
* scala fissa
* necessità di conversione in formato digitale

**Digitale**

* file di dati digitali
* immagini da telerilevamento
* file di output GPS
* scala “libera” / flessibile
* formato del file predefinito
* scaricabile o copiabile



### Astrazione del mondo reale



### Dati geografici

**DATI**
I dati permettono di costruire un modello del mondo reale

* Dati spaziali
* Dati attributo

Esempi:

* fermata bus
* limite di velocità (35)
* nome della strada
* intervallo civici a sinistra/destra
* lunghezza del percorso
* direzione di percorrenza



### Mappe dinamiche

* Spostamento sulla mappa (pan/zoom/salto)
* Modifica dei simboli: linee/colori/icone/font
* Visualizzazione simultanea di più dati e mappe
* Attivazione/disattivazione delle informazioni



### Selezioni GIS

* Selezione grafica
* Selezione tramite query



### GIS: collegamento tra entità e attributi

* Il GIS collega elementi grafici al database
* Coordinate spaziali
* Simboli
* Dati/Informazioni



### Sistema Informativo Geografico

Il GIS collega elementi grafici (entità) a dati tabellari (attributi).



### Modello dei dati GIS: scopo

Il GIS consente che le caratteristiche geografiche del mondo reale siano rappresentate digitalmente e memorizzate in un database, così da poter essere presentate in forma astratta su una mappa (analogica) e manipolate per risolvere problemi.



### Modello dei dati GIS: esempio

Abbiamo tre layer (livelli/temi):

* strade
* idrologia (acqua)
* topografia (altitudine del terreno)

Sono collegabili grazie alle coordinate geografiche precise registrate per ciascun tema.

I layer comprendono due tipi di dati:

* dati spaziali (dove)
* dati attributo (cosa, quanto, quando)

Rappresentazione dei layer:

* formato vettoriale (punti e linee)
* formato raster (pixel/immagini)

Proprietà dei dati geografici:

* proiezione
* scala
* accuratezza
* risoluzione



### Layer

**Layer vettoriali**

* rete stradale: linee
* particelle catastali: poligoni

**Layer raster (immagini)**

* ortofoto digitale:
  combina le proprietà visive di una fotografia con l’accuratezza posizionale di una mappa, in formato leggibile dal computer



### Classificazione dei dati: METADATI

Il termine metadati è spesso spiegato come “dati sui dati”.

Tradizionalmente presenti nei cataloghi delle biblioteche, oggi i metadati descrivono anche dati digitali secondo standard specifici. Descrivendo contenuto e contesto dei dati, migliorano notevolmente la qualità dei file.



### METADATI GEOSPAZIALI

I metadati geospaziali (o geografici) si applicano a oggetti con una posizione geografica esplicita o implicita sulla superficie terrestre.

Questi oggetti possono essere:

* dati GIS
* documenti
* dataset
* immagini
* servizi

Possono essere organizzati in cataloghi (directory o inventari di dati).



### METADATI GEOSPAZIALI

**ISO 19115 – “Informazione geografica – Metadati”**
Fornisce informazioni su:

* identificazione
* estensione
* qualità
* schema spazio-temporale
* riferimento spaziale
* distribuzione dei dati geografici digitali

Principi applicabili anche a:

* mappe
* carte
* documenti testuali
* dati non geografici

**Definizione FGDC (USA):**
Un record di metadati è un file (spesso XML) che descrive le caratteristiche principali di una risorsa informativa:

* chi
* cosa
* quando
* dove
* perché
* come

Include:

* titolo, abstract, dati di pubblicazione
* estensione geografica e proiezione
* definizioni degli attributi



### METADATI INSPIRE

INSPIRE è un’iniziativa dell’Unione Europea per creare un’infrastruttura di informazioni territoriali, rendendo i dati geografici più accessibili e interoperabili a supporto dello sviluppo sostenibile.

La direttiva INSPIRE:

* è entrata in vigore il 15 maggio 2007
* definisce un quadro per infrastrutture di dati spaziali (SDI)
* supporta politiche ambientali europee
* copre 34 temi di dati spaziali



### METADATI INSPIRE

Per garantire compatibilità e utilizzo tra Stati membri, la direttiva richiede regole comuni per:

* metadati
* interoperabilità dei dati e servizi
* servizi di rete
* condivisione dei dati
* monitoraggio e reporting


### 03.02 Formato file – Georeferenziazione – Feature

**FORMATI FILE RASTER e VECTOR**



### Raster vs. Vector

**Vantaggi del RASTER**

* formato di dati più comune
* facile eseguire operazioni matematiche e di overlay
* facile integrazione di dati satellitari
* migliore rappresentazione di dati “continui”

**Vantaggi del VECTOR**

* elevata precisione della posizione (ideale per elementi discreti: strade, coste, fondali, ecc.)
* minore occupazione di spazio su disco
* possibilità di associare un numero illimitato di attributi



### Elementi spaziali

* Raster
* Vector
* Mondo reale



### Che tipo di mappa digitale?

Raster?
Vector?



### RASTER

Memorizza immagini come righe e colonne di numeri con un **valore digitale (DN)** per ogni cella.

* unità rappresentate come celle quadrate uniformi
* dati classificati come:

  * **continui** (es. immagini)
  * **tematici** (ogni cella rappresenta una classe/feature)



### Formato raster

Nelle immagini la cella minima è il **pixel**, con:

* coordinate
* informazioni di colore



### Rasterizzazione delle entità

(processo di conversione in formato raster)



### Formati raster principali

* ADRG
* BIL
* CADRG
* CIB
* DRG
* ECRG
* ECW
* Esri Grid
* GeoTIFF
* IMG
* JPEG2000
* MrSID



### GeoTIFF

Standard pubblico che permette di incorporare informazioni di georeferenziazione in un file TIFF.

Include:

* proiezione
* sistema di coordinate
* ellissoide
* datum
* riferimento spaziale completo

Compatibile con TIFF 6.0 (leggibile anche senza supporto GIS).

**File associati:**

* .TIF / .TIFF → immagine
* .TFW → file di georeferenziazione
* opzionale: .PRJ → sistema di proiezione



### ATTRIBUTI

* **Raster:** il valore della cella (DN) è l’attributo

  * es. luminosità, copertura del suolo, temperatura

* **Vector:**

  * attributi collegati a punti, linee e poligoni
  * più attributi per ogni elemento
  * collegamento tramite ID univoco



### VECTOR

* rappresenta posizioni specifiche nello spazio continuo
* memorizza elementi come coppie di coordinate X,Y



### Formati vector principali

* **Shapefile** (ESRI)
* **Spatialite** (open source)



### SHAPEFILE

* memorizza geometria + attributi
* geometria = insieme di coordinate vettoriali
* vantaggi:

  * veloce da disegnare
  * facile da modificare
  * poco spazio su disco
* supporta:

  * punti
  * linee
  * poligoni

Attributi salvati in formato **dBase (.dbf)**
Relazione 1:1 tra geometria e attributi



### File obbligatori dello shapefile

* **.shp** → geometria
* **.shx** → indice
* **.dbf** → attributi



### File opzionali

* .prj → sistema di riferimento
* .sbn / .sbx → indice spaziale
* .ain / .aih → indice attributi
* .xml → metadati
* .cpg → codifica caratteri
  (altri file di supporto)



### Problemi dello SHAPEFILE

* formato datato
* composto da più file (se uno manca → dataset inutilizzabile)
* molto diffuso come standard di scambio



### SPATIALITE

* formato open source basato su database
* supporta geometrie standard OGC
* permette query SQL
* può leggere shapefile senza importarli



### Classi geometriche

* semplici
* multiple
* collezioni



### Georeferenziazione

Georeferenziare significa definire la posizione di un oggetto nello spazio reale tramite:

* sistemi di coordinate
* proiezioni cartografiche

Serve per collegare:

* immagini raster
* dati vettoriali
* altri dati geografici



### Applicazioni

* posizionare immagini satellitari
* confrontare dati nel tempo
* unire mappe con sistemi diversi
* integrare dati GPS
* collegare dati statistici a territori



### Ground Control Points (GCP)

* punti con coordinate note
* usati per georeferenziare immagini
* consigliati: 12–20 punti distribuiti
* ottenibili tramite GPS o cartografia



### Georeferenziazione con QGIS

Procedura:

1. Aprire plugin “Georeferencer”
2. Caricare immagine raster
3. Definire sistema di riferimento (CRS)
4. Inserire GCP (punti di controllo)
5. Avviare georeferenziazione
6. Verificare il risultato



### Feature (entità)

Elementi spaziali:

* **Punti** (più semplici)
* **Linee** (insieme di punti)
* **Poligoni** (linee chiuse)



### Attributi (vector)

* collegati a ogni feature
* memorizzano informazioni descrittive



### Operazioni topologiche principali

* Buffer
* Overlay
* Union
* Intersect
* Identity
* Operazioni booleane



### BUFFER (analisi di prossimità)

Definisce una zona attorno a un elemento:

* punto → cerchio
* linea → fascia
* poligono → area estesa

Può variare in base agli attributi (es. livello di inquinamento).



### OVERLAY

Combina più layer per analisi spaziale:

* confronto
* sovrapposizione
* intersezione

Tipi:

* **Vector overlay** → più complesso
* **Raster overlay** → confronto cella per cella



### Tipi di overlay vector

* punto in poligono
* linea in poligono
* poligono in poligono



### Operazioni booleane

* **UNION (OR)** → unisce aree
* **INTERSECT (AND)** → mantiene solo aree comuni
* **IDENTITY** → mantiene caratteristiche di un layer

