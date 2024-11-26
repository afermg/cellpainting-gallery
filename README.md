# Cell Painting Gallery

This page provides a guide to the datasets that are available in the Cell Painting Gallery, hosted by the AWS Registry of Open Data (RODA): <https://registry.opendata.aws/cellpainting-gallery>

## Citation/license

All the data is released with CC0 1.0 Universal (CC0 1.0).
Still, professional ethics require that you cite the appropriate resources/publications, [listed below](#available-datasets), when using individual datasets, along with our Nature Methods publication announcing the Cell Painting Gallery ([Weisbart et al., 2024](https://doi.org/10.1038/s41592-024-02399-z)).
For example,

> We used the dataset `cpg0000` ([Chandrasekaran et al., 2022](https://doi.org/10.1101/2022.01.05.475090)), available from the Cell Painting Gallery ([Weisbart et al., 2024](https://doi.org/10.1038/s41592-024-02399-z)) on the Registry of Open Data on AWS (<https://registry.opendata.aws/cellpainting-gallery/>).

## Documentation

Please see [our documentation](https://broadinstitute.github.io/cellpainting-gallery/) for extensive supporting information.

It includes:

- [how to browse gallery data](https://broadinstitute.github.io/cellpainting-gallery/browsing_data)
- [how to download gallery data](https://broadinstitute.github.io/cellpainting-gallery/download_instructions.html) (with AWS CLI, Quilt, or dataset-specific tools)
- [how to contribute to the gallery](https://broadinstitute.github.io/cellpainting-gallery/contributing_to_cpg)

## Available datasets

All datasets are generated using the Cell Painting assay unless indicated otherwise. Several updates to that protocol exist ([Cell Painting wiki](https://github.com/carpenterlab/2022_Cimini_NatureProtocols/wiki)).

The datasets are stored with the prefix indicated by the dataset name.
e.g. the first dataset is located at `s3://cellpainting-gallery/cpg0000-jump-pilot` and can be listed using AWS CLI `aws s3 ls --no-sign-request s3://cellpainting-gallery/cpg0000-jump-pilot/` (note the `/` at the end).
See [browsing data](https://broadinstitute.github.io/cellpainting-gallery/browsing_data) in our documentation for more information on viewing the gallery in a browser and examples of how to list files using AWS CLI or boto3.

The datasets' accession numbers are the first seven characters of the dataset name.
e.g. the accession number of the first dataset is `cpg0000`.

| Dataset name                             | Description                                                                                                                                                                                                      | Publication to cite                                                                                                                                                                                                | Associated repositories                                                                                                                                                        | Total size | Images size | Numerical data size | Cell Painting protocol |                                                                                          Other aliases                                                                                           |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------:|:-----------:|:-------------------:|:----------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| cpg0000-jump-pilot                       | 300+ compounds and 160+ genes (CRISPR knockout and overexpression) profiled in A549 and U2OS cells, at two timepoints                                                                                            | (Chandrasekaran et al., 2024) [Publication](https://doi.org/10.1038/s41592-024-02241-6), [Preprint](https://doi.org/10.1101/2022.01.05.475090), Description of Cell Painting v2.5.                                 | [data](https://github.com/jump-cellpainting/2023_Chandrasekaran_submitted)                                                                                                     |  12.3 TB   |   6.1 TB    |       6.1 TB        |          v2.5          |                                                                                                                                                                                                  |
| cpg0001-cellpainting-protocol            | 300+ compounds profiled in U2OS cells using several different modifications of the Cell Painting protocol                                                                                                        | (Cimini et al., 2022) [Publication](https://doi.org/10.1038/nprot.2016.105), [Preprint](https://doi.org/10.1101/2022.07.13.499171) Description of Cell Painting v3.                                                | [data](https://github.com/carpenter-singh-lab/2023_Cimini_NatureProtocols)                                                                                                     |  40.3 TB   |   18.7 TB   |       21.6 TB       |   v3 and experiments   |                                                                                                                                                                                                  |
| cpg0002-jump-scope                       | 90 compounds (JUMP-MOA plate) profiled in U2OS using different microscopes and settings                                                                                                                          | (Tromans-Coia and Jamali et al., 2023) [Publication](https://doi.org/10.1002/cyto.a.24786), [Preprint](https://doi.org/10.1101/2023.02.15.528711)                                                                  | [data](https://github.com/jump-cellpainting/jump-scope), [analysis](https://github.com/jump-cellpainting/jump-scope-analysis)                                                  |  16.7 TB   |   12.5 TB   |       4.2 TB        |          v2.5          |                                                                                                                                                                                                  |
| cpg0003-rosetta                          | 28,000+ genes and compounds profiled in Cell Painting and [L1000](https://doi.org/10.1016%2Fj.cell.2017.10.049) gene expression                                                                                  | (Haghighi et al., 2022) [Publication](https://doi.org/10.1038/s41592-022-01667-0), [Preprint](https://doi.org/10.1101/2021.09.08.459417)                                                                           | [data](https://github.com/carpenter-singh-lab/2022_Haghighi_NatureMethods)                                                                                                     |   8.5 GB   |      0      |       8.5 GB        |                        |                                                                                                                                                                                                  |
| cpg0004-lincs                            | 1,571 compounds across 6 doses in A549 cells                                                                                                                                                                     | (Way et al., 2022) [Publication](https://doi.org/10.1016/j.cels.2022.10.001), [Preprint](https://doi.org/10.1101/2021.10.21.465335)                                                                                | [data](https://github.com/broadinstitute/lincs-cell-painting)                                                                                                                  |  65.7 TB   |   61.9 TB   |       3.8 TB        |           v2           |                                                                                             idr0125                                                                                              |
| cpg0010-caie-drugresponse                | MCF-7 breast cancer cells treated  with 113 small molecules at eight concentrations.                                                                                                                             | (Caie et al., 2010) [Publication](https://doi.org/10.1158/1535-7163.MCT-09-1148)                                                                                                                                   |                                                                                                                                                                                |  239.2 GB  |   98.4 GB   |      140.8 GB       |    other variation     |                                                                        [BBBC021](https://bbbc.broadinstitute.org/BBBC021)                                                                        |
| cpg0011-lipocyteprofiler                 | Variety of lipocytes in different metabolic states and with genetic and drug perturbations                                                                                                                       | (Laber and Strobel et al., 2023) [Publication](https://doi.org/10.1016/j.xgen.2023.100346), [Preprint](https://www.biorxiv.org/content/10.1101/2021.07.17.452050v1) Description of Cell Painting lipocyte variant. | [Batch1 and Batch3 data](https://github.com/broadinstitute/2018_04_12_T2D_V2F_Saadat_Broad), [analysis](https://github.com/ClaussnitzerLab/Lipocyte-Profiler) |   1.2 TB   |   1.2 TB    |        16 MB        |        lipocyte        |                                                                                                                                                                                                  |
| cpg0012-wawer-bioactivecompoundprofiling | 30,000 compound dataset in U2OS cells. Original images re-profiled in 2023 (original profiles available in workspace/gigascience_profiles)                                                                       | (Wawer et al., 2014) [Publication](https://doi.org/10.1073/pnas.1410933111) Description of Cell Painting v1, (Bray et al., 2017) [Publication](https://doi.org/10.1093/gigascience/giw014) Description of Cell Painting v2 | [data](https://github.com/broadinstitute/2015_Bray_GigaScience-data)                                                                                                   |  10.7 TB   |   3.1 TB    |       7.6 TB        |           v1           |       [idr0016](https://idr.openmicroscopy.org/webclient/?show=screen-1251), CDRP, [BBBC036](https://bbbc.broadinstitute.org/BBBC036), [BBBC047](https://bbbc.broadinstitute.org/BBBC047)        |
| cpg0015-heterogeneity                    | 2,200+ compounds and 200+ genes profiles in U2OS cells                                                                                                                                                           | (Rohban et al., 2019) [Publication](https://doi.org/10.1038/s41467-019-10154-8)                                                                                                                                    | [data](https://github.com/carpenterlab/2018_Rohban_NatComm)                                                                                                                    |   204 GB   |      0      |       204 GB        |                        | [idr0016](https://bbbc.broadinstitute.org/BBBC036), [idr0036](https://idr.openmicroscopy.org/webclient/?show=screen-1952), [idr0033](https://idr.openmicroscopy.org/webclient/?show=screen-1751) |
| cpg0016-jump                             | 116,000+ compounds and 16+ genes (CRISPR knockout and overexpression) profiled in U2OS cells. Over 8 million images (>126 TB), over 1.5 billion cells of numerical data (>126TB), for over 250 TB data in total. | (Chandrasekaran et al., 2023) [Preprint](https://doi.org/10.1101/2023.03.23.534023)                                                                                                                                | [datasets resource](https://github.com/jump-cellpainting/datasets),[JUMP-Cell Painting Hub](https://broad.io/jump) |  358.4 TB  |             |                     |           v3           |                                                                                                                                                                                                  |
| cpg0017-rohban-pathways                  | 323 genes overexpressed in U2OS cells. Original images re-profiled in 2023 (original profiles not in gallery)                                                                                                    | (Rohban et al, 2017) [Publication](https://doi.org/10.7554/eLife.24060), [Preprint](https://doi.org/10.1101/092403)                                                                                                | [re-profiled data](https://github.com/broadinstitute/cpg0017-rohban-pathways), [original data](https://github.com/carpenterlab/2017_Rohban_eLife)                              |   321 GB   |   189 GB    |       132 GB        |           v1           |                                                                    [BBBC037](https://bbbc.broadinstitute.org/BBBC037), TA-ORF                                                                    |
| cpg0018-singh-seedseq                    | U2OS cells treated with each of 315 unique shRNA sequences                                                                                                                                                       | (Singh et al. 2013) [Publication](https://doi.org/10.1371/journal.pone.0131370)                                                                                                                                    |                                                                                                                                                                                |  247.1 GB  |  247.1 GB   |          0          |                        |                                                                                                                                                                                                  |
| cpg0019-moshkov-deepprofiler             | 8.3 million single cells from 232 plates, across 488 treatments from 5 public datasets, used for learning representations                                                                                        | (Moshkov et al., 2022) [Preprint](https://doi.org/10.1101/2022.08.12.503783)                                                                                                                                       | [data](https://github.com/broadinstitute/DeepProfilerExperiments), [software](https://github.com/cytomining/DeepProfiler)                                                      |   522 GB   |   482 GB    |        40 GB        |   dataset dependent    |                                                                                                                                                                                                  |
| cpg0021-periscope                        | 30 million cells with 20,000 single-gene knockouts in pooled format. A549 cells and HeLa cells in two growth media                                                                                               | (Ramezani, Weisbart, Bauman, and Singh et al., 2023) [Preprint](https://doi.org/10.1101/2023.08.06.552164) Description of Cell Painting pooled variant.                                                            | [analysis](https://github.com/broadinstitute/2022_PERISCOPE), [data](https://github.com/broadinstitute/CP186-A549-WG), [data](https://github.com/broadinstitute/CP257-HeLa-WG) |  56.0 TB   |   45.0 TB   |       11.0 TB       |         pooled         |                                                                                                                                                                                                  |
| cpg0022-cmqtl                            | 297 iPSC lines                                                                                                                                                                                                   | (Tegtmeyer et al., 2024) [Publication](https://doi.org/10.1038/s41467-023-44045-w), [Preprint](https://doi.org/10.1101/2023.01.09.522731)                                                                          | [data](https://github.com/broadinstitute/cmQTL)                                                                                                                                |   3.7 TB   |  2.8 TB     |        945 GB       |          v2.5          |                                                                                                                                                                                                  |
| cpg0028-kelley-resistance                | Bortezomib resistant HCT116 clones                                                                                                                                                                               | (Kelley et al., 2023) [Publication](https://doi.org/10.7554/eLife.91362)                                                                                                                                           | [data](https://github.com/broadinstitute/profiling-resistance-mechanisms)                                                                                                      |   4.1 TB   |   1.9 TB    |       2.2 TB        |                        |                                                                                                                                                                                                  |
| cpg0030-gustafsdottir-cellpainting       | U2OS cells treated with each of 1600 known bioactive compounds. Description of Cell Painting v1.                                                                                                                 | (Gustafsdottir et al., 2013) [Publication](https://doi.org/10.1371/journal.pone.0080999)                                                                                                                           |                                                                                                                                                                                |   234 GB   |   234 GB    |        .3 GB        |           v1           |                                    [BBBC022](https://bbbc.broadinstitute.org/BBBC022), [idr0036](https://idr.openmicroscopy.org/webclient/?show=screen-1952)                                     |
| cpg0031-caicedo-cmvip                    | ORF over-expression of 596 alleles of 53 genes in A549 cells. Original images re-profiled in 2023 (original profiles available in workspace/profiles_orig)                                                       | (Caicedo et al., 2023) [Publication](https://www.molbiolcell.org/doi/10.1091/mbc.E21-11-0538), [Preprint](https://doi.org/10.1101/2021.11.18.469171)                                                               | [original data](https://github.com/broadinstitute/luad-cell-painting), [re-profiled data](https://github.com/broadinstitute/cpg0031-caicedo-cmvip)                             |   2.2 TB   |   605 GB    |       1.6 TB        |           v1           |                                                                                          BBBC043, LUAD                                                                                           |
| cpg0036-EU-OS-bioactives                 | 2464 compounds from EU-OPENSCREEN Bioactive compound set, four imaging sites, two cell lines (HepG2 & U2OS)                                                                                                      | (Wolff et al., 2024) [Preprint](https://doi.org/10.1101/2024.08.27.609964)                                                                                                                                         | [aggregated profiles](https://doi.org/10.5281/zenodo.13309566), [analysis scripts](https://github.com/schmiedc/EU-OS_bioactives), [compound information](https://www.probes-drugs.org/compounds/standardized#compoundset=353@AND) |   3.5 TB   |   3.5 TB    |               |           v1           |                                                                                          Bioactives, EU-OS-Bioactives                                                                                          |
