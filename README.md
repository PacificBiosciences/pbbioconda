<p align="center">
  <img src="img/pbbioconda.png" alt="pbbioconda logo"/>
</p>
<p align="center">PacBio Tools on Bioconda</p>

***

## Information
Binaries distributed via [bioconda](https://bioconda.github.io/) are
pre-release, not ISO compliant, for research only, not for use in diagnostics
procedures, and only for command-line users.

Official support is only provided for official and stable
[SMRT Analysis builds](http://www.pacb.com/products-and-services/analytical-software/)
provided by PacBio.

No support via mail to developers.

## Installation
Information how to install `conda` and add the `bioconda` channel is
available on https://bioconda.github.io/.

Packages can be installed using following command:
```sh
> conda install package_name
```

## Available Packages

| Package | Linux | Mac | Description |
| - | - | - | - |
| [bam2fastx](https://github.com/pacificbiosciences/bam2fastx/) | Y | Y | Convert and split BAM files into fasta.gz and fastq.gz |
| [bax2bam](https://github.com/pacificbiosciences/bax2bam/) | Y | Y | Convert legacy PacBio Bax.H5, Bas.H5, and Ccs.H5 files to BAM |
| [blasr](https://github.com/pacificbiosciences/blasr/) | Y | Y | The long read aligner |
| [genomicconsensus](https://github.com/pacificbiosciences/genomicconsensus/) | Y | - | Polish genome assemblies |
| [isoseq3](https://github.com/pacificbiosciences/isoseq3/) | Y | - | Scalable de novo isoform discovery |
| [lima](https://github.com/pacificbiosciences/barcoding/) | Y | - | Demultiplex barcoded samples |
| [pbbam](https://github.com/pacificbiosciences/pbbam/) | Y | Y | BAM C++ library |
| [pbccs](https://github.com/pacificbiosciences/unanimity/) | Y | - | Generate consensus sequences from single SMRTbells |
| [pbcommand](https://github.com/pacificbiosciences/pbcommand/) | Y | Y | Common models, CLI tool contract and SMRT Link service interface |
| [pbcopper](https://github.com/pacificbiosciences/pbcopper/) | Y | Y | Core C++ library for data structures, algorithms, and utilities |
| [pbcore](https://github.com/pacificbiosciences/pbcore/) | Y | Y | Python library for reading and writing data files |
| [pbcoretools](https://github.com/pacificbiosciences/pbcoretools/) | Y | Y | CLI tools and add-ons for PacBio's core APIs (incl `dataset`) |
| [pblaa](https://github.com/pacificbiosciences/pblaa/) | Y | - | Long amplicon analysis |
| [pbsv](https://github.com/pacificbiosciences/pbsv/) | Y | - | Structural variant analysis |

**Note:** BAM refers to the PacBio BAM format that includes additional information

## Disclaimer
THIS WEBSITE AND CONTENT AND ALL SITE-RELATED SERVICES, INCLUDING ANY DATA, ARE PROVIDED "AS IS," WITH ALL FAULTS, WITH NO REPRESENTATIONS OR WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTIES OF MERCHANTABILITY, SATISFACTORY QUALITY, NON-INFRINGEMENT OR FITNESS FOR A PARTICULAR PURPOSE. YOU ASSUME TOTAL RESPONSIBILITY AND RISK FOR YOUR USE OF THIS SITE, ALL SITE-RELATED SERVICES, AND ANY THIRD PARTY WEBSITES OR APPLICATIONS. NO ORAL OR WRITTEN INFORMATION OR ADVICE SHALL CREATE A WARRANTY OF ANY KIND. ANY REFERENCES TO SPECIFIC PRODUCTS OR SERVICES ON THE WEBSITES DO NOT CONSTITUTE OR IMPLY A RECOMMENDATION OR ENDORSEMENT BY PACIFIC BIOSCIENCES.