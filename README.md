# Monocle2-fixed
A patched version of Monocle2 (v2.9.0) compatible with modern R environments (R ≥4.0, Matrix ≥1.5, dplyr ≥1.1) with fixes for sparse matrix handling, deprecated APIs, and igraph compatibility (tested with igraph 1.2.11).

## Installation

This patched version of **Monocle2 (v2.9.0)** is designed for modern R environments.

### Tested environment

```
R ≥ 4.0
Matrix ≥ 1.5
dplyr ≥ 1.1
igraph 1.2.11 (required)
```

---

## 1 Install igraph 1.2.11

Monocle2 is not fully compatible with newer igraph APIs.  
Install **igraph 1.2.11** before installing Monocle.

```r
install.packages("igraph_1.2.11.tar.gz", repos = NULL, type = "source")
```

---

## 2 Install Monocle2-fixed

Download the patched source and install:

```r
install.packages("monocle-release-master-fixed.zip",
                 repos = NULL,
                 type = "source")
```

or from terminal:

```bash
R CMD INSTALL monocle-release-master-fixed.zip
```

---

## 3 Load the package

```r
library(monocle)
```

---

## Verify installation

```r
packageVersion("monocle")
```

Expected output:

```
[1] "2.9.0"
```

---

## Supported functionality

The patched version supports the full Monocle2 workflow:

```
DDRTree
orderCells
plot_cell_trajectory
BEAM
plot_genes_branched_heatmap
differentialGeneTest
```
