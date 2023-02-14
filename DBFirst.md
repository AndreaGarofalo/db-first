<!-- Vi chiediamo di immaginare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario!
Elencate le colonne, poi pensate ai tipi di dati corretti per ciascuna colonna. Infine, identificate la primary key ed assegnate gli attributi appropriati -->

| Colonne                                                          | Types         | Indici      | Attributi                       |
| ---------------------------------------------------------------- | ------------- | ----------- | ------------------------------- |
| ID                                                               | BIGINT        | PRIMARY KEY | NOT NULL, UNIQUE, AUTOINCREMENT |
| TARGA                                                            | VARCHART(20)  | ---         | NULL                            |
| MODELLO                                                          | VARCHART(20)  | ---         | NOT NULL                        |
| KILOMETRAGGIO                                                    | MEDIUMINT     | ---         | NOT NULL                        |
| ANNO                                                             | YEAR          | ---         | NOT NULL                        |
| TIPO DI ALIMENTAZIONE (BENZINA, ELETTRICA, GPL, METANO O DIESEL) | CHART(1)      | ---         | NOT NULL, DEFAULT(B)            |
| CAMBIO MANUALE O AUTOMATICO                                      | CHART(1)      | ---         | NOT NULL, DEFAULT(M)            |
| CONDIZIONE                                                       | VARCHART(25)  | ---         | NOT NULL                        |
| COLORE                                                           | VARCHART(16)  | ---         | NOT NULL                        |
| SISTEMI DI SICUREZZA                                             | VARCHART(100) | ---         | NOT NULL, DEFAULT(DI SERIE)     |
| PREZZO DI ACQUISTO                                               | FLOAT(8,2)    | ---         | NOT NULL                        |
| PREZZO DI VENDITA                                                | FLOAT(8,2)    | ---         | NOT NULL                        |
| CONSUMI                                                          | VARCHART(40)  | ---         | NOT NULL                        |
| CONFORT ELETTRONICI                                              | VARCHART(100) | ---         | NULL                            |
| TIPO DI CERCHIONI                                                | VARCHART(20)  | ---         | NULL                            |
| INTERNI                                                          | CHART(20)     | ---         | NULL                            |
| DATA DI ACQUISTO                                                 | YEAR          | ---         | NOT NULL                        |
| VENDUTA                                                          | TINYINT(1)    | ---         | DEFAULT(0)                      |
| NO. POSTI                                                        | TINYINT       | ---         | DEFAULT(4)                      |
