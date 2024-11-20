# Campionato di F1
Realizzare un sistema per gestire il campionato di formula 1 (CampionatoF1)

## R1: Squadre
Ogni squadra ha un nome, una nazionalità (Italia, Gran Bretagna, ecc.) e un insieme di piloti (2 + 1 eventuale riserva).
Il metodo addPilota(..) aggiunge un oggetto Pilota ad una squadra.
Il metodo piloti(..) ritorna una stringa contenente numero, nome, cognome e nazione di origine dei piloti della squadra con il seguente formato: "#25 Max Verstappen (Olanda)". 
Il metodo toString() restituisce una stringa contenente nome e nazione della scuderia, ad esempio: “Team Ferrari (Italia)”
Il metodo getPunti() restituisce i punti conquistati dalla scuderia ottenuti sommando i punti ottenuti dai piloti della squadra.

## R2: Piloti
Ogni pilota è identificato da nome, cognome, nazionalità e numero della vettura (che lo distingue univocamente dagli altri compagni di squadra), dai punti conquistati in ogni gran premio corso e dalla scuderia (team) di appartenenza. Definire i metodi getTeam() e setTeam(). Definire i metodi getPunti() e addPunti(int n) oltre ad un opportuno metodo toString().
 
## R3: Gran Premi (GP)
Ogni Gran Premio è caratterizzato da un nome, una nazione, dalla lunghezza del circuito, dal numero di giri da effettuare e da un ordine di arrivo (primi tre piloti).
Definire i seguenti metodi:
- setOrdine(…) che riceve tre oggetti di classe Pilota passati in ordine di arrivo, il metodo deve aggiornare anche i punti conquistati da ciascun pilota ( 6 punti al vincitore, 3 al secondo arrivato ed 1 al terzo).
- getOrdine() restituisce una stringa contenente tutte le posizioni del podio (una per  riga), con pilota e nome della scuderia di appartenenza. 
	Esempio:  “1° - #16 Charles Leclerc (Monaco) – Ferrari”
- toString() che restituisca una stringa con i dati del circuito (nome, nazione, numero di giri da effettuare, lunghezza complessiva della gara). 
	Esempio: “GP di Monza (Italia) 71 giri (Km. 230,61)”

## R4: Campionato
La classe CampionatoF1 espone i seguenti metodi da definire:
 - aggiungiGP(..) permette di aggiungere un gran premio alla classe CampionatoF1. 
- aggiungiSquadra() della classe CampionatoF1 aggiunge una squadra al sistema.
- getSquadre() deve ritornare una stringa contenente tutte le squadre inserite
- getGP() deve ritornare una stringa contenente tutti i Gran premi inseriti

## R5: Classifica piloti
Il metodo classificaPiloti() ritorna una stringa contenente una lista dei piloti insieme ai punti conquistati.

## R6: Classifica costruttori
Il metodo classificaCostruttori() ritorna una stringa contenente una lista di tutte le scuderie iscritte al campionato insieme ai punti conquistati.
