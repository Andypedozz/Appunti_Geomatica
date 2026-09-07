
# Argomenti Trattati
* Introduzione
    * Cartografia
    * Telerilevamento
        * Fotografia aerea
        * Immagini satellitari
* Acquisizione dati telerilevati
    * LIDAR: laser scanner terresetre
    * LIDAR aereo
    * Droni per il rilievo di informazioni territoriali
* Sistemi Informativi Geografici
    * Cartografia digitale e banche dati territoriali
    * Formati dei file, georeferenziazione, features
    * GIS open source (Quantum GIS)
* Sistemi di posizionamento globale (GPS)
    * Storia dei diversi sistemi
    * Segmenti e la trilaterazione
    * Precisione, accuratezza, errori e correzioni
* Rilevamento digitale
    * Mobile GIS
    * Tablet PC
    * GPS per il mobile GIS
* Modellazione multidimensionale
    * Cartografia e sezioni geologiche (2D)
    * DEM e DTM (2.5D)
    * Modelli 3D e n-dimensionali

## Cartografia
La cartografia è lo studio delle mappe e la pratica di realizzare mappe.

Si possono realizzare diversi tipi di mappe:
* Mappe topografiche
* Mappe idrografiche
* Mappe orografiche
* Mappe urbane

Ogni mappa geografica è caratterizzata da una scala. La scala di una mappa indica il rapporto tra una distanza sulla mappa e sulla Terra. In base a essa distinguiamo mappe a piccola scala (1:10.000 - 1:50.000), mappe a scala intermedia (1:50.000 - 1:250.000) e mappe a piccola scala (1.250.000 - 1.7.500.000).

La scala è rappresentata sulle mappe anche visualmente, tramite delle linee indicative della distanza da prendere sulla mappa. Questa è utile in quanto consente di mantenere l'informazione anche se la mappa viene stampata in diverse dimensioni.

## Proiezioni Cartografiche:

Le proiezioni sono delle trasformazioni che vengono effettuate per rappresentare la terra, o un oggetto tridimensionale qualsiasi, su un piano. Le proiezioni vengono scelte in base allo scopo della mappa in quanto esse comportano una distorsione dell'oggetto in esame, riguardo a una o più proprietà. Perciò esistono diverse proiezioni:
* Conformi: conservano gli angoli e le forme locali (UTM)
* Equivalenti: conservano le aree (Lambert)
* Equidistanti: conservano le distanze rispetto a un punto o a una linea di riferimento.

## Coordinate Geografiche
Per identificare un qualsiasi punto sulla terra si usano due coordinate geografiche:
* Latitudine: è l'angolo compreso tra il piano equatoriale e una linea perpendicolare al piano equatoriale passante per il punto. (circonferenze)
* Longitudine: è l'angolo compreso tra una linea parallela passante per il punto e il meridiano di Greenwich. (semicirconferenze)

## Formati delle coordinate
Le coordinate possono essere espresse in Gradi, Primi e Secondi sessaggesimali o in gradi decimali, come avviene nella cartografia digitale e nel GPS.

## Forme della Terra
La terra viene approssimata sia con un Elissoide o un Geoide.

# Sistemi di Riferimento
Esistono diversi sistemi di riferimento per geolocalizzare punti sulla Terra.

* Gauss-Boaga (Roma 40): sistema di riferimento italiano proposto da Giovanni Boaga.
* WGS 84: sistema di riferimento globalo usato dai sistemi GPS
* UTM (Universal Transverse Mercator): divide la terra in 60 fusi, di cui l'italia occupa il fuso 32 e 33.

## Curve di Livello
Le curve di livello sono delle curve che rappresentano insiemi di punti su una mappa che condividono la stessa altitudine.

# Modelli Digitali
I modelli digitali sono rappresentazioni numeriche dell'altimetria.

* DEM (Digital Elevation Model): qualsiasi modello di quota, generato tramite fotogrammetria, Lidar aereo, interferometria SAR e digitalizzazione di curve di livello.
* DTM (Digital Terrain Model): modello che rappresenta solo la quota del terreno spoglio di vegetazione e urbanistica.
* DSM (Digital Surface Model): modello di quota che rappresenta il terreno e anche vegetazione e edifici.

## Modellazione 2.5D
Si tratta di un tipo di modellazione intermedio tra il 2D e il 3D in quanto non modella volumi o oggetti tridimensionali, ma solo superfici seppure definite su 3 dimensioni. Viene spesso abbinato alla fotogrammetria in modo da applicare un immagine (fotografia aerea, immagine satellitare o mappa geologica) sulla superficie di un DEM, ottenendo una visualizzazione tridimensionale del territorio.

## Come si generano i DEM?
* Fotogrammetria: a partire da coppie stereoscopiche o image matching automatico
* Lidar aereo: nuvola di punti 3D
* Interferometria SAR: tramite segnali RADAR
* Digitalizzazione di curve di livello: da carte topografiche tradizionali

## Telerilevamento: Lidar

## Telerilevamento: Immagini satellitari
### Sistemi ottici: Telerilevamento passivo

Il telerilevamento ottico utilizza sensori nel visibile, nel vicino infrarosso e nell'infrarosso a onde corte per formare immagini della superficie terrestre rilevando la radiazione solare riflessa dagli obiettivi sul terreno.

### Orbite satellitari
Il percorso seguito da un satellite è definito orbita. I satelliti geostazionari si trovano ad altitudini di circa 329.000 Km e ruotano a velocità che corrispondono alla rotazione terrestre. La maggior parte delle piattaforme satellitari di telerilevamento oggi si trova in orbite quasi polari, il che significa che il satellite viaggia verso nord su un lato della Terra e poi verso il polo sud a nella seconda metà della sua orbita. Queste sono chiamate rispettivamente passaggi ascendenti e discendenti.

## Le 4 risoluzioni
* Risoluzione Spaziale: area minima sul terreno visibile al sensore.
* Risoluzione Radiometrica: capacità di distinguere piccole differenze di energia

* Risoluzione spettrale: capacità di analizzare parti dello spettro utilizzando un sensore pancromatico, multispettrale o iperspettrale.

### Immagini satellitari
* Panoramiche: un sensore a canale singolo viene utilizzato per rilevare la radiazione. Se l'intervallo di lunghezza d'onda e l'intervallo visibile coincidono, l'immagine apparirà come una fotografia in bianco e nero scattata dallo spazio.
* Multispettrali: usano un rilevatore multicanale e registrano la radiazione con un intervallo ristretto. Sono disponibili informazioni sulla luminosità e sul colore.

Formati Raster: GeoTIFF, JPEG 2000, ECW, MrSID
Formati Vettoriali: Shapefile, GeoPackage, SpatiaLite

# Georeferenziazione
Significato: assegnare coordinate geografiche reali a un immagine raster o a un dato vettoriale, stabilendo la corrispondenza tra i pixel e le posizioni sul terreno.

## Modelli di Dati nei GIS
* Formato Raster: rappresenati lo spazio tramite una griglia di pixel. Ogni cella contiene un valore numerico, ideal per DEM e immagini satellitari.
* Formato Vettoriale: rappresenta lo spazio con 3 oggetti primitivi: punti, linee e poligoni. Ogni elemento è localizzato con precisione tramite array di coordinate (X, Y) più degli attributi associati.

Ground Control Points (GCP): sono dei punti la cui posizione sulla terra è nota, che servono a orientare la carta.

# Sistemi di posizionamento globale (GNSS)

GNSS (Global Navigation Satellite System): sono sistemi globali di navigazione basati su costellazioni di satelliti che trasmettono segnali. Ricevendo questi segnali, un dispositivo sulla terra può calcolare la sua posizione.

## Costellazioni
* GPS (USA)
* Glonass (Russia)
* Galielo (Europa)
* Compass (Cina)