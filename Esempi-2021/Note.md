# Esempi 2021

## Conversione da .csv a .json
In questa cartella si trovare esempi dei file JSON generati a partire dai file forniti dalla SAVNO. La generazione è il risultato di un processo semi automatico di conversione dei file da Excel in CSV e poi in JSON.

Ogni anno i file forniti hanno delle differenze che mi forzano a pulirli e organizzarli prima di convertirli in CSV e darli in pasto al programma che genera i file in formato JSON compatibili con l'app.

I nomi dei files, delle zone, dei tipi di rifiuto sono fissi in quanto l'app li usa per collegare i vari dati e presentarli correttamente.

## Conversione file Google Calendar
In alternativa le date possono essere estratte dai file .ics forniti sul sito [SAVNO Servizi - Downloads](https://www.savnoservizi.it/it/avvisi-e-download/download/calendari).

## Generare i file .json

Usando i file .csv (o i file .ics) devi generare i file in formato .json simili a:

`````
  [
    {
      "day": "4",
      "month": "1",
      "year": "2021",
      "type": "Umido",
      "city": "Cappella Maggiore zona A"
    },
    {
      "day": "4",
      "month": "8",
      "year": "2021",
      "type": "Vetro",
      "city": "Cappella Maggiore zona A"
    }
    ...
 ]
``````

Il campo ``type`` accetta i seguenti valori:
- Vetro
- Umido
- Secco
- Plastica e Lattine
- Carta

L'app attualmento non supporta il verde e le ramaglie

Per verificare che è un file .json corretto, puoi usare un sito di validazione come [jsonformatter.org](https://jsonformatter.org/)

## Supporto iOs
Non esiste un'app iOs al momento. Esiste comunque un mio tentativo piuttosto grezzo di fornire i prelievi come file .ics per caricare le date in iCalendar o altri calendari che supportano tale formato.
