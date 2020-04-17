# Influenza virus deep mutational scanning data sets visualized by `dms-view`

## Data sets

- BRCA1 functional scores measured by Findlay _et al._ (2018). See [here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2FFindlay2018_ringdomain.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2FFindlay2018_ringdomain.csv&condition=SGE&site_metric=site_mean+score&mutation_metric=mut_score&selected_sites=1%2C3%2C12%2C19%2C22%2C29%2C30%2C33%2C37%2C39%2C41%2C44%2C47%2C54%2C59%2C60%2C61%2C63%2C64%2C71%2C74%2C81%2C84%2C87%2C94&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2F1jm7.pdb) for an interactive dms-view visualization of the RING domain focused on sites variants classified as "Pathogenic" by clinVar. See [here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2FFindlay2018_brctdomain.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2FFindlay2018_brctdomain.csv&condition=SGE&site_metric=site_mean+score&mutation_metric=mut_score&selected_sites=1661%2C1666%2C1667%2C1676%2C1683%2C1685%2C1690%2C1692%2C1694%2C1703%2C1706%2C1708%2C1710%2C1711%2C1712%2C1715%2C1716%2C1718%2C1721%2C1725%2C1727%2C1731%2C1737%2C1738%2C1747%2C1751%2C1754%2C1756%2C1764%2C1766%2C1767%2C1769%2C1775%2C1779%2C1781%2C1782%2C1785%2C1787%2C1788%2C1794%2C1796%2C1797%2C1811%2C1815%2C1817%2C1823%2C1835%2C1836%2C1837%2C1838%2C1845%2C1846%2C1847%2C1848%2C1853&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FBRCA1%2Fmaster%2Fdata%2FFindlay2018%2F1t29.pdb) for an interactive dms-view visualization of the BRCT domain focused on sites variants classified as "Pathogenic" by clinVar. The raw data are [here](data/Findlay2018/).

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
