Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un `concessionario`.


-id | INDEX | NOTNULL | INT | UNIQUE | AI
-marca  | INDEX | VARCHART(`200`) | NOTNULL
-modello | VARCHART(`255`) | NOTNULL
-prezzo | MEDIUMINT | NOTNULL

-immagine | VARCHART(`255`) | NULL
-anno | YEAR | DEFAULT(`N/A`)
-colore | VARCHART(`50`)
-carburante | VARCHART(`100`) | DEFAULT(`N/A`)
-km | MEDIUMINT | DEFAULT(`0`)
-potenza | SMALLINT | NULL

-porte | TINYINT | NULL
-posti | TINYINT | NULL
-catagoria | VARCHART(`255`) | NULL
-stato | VARCHART(`50`) | DEFAULT(`USATA`)
-cambio | VARCHART(`100`) | NULL
-descrizione | TEXT | NULL
-note | TEXT | NULL