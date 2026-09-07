## Come funziona il GPS – Spiegazione completa

Il GPS (Global Positioning System) è un sistema di navigazione satellitare che permette a un ricevitore di determinare la propria posizione **in qualsiasi punto della Terra**, in **qualsiasi condizione meteorologica**, **24 ore su 24**.

Si basa su tre elementi chiave: **satelliti**, **segnali radio** e **calcoli matematici**.

---

### 1. I protagonisti: i satelliti

Il sistema GPS è composto da una costellazione di **almeno 24 satelliti** (attualmente circa 31) che orbitano intorno alla Terra a circa **20.200 km** di altitudine, distribuiti su **6 piani orbitali** in modo da garantire che da qualsiasi punto della Terra siano sempre visibili almeno **4 satelliti**.

Ogni satellite è dotato di:
- Un **orologio atomico** estremamente preciso (errore di pochi nanosecondi).
- Un trasmettitore che invia continuamente **segnali radio** verso la Terra.

---

### 2. Il segnale trasmesso

Ogni satellite trasmette un'onda radio che contiene tre informazioni fondamentali:

1. **Un codice identificativo univoco** (codice PRN) – permette al ricevitore di capire da quale satellite proviene il segnale.

2. **L'ora esatta di trasmissione** – generata dall'orologio atomico del satellite.

3. **Le effemeridi** – cioè i dati orbitali che descrivono la posizione esatta del satellite nello spazio in quel momento (forniscono anche informazioni sullo stato di salute del satellite).

---

### 3. Il ricevitore: come calcola la distanza

Il ricevitore GPS (nel tuo telefono, nel navigatore o nello strumento topografico) riceve i segnali da più satelliti contemporaneamente. Per ciascun satellite:

- **Misura il tempo di volo** del segnale: confronta l'ora di ricezione (registrata dal suo orologio interno, meno preciso) con l'ora di trasmissione (ricevuta dal satellite).
- Moltiplica il tempo di volo per la **velocità della luce** (circa 300.000 km/s).
- Ottiene così la **distanza** dal satellite.

Distanza = Velocità della luce × Tempo di volo

---

### 4. Il problema dell'orologio

L'orologio del ricevitore non è atomico e quindi non è perfettamente sincronizzato con quelli dei satelliti. Un errore di **1 microsecondo** (un milionesimo di secondo) produce un errore di **circa 300 metri** nella distanza calcolata.

Per questo il ricevitore deve risolvere **4 incognite**:
- Le tre coordinate spaziali: **X, Y, Z** (posizione).
- L'errore del suo orologio: **Δt**.

---

### 5. La trilaterazione: come si trova la posizione

Con un solo satellite, il ricevitore sa di trovarsi su una **sfera** centrata sul satellite, di raggio pari alla distanza misurata.

Con due satelliti, l'intersezione delle due sfere è una **circonferenza**.

Con tre satelliti, l'intersezione si riduce a **due punti** (uno dei quali è generalmente impossibile, ad esempio nello spazio profondo).

Con **quattro satelliti**, il sistema risolve le 4 incognite e determina in modo univoco la **posizione tridimensionale** (latitudine, longitudine e altitudine) **e corregge l'errore dell'orologio** del ricevitore.

---

### 6. Perché i satelliti sono così precisi?

Gli orologi atomici dei satelliti sono così precisi che un errore di 1 secondo si verificherebbe dopo **1 milione di anni**. Tuttavia, la relatività di Einstein introduce due effetti:

- I satelliti si muovono a **14.000 km/h**: il movimento rallenta gli orologi (effetto relativistico speciale).
- I satelliti si trovano a 20.000 km di quota, in un campo gravitazionale più debole: il tempo scorre più velocemente (effetto relativistico generale).

**Effetto netto**: l'orologio del satellite va avanti di circa **38 microsecondi al giorno**. Senza correzione, il posizionamento sbaglierebbe di oltre **10 km al giorno**. I sistemi a terra correggono continuamente questo errore.

---

### 7. Fonti di errore e correzioni

Anche con tutto questo, la precisione del GPS standard è di circa **15 metri**. Gli errori principali sono:

| Fonte di errore | Effetto |
|---|---|
| **Ionosfera** | Il segnale rallenta attraversando gli strati ionizzati. |
| **Troposfera** | Vapore acqueo e variazioni di pressione rallentano il segnale. |
| **Multipath** | Il segnale rimbalza su edifici o superfici prima di arrivare. |
| **Errori dell'orologio** | Derivano dal ricevitore o da piccole imprecisioni dei satelliti. |
| **Errori orbitali** | La posizione del satellite non è nota con precisione assoluta. |

Per migliorare la precisione si usano tecniche differenziali:

- **DGPS** (Differential GPS): una stazione a terra di coordinate note calcola l'errore e lo trasmette al ricevitore mobile, portando l'errore a **1–5 metri**.
- **RTK** (Real-Time Kinematic): usa una stazione base e un ricevitore mobile che comunicano in tempo reale, raggiungendo precisioni di **1–2 cm**.
- **WAAS/EGNOS**: reti di stazioni a terra che inviano correzioni via satellite geostazionario, portando l'errore sotto i **5 metri**.

---

### 8. Il risultato finale

Il ricevitore combina tutte queste informazioni e, in pochi secondi, restituisce:

- **Posizione** (latitudine, longitudine, altitudine).
- **Velocità** (derivata dalla variazione di posizione nel tempo).
- **Tempo** (sincronizzato con l'ora atomica).

---

### Schema riassuntivo

```
Satellite → trasmette segnale (ora + posizione)
Ricevitore → riceve segnale → calcola tempo di volo → distanza
Con 4 satelliti → risolve X, Y, Z e errore orologio → posizione 3D
Correzioni (DGPS, RTK) → migliorano la precisione
```

