# Slide per il testo "Scienza delle finanze"

In questa respository sono disponibili le slide, con relativi file sorgente, per il testo:

* G. Arachi e M. D'Antoni, *Scienza delle finanze*, Il Mulino, Bologna, 2023. 

Le slide sono in formato PDF mentre i file sorgente sono in formato LaTeX/Beamer. Sono presenti anche le figure, nei formati PDF, JPEG e PNG.

Il materiale didattico, creato da Massimo D'Antoni, è rilasciato con licenza BSD (Clause 3), dunque è possibile per chiunque scaricarlo, modificarlo e utilizzarlo a proprio piacimento. L'unica condizione è quella di menzionare l'autore originale.

## Compilazione

Per compilare è necessario disporre di un'installazione LaTeX. I file sono predisposti per essere compilati utilizzando il motore XeLaTeX, che consente di utilizzare i font ttf (per la creazione dei PDF sono stati utilizzati i font Roboto). È possibile utilizzare altri font (es. Calibri o Arial) modificando l'impostazione del file localheader.sty.

Per utilizzare pdfLaTeX è necessario modificare i comandi nel file localheader.sty

## Modifiche e personalizzazioni

In ciascun file sono indicati, e possono essere personalizzati, i seguenti campi:

    \author{...}
    \date{...}  % qui indico l'anno accademico
    \title{...} 
    \subtitle{...}  % qui metto la denominazione dell'insegnamento
    \institute{...}



