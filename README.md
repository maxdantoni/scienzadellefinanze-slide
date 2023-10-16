# Slide per il testo "Scienza delle finanze"

In questa respository sono disponibili le slide, con relativi file sorgente, per il testo:

* G. Arachi e M. D'Antoni, [*Scienza delle finanze*](https://www.mulino.it/isbn/9788815290113), Il Mulino, Bologna, 2023. 

Le slide sono in formato PDF mentre i file sorgente sono in formato LaTeX/Beamer. Sono presenti anche le figure, nei formati PDF, JPEG e PNG.

Il materiale didattico, creato da Massimo D'Antoni, è rilasciato con licenza BSD (Clause 3), dunque è possibile per chiunque scaricarlo, modificarlo e utilizzarlo a proprio piacimento. L'unica condizione è quella di menzionare l'autore originale.

## Compilazione

I file sorgente per ricompilare le slide si trovano nella cartella `/tex`.

Per la compilazione è necessario disporre di un'installazione LaTeX che comprenda i pacchetti necessari, incluso [beamer](https://ctan.org/pkg/beamer). Come motore di compilazione è possibile usare sia il tradizionale `pdftex` che i più moderni `xetex` e `luatex`, che possono utilizzare i font OpenType e TrueType installati nel sistema. 

* I pdf inclusi inella cartella `/pdf` sono stati compilati con `xetex` e utilizzano i font [Roboto](https://fonts.google.com/specimen/Roboto) per il testo e [Fira Math](https://github.com/firamath/firamath) per formule matematiche. Chi non avesse tali font installati nel proprio sistema può impostare altri font TrueType (es. Calibri o Arial) modificando i commandi `\setmainfont`, `\setsansfont` e `\setmathfont` nel file `localheader.sty`.

* Compilando i file con `pdftex` vengono utilizzati i font Noto con il pacchetto [notomath](https://ctan.org/pkg/notomath). Anche in questo caso è possibile modificare l'impostazione nel file  `localheader.sty`.


## Modifiche e personalizzazioni

I file `.tex`, che contengono il testo delle slide, utilizzano [beamer](https://ctan.org/pkg/beamer), un formato che si è affermato come standard nella creazione di presentazioni in ambiente LaTeX.  La modifica del testo non richiede tuttavia la padronanza di tale formato, è sufficiente una conoscenza di base della sintassi LaTeX. Nella maggior parte dei casi sarà sufficiente intervenire modificando il testo esistente.

In ciascun file sono impostati alcuni dati relativi al docente, all'insegnamento, all'università e all'anno accademico, che possono essere personalizzati modificando gli argomenti dei seguenti comandi:

    \author{...}    % l'autore o il docente che svolge le lezioni
    \date{...}      % l'anno accademico
    \title{...}     % il titolo della lezione
    \subtitle{...}  % la denominazione dell'insegnamento
    \institute{...} % l'università o istituzione

È possibile cambiare del tutto il tema grafico delle slide modificando o sostituendo il file di stile `localheader.sty`. Nel caso di sostituzione con un nuovo file con un nome diverso, occorrerà modificare il comando `\usepackage{localheader}` presente nel preambolo dei file `.tex`.

**Nota bene:** le slide vengono compilate anche nel caso in cui il comando `\usepackage{localheader}` venga semplicamente rimosso dal file `.tex`, ma in questo caso sarà utilizzato un tema di base con una grafica essenziale.

