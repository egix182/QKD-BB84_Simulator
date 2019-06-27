# QKD-BB84_Simulator
Il tool descritto è una semplice simulazione dei passi del protocollo BB84.
In breve: due parti Alice e Bob, senza che condividano alcuna informazione precedente, vogliono poter generare una chiave segreta sicura, in modo tale da rilevare la presenza di un eventuale intercettatore, Eve, se si intromette nella comunicazione. 

Lo scenario preso in considerazioni consiste in 3 figure: 
### Alice – Mittente: 
ha il compito di generare casualmente la chiave iniziale, codificarla  e inviare i fotoni a Bob; successivamente effettuare delle operazioni sul canale classico per rilevare che non ci siano stati errori e, eventualmente, generare la chiave segreta; 

### Bob – Ricevente: 
ha il compito di misurare i fotoni ricevuti, ottenendo la propria chiave inziale; successivamente effettuare delle operazioni sul canale classico per rilevare che non ci siano stati errori e, eventualmente, generare la chiave segreta; 

### Eve – Eveasdropper: 
ha il compito di intercettare i fotoni inviati da Alice, con il fine di ottenere informazioni sulla chiave segreta, effettuandone la misurazione e re-inviarli a Bob (sta inscenando un attacco intercettazione-rinvio). 

Essendo una simulazione, il tool non tiene in considerazione alcuni fattori. Di seguito riportiamo le limitazioni:
- Qualsiasi rilevamento di errore viene attribuito alla presenza di un intercettatore; 
- Non sono simulate perdite di informazioni dovute al transito all’interno del canale quantistico; 
- Non è fissato alcuna lunghezza del canale quantistico. 
- Non sono state simulate tecniche di correzione degli errori e amplificazione della privacy. 
