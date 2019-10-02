# Gitlog Analysis

This projects analyzes the Git logs of the Linux kernel project to develop
a classifier which can predict which commits will lead to problems that
will need fixing by subsequent patches.

This analysis is based on patches indentified as incorrect by a subsequent
patch with a 'Fixes:' line.

The data preparation work has been done in a separate project available at
https://github.com/xypron/gitlog\_analyzer.

The output of the data preparation are the files authors.csv.gz and
commits.csv.gz. These can be unzipped with Gzip.

gitlog\_analysis.ipynb is a Juypter notebook. Just start Juypter with

    jupyter notebook

and select the file in your browser. The notebook contains the further
project description.

## Software Dependencies

On Debian Buster the following packages will have to be installed:

    apt-get install jupyter python3-pandas python3-sklearn python3-numpy \
    python3-matplotlib
