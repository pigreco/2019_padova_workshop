===================
Diagrammi e grafici
===================

* caricamento dati ``geochimica`` e basemap ``OSM``
* creazione diagrammi a torta con Mg, Ca e Na e dimensione di EC
* attivazione legenda in funzione della dimensione

* scaricare e attivazione plugin DataPlotly
* spiegazione funzionalità principali del plugin
* ``Scatterplot`` Ca - Mg e interazione con grafico (vari pulsanti)
* attivare etichette con ``id`` dei punti e cambiare hover label Dataplotly per mostrare interattività
* dimensione in funzione di ``ec / 100``
* colore in funzione di parametro ``na``
* aggiunta altro ``Scatterplot`` sovrapposto Ca - Fe (cambiare hover label complessa 'pozzo numero' || '\n' || 'id' )
* esportazione grafico in png e html
* pulire grafico e mostrare opzione e rifare con Ca - Mg e Ca - Na. Valori troppo distanti, 2 grafici separati 
* opzione Subplots con i 2 grafici
* Boxplot ``depth - mg``
* aggiunta statistiche
* Barplot (``id - ca``)
* opzione stacked con ``id - mg``
* Histogram con ``ec``
* opzione cumulativo e varie normalizzazioni 
* Pie con ``depth e mg``
* Ternario con ``na - mg - so4``
* Violin ``depth - ec`` 
* confronto con Boxplot per mostrare differenza varianza
* Creazione di una composizione di stampa con grafici e esportazione


=========
John Snow
=========

* caricare progetto ``john_snow``
* aree di influenza delle sorgenti idriche per capire diffusione colera
* :menuselection:`Processing --> Poligoni di Voronoi`
* :menuselection:`Processing --> Count points in polygon`
* :menuselection:`Processing --> SAGA -> Kernel` con parametri (Colera Deaths: radius: 100, extent: canvas, cs:1)
* :menuselection:`Processing --> Distance to nearest hub (line to hub)` (Colera, Pumps, Id, meters)

Layer temporanei e non voluti (Voronoi) e analisi ripetitive. Se avessimo stessa struttura dati per 30 quartieri di Londra?

Noi vogliamo dare solamente 4 parametri in input:

1. vettore di punti delle morti del colera
2. campo della tabella degli attributi dele vettore dei morti con conteggio vittime
3. vettore puntuale di sorgenti idriche
4. estensione spaziale per il kernel

opzionalmente anche 5. che è campo del vettore delle sorgenti che serve per ``Distance to nearest hub``


