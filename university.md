## Dipartimento
ID | smallint - auto-increment - PK
nome | VARCHAR(50)

## Corso di Laurea

ID | smallint - auto-increment - PK
id_dipartimento | BIGINT - FOREIGN KEY
nome VARCHAR(50)

## Corso

ID | smallint - auto-increment - PK
id_corso_laurea | smallint - auto-increment - PK
nome | VARCHAR(50)

## Insegnanti

ID | smallint - auto-increment - PK
nome | VARCHAR(50)
cognome | VARCHAR(50)
email | VARCHAR(50)

## Studente

ID | bigint - auto-increment -PK
nome | VARCHAR(50)
cognome | VARCHAR(50)
email | VARCHAR(50)
id_corso_laurea | smallint - auto-increment - PK

## Esame

ID | bigint - auto-increment -PK
id_studente | BIGINT - FOREIGN KEY
id_corso| smallint - auto-increment
nome | VARCHAR(50)
voto | TINYINT