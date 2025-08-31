# KSH00 — Shell Basics (Piscine K&R)

Obiettivo: muoversi come alla Piscine 42 con terminale, toolchain C e un flusso di lavoro minimale (compilare, eseguire, redirigere, documentare).

## Cosa impari
- Comandi base di ispezione (`cat`, `less`)
- Compilazione con `gcc` e flag severi (`-Wall -Wextra -Werror`)
- Manuali (`man 1/2/3`) e note operative
- Redirezioni e pipe (`>`, `>>`, `<`, `|`)
- Makefile minimo
- Git init e struttura pulita
- Script di build robusto

## Regole
- Standard: `-std=c99` (ok anche c11), `-Wall -Wextra -Werror`
- Niente librerie esterne
- Ogni esercizio ha i suoi **turn-in files** (vedi elenco sotto)
- Script bash con `#!/usr/bin/env bash` e `set -euo pipefail`
- Mantieni i comandi riproducibili (niente “magie” manuali durante la correzione)

## Struttura modulo
KSH00_shell-basics/
├── README.md
├── ex00_cat-less/ # ispezione file
├── ex01_gcc-run/ # compilare+eseguire
├── ex02_flags-Wall-Wextra-Werror/ # differenze dei warning
├── ex03_man-pages/ # reference minimo
├── ex04_redirections-pipes/ # I/O da shell
├── ex05_makefile-min/ # Makefile essenziale
├── ex06_git-init-structure/ # repo pulito
└── ex07_build-script/ # script di build


## Turn-in per esercizio (riassunto)
- **ex00** → `notes.md`
- **ex01** → `commands.sh`, `out.txt`
- **ex02** → `flags.md`, `commands.sh`
- **ex03** → `man-notes.md`
- **ex04** → `io.md`, `output.txt`
- **ex05** → `Makefile`
- **ex06** → `.gitignore`, `gitlog.txt`
- **ex07** → `build.sh`, `build/output.txt`

> Ogni cartella contiene `subject.md` con i dettagli.

## Workflow consigliato
1. Leggi `subject.md` dell’esercizio.
2. Implementa i file richiesti (script, Makefile, note).
3. Prova tutto da zero: `git clean -fdx && (make || ./build.sh)`.
4. Committa con messaggio chiaro (es. `ksh00: ex03 man notes`).

## Valutazione (indicativa)
- Esecuzione corretta e ripetibile: **60%**
- Pulizia struttura/naming/Makefile: **20%**
- Note e spiegazioni sintetiche ma utili: **20%**

## Quick refs
- **gcc**: `gcc -std=c99 -Wall -Wextra -Werror hello.c -o hello`
- **redir**: `./hello > out.txt`, `./hello >> out.txt`, `wc -c < out.txt`
- **pipe**: `./hello | wc -c`
- **make** (minimo): targets `all/clean/fclean/re`; variabili `CC CFLAGS NAME SRC OBJ`
- **man utili**: `man 1 gcc`, `man 1 make`, `man 1 grep`, `man 1 wc`, `man 3 printf`, `man 3 scanf`, `man 2 open/read/write`

## Checklist
- [ ] ex00
- [ ] ex01
- [ ] ex02
- [ ] ex03
- [ ] ex04
- [ ] ex05
- [ ] ex06
- [ ] ex07

## Prossimo step
Passa a **KSH01_toolchain-workflow** (layout progetto, header/guard, lib statica, mini test-runner).

