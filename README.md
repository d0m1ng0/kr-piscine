# kr-piscine

#shell00 - Minimo vitale dal K&R
    Cap. 1 (Introduzione, tutorial)
        Hello, world e scheletro di un programma C
        Variabili ed espressioni aritmetiche
        for e costanti simboliche (#define)
        I/O a caratteri e a linee (getchar, putchar, concetto di newline)
        Funzioni (definizione/chiamata)
        (facoltativo ma utile): argomenti da riga di comando (argc/argv)
    Cap. 7 (Input/Output formattato)
        basi di printf/scanf: come stampare stringhe/integri/float
        Appendice B (Libreria standard)
        tabellina dei format specifiers di printf/scanf (%d, %f, %s, etc.)
        Non serve dal libro (usa i manuali)
        Queste parti di KSH00 sono “shell/tooling”, non coperte dal K&R:
        Redirezioni e pipe → man bash (operatori >, >>, <, |)
        Compilazione → man 1 gcc (flag), man 3 printf (reference formati)
        Makefile → man make (target/variabili di base)
        Git → git help / man git
        Script → shebang #!/usr/bin/env bash, set -euo pipefail

Mappa rapida esercizio → lettura
    ex00 (cat/less) → serve solo un hello.c: leggi Hello, world (Cap.1).
    ex01 (gcc & run) → Cap.1 (+ un’occhiata a printf in Cap.7).
    ex02 (flag di compilazione) → man gcc.
    ex03 (man pages) → man gcc/make/grep/wc e man 3 printf/scanf.
    ex04 (redir/pipe) → man bash redirezioni e pipe.
    ex05 (Makefile min) → man make (targets e variabili).
    ex06 (git init) → git help / man git.
    ex07 (build.sh) → basi bash (shebang, set -euo pipefail, redirect).
    Facoltativo (anteprima per moduli dopo KSH00)
    Cap. 8: interfaccia UNIX a basso livello (open/read/write/close, lseek), utile più avanti per IO “raw”.
