![PyCon 2022 Banner](./banner_pycon22.png)

🇮🇹 Benvenuti al Workshop per Beginners di [PyCon 2022](https://pycon.it)! Il workshop pensato per introdurre neofiti e appassionati al linguaggio di programmazione Python.

🇬🇧 Welcome to [PyCon 2022](https://pycon.it) Beginners' Day Workshop! The workshop for beginners and code practictioners to the main features of the [Python](https://python.org) programming language.

### Get Started

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonitalia/pycon-beginners-day/pycon-2022) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pythonitalia/pycon-beginners-day/blob/pycon-2022/index.ipynb)


- About the workshop [ita](#descr-ita) | [eng](#descr-eng)
- [Credits](#credits)
- [License](#license)

### <a name="descr-ita">Descrizione 🇮🇹 </a>

Durante il workshop lavoreremo su un progetto che vuole realizzare un innovativo [Motore di Ricerca](https://it.wikipedia.org/wiki/Motore_di_ricerca) per i **Pokémon**.

Tale motore di ricerca includerà una speciale e super segreta tecnologia in grado di identificare i `k` Pokémon più simili ad una data [_query di ricerca_](https://it.wikipedia.org/wiki/Information_retrieval).

Progetteremo e svilupperemo passo passo questa speciale tecnologia che avrà l'obiettivo di calcolare un punteggio di similirità tra Pokémon, sia esitenti che immaginari, identificati da un insieme di specifiche caratteristiche. 

🧑‍💻 **Happy coding!** 👩‍💻

#### Curioso di saperne di più? (⚠️  ATTENZIONE, SPOILER )

Lavoreremo insieme all'implementazione dell'algoritmo [KNN](https://it.wikipedia.org/wiki/K-nearest_neighbors), un popolare e semplice metodo di [Machine Learning](https://it.wikipedia.org/wiki/Apprendimento_automatico) pensato per misurare le distanze fra punti in spazi ad N dimensioni. 

Ogni `Pokémon` nel nosto insieme di dati sarà rappresentato dalle seguenti caratteristiche:

```
- HP
- Attacco
- Difesa
- Attacco Speciale
- Difesa Speciale
- Velocità
```

Obiettivo dell'algoritmo è quello di confrontare il valore di ciascuna di queste caratteristiche, e restituire i `k` pokémon _maggiormente simili_ (i.e. alternativamente, a minore distanza), dati i paramentri della _query di ricerca_.

🧑‍💻 **Happy coding!** 👩‍💻

#### Strumenti

Il codice sviluppato durante il workshop non farà uso di alcuno strumento o software di terze parti che non sia direttamente incluso nell'installazione del linguaggio Python, con la sola eccezione di [`ipyplot`](https://github.com/karolzak/ipyplot) esclusivamente utilizzato per mostrare le immagini dei Pokémon.

### <a name="descr-eng">About 🇬🇧</a>

During the workshop, we will design an innovative **Pokémon** [Search Engine](https://en.wikipedia.org/wiki/Search_engine).

This engine will feature a special and super secret technology that is capable of retrieving the `k` most similar Pokémons with respect to the [_search query_](https://en.wikipedia.org/wiki/Information_retrieval).

We will design and implement _step-by-step_ this core technology in order to calculate the similarities between any pair of Pokémons, either existing or _imaginary_ ones, as identified by a specified set of characteristics.

🧑‍💻 **Happy coding!** 👩‍💻

#### Curious to know more? (⚠️  SPOILER ALERT)

We will be working on our implementation of the [KNN](https://en.wikipedia.org/wiki/K-nearest_neighbors), a very popular and simple [Machine learning](https://en.wikipedia.org/wiki/Machine_learning) algorithm designed to measure the distances between points in N-dimensional spaces.

Each `Pokémon` in our dataset will be denoted by the following set of _features_:

```
* HP
* Attack
* Defense
* Special attack
* Special defense
* Speed
```

The goal of the algorithm is to compare the values of each of those characteristics, and return the `k` _most similar_ pokémons (i.e. the ones at closest distance) given
an input search query.

#### Tools

We won't be using any external libraries or software. Everything will be implemented in pure Python, using all the _batteries already included_ in the language stack.
This is true with the **only exception of the [`ipyplot`](https://github.com/karolzak/ipyplot) package, that will be used in the _bonus material_ to display Pokémon images.

The development environment used throughout the workshop will be [Jupyter](https://jupyter.org).

### CREDITS

- Giuseppe Mastrandrea, Machine Learning Teacher `@` [Datamasters.it](https://datamasters.it/): code, and lecture materials
- [Alberto Barradas](https://www.kaggle.com/datasets/abcsds/pokemon) - Original Pokémon Dataset
- [Ken Sugimori](https://veekun.com/dex/downloads) - Pokémon Arts (adapted, and compressed in JPEG for storage requirements)

### LICENSE

All the **Code** material is distributed under the terms of the Apache License. See [LICENSE](./LICENSE) file for additional details.

All the instructional materials in this repository are free to use, and made available under the [Creative Commons Attribution
license][https://creativecommons.org/licenses/by/4.0/].
