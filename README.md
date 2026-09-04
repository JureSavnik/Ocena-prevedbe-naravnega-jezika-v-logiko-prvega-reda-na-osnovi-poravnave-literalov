# Ocena-prevedbe-naravnega-jezika-v-logiko-prvega-reda-na-osnovi-poravnave-literalov
Repozitorij vsebuje celotne rezultate in vizualizacije za članek "Ocena prevedbe naravnega jezika v logiko prvega reda na osnovi poravnave literalov" objavljen na ERK 2026.

## Rezultati

V razdelku so predstavljeni rezultati eksperimenta. Vizualno so predstavljene vrednosti LA (za LE in LS) in vrednosti LE ter LS, za vse baze ter pare metod in LLM. Temu sledijo tabele z vsemi rezultati za posamezne baze.

### Povprečne vrednosti LA
![Povprečne vrednosti LA pri meri LE in LS za vse baze ter pare metod in LLM-jev.](/slike/la.png)

### Povprečne vrednosti LE in LS
![Povprečne vrednosti LE in LS za prevode FOL vseh baze ter pare metod in LLM-jev.](/slike/le_ls.png)

### Tabela 1: FOLIO

Tabela prikazuje število napak ter vrednosti $LA$ za meri $LE$ in $LS$ ter vrednosti $LE$ in $LS$ na vseh NL-FOL parih v zbirki FOLIO.

| Met. | LLM | Napake LE | Napake LS | LA LE | LA LS | LE | LS |
|------|-----|----------|----------|-------|-------|-----|-----|
| A | gpt-oss | 74 | 30 | 0,667 | 0,716 | 0,871 | 0,858 |
| A | Llama-3.1 | 369 | 297 | 0,627 | 0,700 | 0,812 | 0,784 |
| B | gpt-oss | 94 | 40 | 0,666 | 0,720 | 0,854 | 0,841 |
| B | Llama-3.1 | 459 | 377 | 0,612 | 0,699 | 0,788 | 0,752 |
| Povprečje | | 249 | 186 | 0,643 | 0,708 | 0,831 | 0,808 |

---

### Tabela 2: MALLS (2020 naključnih)

Tabela prikazuje število napak ter vrednosti $LA$ za meri $LE$ in $LS$ ter vrednosti $LE$ in $LS$ na 2020 naključno izbranih NL–FOL parih iz zbirke MALLS.

| Met. | LLM | Napake LE | Napake LS | LA LE | LA LS | LE | LS |
|------|-----|----------|----------|-------|-------|-----|-----|
| A | gpt-oss | 218 | 7 | 0,730 | 0,824 | 0,741 | 0,735 |
| A | Llama-3.1 | 445 | 227 | 0,655 | 0,780 | 0,665 | 0,653 |
| B | gpt-oss | 337 | 19 | 0,728 | 0,806 | 0,777 | 0,771 |
| B | Llama-3.1 | 555 | 320 | 0,637 | 0,749 | 0,662 | 0,665 |
| Povprečje | | 389 | 143 | 0,687 | 0,789 | 0,711 | 0,706 |

---

### Tabela 3: FOLIO (25 ročno izbranih)

Tabela prikazuje število napak ter vrednosti $LA$ za meri $LE$ in $LS$ ter vrednosti $LE$ in $LS$ na 25 ročno izbranih NL-FOL parih iz zbirke FOLIO.

| Met. | LLM | Napake LE | Napake LS | LA LE | LA LS | LE | LS |
|------|-----|----------|----------|-------|-------|-----|-----|
| A | gpt-oss | 1 | 0 | 0,928 | 0,953 | 0,964 | 0,974 |
| A | Llama-3.1 | 0 | 0 | 0,909 | 0,941 | 0,943 | 0,927 |
| B | gpt-oss | 0 | 0 | 0,924 | 0,948 | 0,963 | 0,973 |
| B | Llama-3.1 | 0 | 0 | 0,913 | 0,939 | 0,927 | 0,917 |
| Povprečje | | 0,25 | 0 | 0,918 | 0,945 | 0,949 | 0,948 |

---

### Tabela 4: MALLS (25 ročno izbranih)

Tabela prikazuje število napak ter vrednosti $LA$ za meri $LE$ in $LS$ ter vrednosti $LE$ in $LS$ na 25 ročno izbranih NL-FOL parih iz zbirke MALLS.

| Met. | LLM | Napake LE | Napake LS | LA LE | LA LS | LE | LS |
|------|-----|----------|----------|-------|-------|-----|-----|
| A | gpt-oss | 0 | 0 | 0,982 | 0,983 | 0,907 | 0,907 |
| A | Llama-3.1 | 5 | 2 | 0,932 | 0,947 | 0,778 | 0,766 |
| B | gpt-oss | 1 | 0 | 0,970 | 0,971 | 0,917 | 0,906 |
| B | Llama-3.1 | 4 | 2 | 0,935 | 0,942 | 0,789 | 0,818 |
| Povprečje | | 2,5 | 1 | 0,955 | 0,961 | 0,848 | 0,849 |

---

### Tabela 5: Ročno izdelani NL-FOL pari

Tabela prikazuje število napak ter vrednosti $LA$ za meri $LE$ in $LS$ ter vrednosti $LE$ in $LS$ na 17 ročno izdelanih NL-FOL parih.

| Met. | LLM | Napake LE | Napake LS | LA LE | LA LS | LE | LS |
|------|-----|----------|----------|-------|-------|-----|-----|
| A | gpt-oss | 4 | 0 | 0,555 | 0,759 | 0,710 | 0,710 |
| A | Llama-3.1 | 4 | 1 | 0,430 | 0,745 | 0,581 | 0,569 |
| B | gpt-oss | 3 | 0 | 0,606 | 0,835 | 0,764 | 0,792 |
| B | Llama-3.1 | 4 | 2 | 0,585 | 0,850 | 0,600 | 0,585 |
| Povprečje | | 3,75 | 0,75 | 0,544 | 0,797 | 0,664 | 0,664 |

