# Influenza virus deep mutational scanning data sets visualized by `dms-view`

## Data sets

## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate study.
   Data are named by the study's first author and year, such as [./data/Findlay2018/](data/Findlay2018/).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
   As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
   In general, you should name these with the CSV data file named according to the study name (e.g., [./data/Findlay2018/Findlay_ringdomain.csv](data/Findlay2018/Findlay_ringdomain.csv)), the PDB file simply being the PDB (e.g., [./data/Findlay2018/1t29.pdb](./data/Findlay2018/1t29.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/Findlay2018/Findlay2018.md](data/Findlay2018/Findlay2018.md)).
   In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/Findlay2018/README.md](data/Findlay2018/README.md)).
   In some cases (such as if the same data is mapped to multiple protein structures) you may need to extend or modify this naming scheme.
   If you need to process other rawer forms of the data (e.g., from paper supplements) into the final data file for `dms-view`, then include those rawer data and the processing scripts if possible, explaining in the subdirectory repo.

4. Make a pull request for your branch or fork to add the data.

5. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

6. Make a pull request for your branch or fork to add the link.
