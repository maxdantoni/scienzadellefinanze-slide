# Slide per il testo "Scienza delle finanze"

In questa respository sono disponibili le slide, con relativi file sorgente, per il testo:

* G. Arachi e M. D'Antoni, *Scienza delle finanze*, Il Mulino, Bologna, 2023. 

Le slide sono in formato PDF mentre i file sorgente sono in formato LaTeX/Beamer. Sono presenti anche le figure, nei formati PDF, JPEG e PNG.

Il materiale didattico, creato da Massimo D'Antoni, è rilasciato con licenza BSD (Clause 3), dunque è possibile per chiunque scaricarlo, modificarlo e utilizzarlo a proprio piacimento. L'unica condizione è quella di menzionare l'autore originale.

## Compilazione

Per compilare è necessario disporre di un'installazione LaTeX. I file sono predisposti per essere compilati con XeLaTeX oppure con LuaLaTeX, "motori" che leggono i caratteri Unicode e consentono di utilizzare i font OpenType e TrueType (per la creazione dei PDF sono stati utilizzati i font [Roboto](https://fonts.google.com/specimen/Roboto)). Chi non avesse tali font installati nel proprio sistema può impostare altri font TrueType (es. Calibri o Arial) modificando i commandi `\setmainfont`, `\setsansfont` e `\setmathfont` nel file `localheader.sty`.

Per utilizzare pdfLaTeX è necessario modificare il `localheader.sty`, rimuovendo il comando: 

    \usepackage[...]{unicode-math}

e i comandi `\setmainfont`, `\setsansfont` e `\setmathfont`, sostituendoli coi pacchetti specifici dei font desiderati.


## Modifiche e personalizzazioni

In ciascun file sono indicati, e possono essere personalizzati, i seguenti campi:

    \author{...}
    \date{...}  % qui indico l'anno accademico
    \title{...} 
    \subtitle{...}  % qui metto la denominazione dell'insegnamento
    \institute{...}



