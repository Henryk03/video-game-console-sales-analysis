# Analisi delle vendite di console e videogiochi

Progetto di analisi dei dati realizzato in R per il corso di **Fondamenti di Scienza dei Dati e Laboratorio** dell'Università degli Studi di Udine (anno accademico 2022/23).

Lo studio esplora le vendite di console e videogiochi nel mondo e confronta i risultati tra generi, aree geografiche e piattaforme. Il progetto comprende uno script R e una presentazione in formato R Markdown, della quale è disponibile anche l'esportazione HTML.

## Domande di ricerca

- Quali tipologie di console hanno registrato le vendite più alte?
- Quali generi di videogiochi vendono di più nelle diverse aree geografiche?
- Che relazione emerge tra le vendite delle console e quelle dei videogiochi? Si distinguono gruppi di console?
- Le vendite dei videogiochi variano in base alla piattaforma?

## Struttura del progetto

```text
.
├── data/                   Dataset utilizzati nell'analisi
├── external/               Foglio di stile e relativa licenza
├── RMarkdown/              Sorgente della presentazione Rmd e HTML
└── src/                    Script R dell'analisi
```

| Percorso | Contenuto |
| --- | --- |
| `src/Project.R` | Script R con preparazione dei dati, grafici, regressione e clustering |
| `RMarkdown/Project_Rmd.Rmd` | Sorgente della presentazione |
| `RMarkdown/Project_HTML.html` | Presentazione HTML già generata |
| `data/vgsales.csv` | Vendite di videogiochi per titolo e piattaforma |
| `data/best-selling game consoles.csv` | Dati sulle console più vendute |
| `external/custom.css` | Stili personalizzati |

## Dataset

I dataset sono reperiti su Kaggle:

- [Sales of Video Games](https://www.kaggle.com/datasets/arslanali4343/sales-of-video-games) — vendite per titolo, piattaforma, genere e area geografica.
- [Best-selling Game Consoles of All Time](https://www.kaggle.com/datasets/tayyarhussain/best-selling-game-consoles-of-all-time) — tipologia, produttore, anni di attività e unità vendute per console.

I file CSV utilizzati sono inclusi nella cartella `data/`.

## Esecuzione

Il progetto richiede R e i pacchetti `readr`, `tidyr`, `dplyr`, `ggplot2`, `forcats`, `factoextra` e `ggrepel`.

I file R caricano i CSV usando percorsi relativi alla cartella di lavoro, mentre i dataset si trovano in `data/`. Per ripetere l'analisi occorre quindi impostare la cartella di lavoro e i percorsi dei dati in modo coerente. La presentazione HTML inclusa permette di consultare i risultati senza rigenerare il report.
