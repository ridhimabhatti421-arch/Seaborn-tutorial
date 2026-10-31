# Seaborn Tutorial

My notes and practice notebooks for learning Seaborn , the Python statistical data visualisation library built on Matplotlib. Each notebook walks through a family of plots with small examples, showing the different parameters and the difference between axis-level and figure-level functions.


### L1: Relational, Distribution & Matrix Plots (`L1-seaborn.ipynb`)
| Topic         | Functions |
|---------------|-------------------------------|
| Why Seaborn?  | Overview of the plot categories |
| Relational plots | `scatterplot`, `lineplot`, `relplot` |
| Faceting       | `col`, `row`, `col_wrap` on `relplot` |
| Distribution plots | `histplot`, `displot`, `kdeplot`, `rugplot` |
| Bivariate distributions | 2D histogram and 2D KDE |
| Matrix plots   | `heatmap` (with `annot`, `cmap`), `clustermap` |

### L2: Categorical, Regression & Grid Plots (`L2-seaborn.ipynb`)
| Topic                        | Functions |
|------------------------------|----------------|
| Categorical scatter plots    | `stripplot`, `swarmplot` |
| Categorical distribution plots| `boxplot`, `violinplot` |
| Categorical estimate plots   | `barplot`, `pointplot`, `countplot` |
| Figure-level function        | `catplot` (with faceting) |
| Regression plots             | `regplot`, `lmplot`, `residplot` |
| Multi-plot grids             | `FacetGrid`, `pairplot`, `PairGrid`, `jointplot`, `JointGrid` |

## Key concepts
- Axis-level vs. figure-level functions: axis-level functions (e.g. `scatterplot`) draw on a single Matplotlib axis. Figure-level functions (e.g. `relplot`, `displot`, `catplot`) manage the whole figure and support faceting via `col` and `row`.
- Semantic mappings: `hue`, `style` and `size` map data columns to colour, marker and size.
- Faceting: splitting one plot into a grid of subplots by a categorical variable.
- Grids for exploration: `pairplot` and `PairGrid` show every pairwise relationship at once.

## Datasets
All data loads directly from the libraries, so no files need downloading:
- `tips`, `iris`, `titanic`, `flights`: bundled with Seaborn (`sns.load_dataset`)
- `gapminder` and `iris`: from Plotly Express (`px.data`), used in L1

## Tech stack
Python, Seaborn, Matplotlib, Plotly Express (datasets only), NumPy

## Run it yourself
```bash
pip install seaborn matplotlib plotly numpy jupyter
jupyter notebook
```
Open `L1-seaborn.ipynb` or `L2-seaborn.ipynb` and run all cells. `sns.load_dataset` needs an internet connection the first time.