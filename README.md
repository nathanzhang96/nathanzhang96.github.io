# nathanzhang96.github.io
This is the repository for DSCI521 Milestone 3. It contains a homepage & about page which provide introduction of myself, and the blog page contains two computational blogs from R and Python, and finally a blog of my orientation day. 

## Prerequisites

Software version used in this project:

- Quarto 1.10.18
- uv 0.12.5
- R 4.6.1
- Python 3.14

## Exact Commands in order

Clone this repository and enter the project directory:

```bash
git clone git@github.com:nathanzhang96/nathanzhang96.github.io.git
cd nathanzhang96.github.io
```

Restore the Python environment from the project lockfile:

```bash
uv sync
```

Restore the R environment from the lockfile. From the project directory, start R:

```bash
R
```

Then, in the R console, run:

```r
renv::restore()
Y
```

After the restore is complete, exit R:

```r
q()
```

```markdown
If prompted to save the workspace image when exiting R, choose `n`.

## Where the built site lands

Build the website from the project directory:

```bash
uv run quarto render
```

The rendered website is generated in the `docs/` directory, and just to preview the website, we run:

```bash
uv run quarto preview
```

## Where the data comes from

Data Source

The data comes from the [Palmer Penguins dataset](https://allisonhorst.github.io/palmerpenguins/), collected and made available by Dr. Kristen Gorman and the Palmer Station Long Term Ecological Research (LTER) Program. The data is available under a [CC0 license](https://creativecommons.org/publicdomain/zero/1.0/).

The data is not required to be downloaded for rendering because the data is with the installation pacakge. However, the package installation needs internet access. 
