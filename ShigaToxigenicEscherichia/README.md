# Dataset of mass spectra for R

## Description and source
Intensity matrix from "Rapid MALDI-TOF mass spectrometry strain typing during a large outbreak of Shiga-Toxigenic Escherichia coli, Dryad, Dataset, https://doi.org/10.5061/dryad.bq64j"

The dataset was was downloaded from this [link](https://datadryad.org/stash/dataset/doi:10.5061%2Fdryad.bq64j)

## Details
The file named **RawIntensityMatrixChristner**  is a data.frame in `.tsv` format. The raw mass spectrum  from to  891 strains were previously imported into the `R` environment. After signal processing with the MSclassifR package (using s/n = 2, tolerance = 0.002) and peaks detection (label = id_number), an intensity matrix was performed. This intensity matrix contained 891 rows (corresponding to the strains) and 1226 columns (corresponding to mass-over-charge (*m/z*)). 

The file named **MetadataShigatoxChristnermetadata** is a `.csv` file associated to the intensity-matrix included 891 rows corresponding to the strains and 4 columns :

- **Toxigenic_status:** corresponding to the toxigenic status of the strain; according to the study:
  - **norec:** triplicate spectra from 190 non-outbreak related Escherichia coli isolates (189 clinical isolates collected during the time of the outbreak, reference strain DH5alpha)
  - **orec:** triplicate spectra from 104 outbreak related Escheriachia coli (O104:H4) isolates.
  - **ref**: triplicate spectra from three biological replicates of outbreak strain reference isolate TY-2482.
- **id_number:** corresponding to the number of the strain
- **Strain_number:** corresponding to the name of the strain in the study
- **spot:** corresponding to the plate spot for MALDI-TOF MS analysis
- **type_of_extraction: ** type of extraction for MALDI-TOF MS analysis (only formic acid extraction was used (fae))

## References
- **Dataset:**

Christner, Martin et al. (2015), Data from: Rapid MALDI-TOF mass  spectrometry strain typing during a large outbreak of Shiga-Toxigenic  Escherichia coli, Dryad, Dataset, https://doi.org/10.5061/dryad.bq64j

- **Article:**

Christner M, Trusch M, Rohde H, Kwiatkowski M, Schlüter H,   et al.   (2014)     Rapid MALDI-TOF Mass Spectrometry Strain Typing during a Large Outbreak of Shiga-Toxigenic *Escherichia coli*. PLOS ONE  9(7): e101924. https://doi.org/10.1371/journal.pone.0101924
