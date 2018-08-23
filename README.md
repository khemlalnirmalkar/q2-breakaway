# `breakaway` QIIME 2 plugin

[![Build Status](https://travis-ci.org/qiime2/q2-breakaway.svg?branch=master)](https://travis-ci.org/qiime2/q2-breakaway)
[![Coverage Status](https://coveralls.io/repos/github/qiime2/q2-breakaway/badge.svg?branch=master)](https://coveralls.io/github/qiime2/q2-breakaway?branch=master)

This repository contains the `breakaway` QIIME 2 plugin. `Breakaway` is in active development and is available in `R` (https://github.com/adw96/breakaway) or as a QIIME2 plugin (q2-breakaway).

To learn how to use `breakaway` in QIIME2, see https://qiime2.org.

`Breakaway` is based in `R` and requires installation of dependencies `phyloseq`, `devtools`, `ggplot2`,`magrittr`, `tibble`, `dplyr`,`withr`,`testthat`, and `praise` into your `conda` environment before installing `breakaway`. Please refer to the following instructions on how to install `breakaway` and its dependencies.


### Activate your QIIME Environment

- Here we activate our example version of QIIME, `qiime2-2018.8`. If you're not sure what your current version of QIIME is you can run `conda env list` in the command line to see a list of installed QIIME environments.

```source activate qiime2-2018.8```

### Install `breakaway` dependencies

(Expected installation time ~3-5 minutes)

```conda install -c bioconda -c conda-forge bioconductor-phyloseq r-devtools r-tibble r-magrittr r-dplyr r-withr r-testthat r-praise unzip```

- Note: When installing select `y` to proceed with installation when prompted.

### Install `breakaway` <br>

```TAR=/bin/tar R -e 'library("devtools"); options(unzip = "internal"); devtools::install_url("https://github.com/adw96/breakaway/archive/master.zip")'```

### Install `q2-breakaway`

```pip install git+https://github.com/statdivlab/q2-breakaway.git```


### Check that `breakaway` is installed <br>

```qiime breakaway --help```
