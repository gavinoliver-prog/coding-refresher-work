# coding-refresher-work

I created this repo to provide a structured short series  notebooks to help retain or retrain basic coding muscle memory in both R and Python.

The repository contains a collection of progressive notebooks designed to refresh and rebuild practical programming skills for computational biology and bioinformatics workflows. The materials are organized as hands-on exercises that move from language fundamentals to data analysis and basic machine learning concepts using small biological examples.

The goal is to provide a structured path from **basic scripting through reproducible analysis and introductory machine learning workflows**, with examples grounded in typical/classical bioinformatics tasks.

---

## Python Environment Setup

The Python notebooks use a virtual environment managed with **uv** and dependencies listed in `python/requirements.txt`.

```bash
cd python
uv venv
source .venv/bin/activate
uv pip install -r requirements.txt
jupyter notebook
```

To set up the R environment, open R from the `r/` directory and run:

```r
install.packages("renv")
renv::restore()
```

R notebooks are written in **Quarto (`.qmd`) format**, so Quarto must also be installed:

https://quarto.org/docs/get-started/

---


## Python Training Notebooks

The current notebooks focus on rebuilding Python fluency and applying it to common classical bioinformatics problems.

### Notebook 1 — Python Reboot for Bioinformatics

A rapid refresher on core Python concepts including:

- variables and strings  
- lists and dictionaries  
- loops and conditionals  
- functions and Python idioms  

All exercises use simple DNA sequence examples to rebuild programming muscle memory.

---

### Notebook 2 — Sequence Algorithms and File Parsing

Introduces practical bioinformatics scripting patterns:

- reading and writing files  
- FASTA parsing  
- reverse complements  
- sliding windows and k-mers  
- motif search  
- basic sequence statistics  

---

### Notebook 3 — Bioinformatics Objects and Pipelines

Introduces structured programming concepts:

- classes and objects  
- modeling biological entities (e.g., sequences and variants)  
- reusable functions  
- simple analysis pipelines  

---

### Notebook 4 — Bioinformatics Data Science with Pandas

Moves into the scientific Python ecosystem:

- working with `pandas` DataFrames  
- filtering and summarizing biological datasets  
- grouping and counting mutations  
- basic visualization with `matplotlib`  

---

### Notebook 5 — Machine Learning and Embeddings for Bioinformatics

Introduces the core machine learning workflow using `scikit-learn`:

- feature matrices and labels  
- train/test splits  
- logistic regression classification  
- clustering with KMeans  
- dimensionality reduction using PCA  
- simple embedding-style visualizations  

---

## R Training Notebooks

A parallel set of Quarto notebooks provides a structured refresher in R for data analysis and statistical workflows commonly used in computational biology.

### Notebook 1 — R Reboot for Bioinformatics

Introduces core R concepts including:

- variables and assignment
- strings and indexing
- vectors and vectorized operations
- functions
- lists
- simple data frames

---

### Notebook 2 — Data Frames and Structured Data

Focuses on working with tabular biological datasets using base R:

- creating data frames
- column and row indexing
- filtering rows with logical conditions
- counting categorical variables
- adding new columns
- basic aggregation

---

### Notebook 3 — Tidyverse Workflows

Introduces the modern R data analysis ecosystem using `dplyr`:

- pipes (`|>`)
- `select()`, `filter()`, and `mutate()`
- grouped summaries with `group_by()` and `summarise()`
- reshaping data with `pivot_longer()`

---

### Notebook 4 — Visualization with ggplot2

Covers the grammar-of-graphics approach to visualization:

- bar plots for categorical data
- scatter plots for biological features
- boxplots for distributions
- faceting
- themes and labeling
- integrating `dplyr` pipelines with plotting

---

### Notebook 5 — Statistics and Modeling

Introduces common statistical workflows in R:

- linear models (`lm`)
- logistic regression (`glm`)
- principal component analysis (PCA)
- clustering with k-means
- interpreting model outputs
