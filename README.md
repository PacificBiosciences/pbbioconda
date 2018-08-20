<p align="center">
  <img src="img/pbbioconda.png" alt="pbbioconda logo"/>
</p>
<p align="center">PacBio Secondary Analysis Tools on Bioconda</p>

***

## Information
Binaries distributed via [bioconda](https://bioconda.github.io/) are
pre-release, **not ISO compliant**, for research only, not for use in diagnostics
procedures, only for command-line users, and possibly newer than the currently
available [SMRT Link release](http://www.pacb.com/products-and-services/analytical-software/).

## Support

Official tech support is only provided for official and stable
[SMRT Link releases](http://www.pacb.com/products-and-services/analytical-software/)
provided by PacBio.

No support via mail to developers.

For issues with the installation of **conda** or adding the **bioconda** channel,
please refer to the [official bioconda website](https://bioconda.github.io/).

For issues with installed **PacBio binaries through bioconda**, please [create
a new issue](https://github.com/PacificBiosciences/pbbioconda/issues/new?template=bug_report.md)!
Our developers will triage your problems internally and reply as soon as possible.

## Installation
Information how to install `conda` and add the `bioconda` channel is
available on https://bioconda.github.io/.

Packages can be installed using following command:
```sh
> conda install -c bioconda package_name
```

Packages can be updated with:
```sh
> conda update package_name
```

## Availability

**Notes:**
* Python packages require version 2.7; python 3 compatibility is tracked [here](https://github.com/PacificBiosciences/pbbioconda/issues/3)
* BAM refers to the PacBio BAM format that includes additional
per-record or per-ZMW information
* Packages might conflict with other bioconda packages not maintained by PacBio

### Packages

| Package | Linux | Mac | Description |
| - | - | - | - |
| [bam2fastx](https://github.com/pacificbiosciences/bam2fastx/) | Y | Y | Convert and split BAM files into fasta.gz and fastq.gz |
| [bax2bam](https://github.com/pacificbiosciences/bax2bam/) | Y | Y | Convert legacy PacBio Bax.H5, Bas.H5, and Ccs.H5 files to BAM |
| [blasr](https://github.com/pacificbiosciences/blasr/) | Y | Y | The long read aligner |
| [genomicconsensus](https://github.com/pacificbiosciences/genomicconsensus/) | Y | - | Polish genome assemblies |
| [isoseq3](https://github.com/pacificbiosciences/isoseq3/) | Y | - | Scalable de novo isoform discovery |
| [lima](https://github.com/pacificbiosciences/barcoding/) | Y | - | Demultiplex barcoded samples |
| [minorseq](https://github.com/PacificBiosciences/minorseq/) | Y | - | Minor Variant Calling and Phasing Tools |
| [pbbam](https://github.com/pacificbiosciences/pbbam/) | Y | Y | BAM C++ library |
| [pbccs](https://github.com/pacificbiosciences/unanimity/) | Y | - | Generate consensus sequences from single SMRTbells |
| [pbcommand](https://github.com/pacificbiosciences/pbcommand/) | Y | Y | Common models, CLI tool contract and SMRT Link service interface |
| [pbcopper](https://github.com/pacificbiosciences/pbcopper/) | Y | Y | Core C++ library for data structures, algorithms, and utilities |
| [pbcore](https://github.com/pacificbiosciences/pbcore/) | Y | Y | Python library for reading and writing data files |
| [pbcoretools](https://github.com/pacificbiosciences/pbcoretools/) | Y | Y | CLI tools and add-ons for PacBio's core APIs (incl `dataset`) |
| [pblaa](https://github.com/pacificbiosciences/pblaa/) | Y | - | Long amplicon analysis |
| [pbalign](https://github.com/PacificBiosciences/pbalign/) | Y | Y | Python wrapper for BLASR and associated tools |
| [pbmm2](https://github.com/PacificBiosciences/pbmm2/) | Y | Y | A minimap2 frontend for PacBio native data formats |
| [pbsv](https://github.com/pacificbiosciences/pbsv/) | Y | - | Structural variant analysis |

### Combo-Packages
These combine multiple repos into a single bioconda package.

| Package | Linux | Mac | Description |
| - | - | - | - |
| [pb-falcon](https://bioconda.github.io/recipes/pb-falcon/README.html) | Y | - | pypeflow/FALCON/FALCON_unzip |
| [pb-dazzler](https://bioconda.github.io/recipes/pb-dazzler/README.html) | Y | Y | PacBio forks of DALIGNER/DAMASKER/DAZZ_DB/DEXTRACTOR |

### Available Meta-Packages
These include dependencies only. They describe a mutually consistent, well-tested set of versions of all dependencies.

| Package | Linux | Mac | Description |
| - | - | - | - |
| [pb-assembly](https://bioconda.github.io/recipes/pb-assembly/README.html) | Y | - | Everything needed to run Falcon and Unzip |

## FAQ

### Where do I get support?
PacBio tools distributed via bioconda are not covered by any service level
agreement or the like. As such, please *do not* contact a PacBio Field
Applications Scientist or PacBio Customer Service for assistance with any
bioconda releases. We instead provide an
[issue tracker](https://github.com/PacificBiosciences/pbbioconda/issues)
for you to report issues.

### I can't find tool X, when will it be available on bioconda?
We do not provide ETAs for currently not available tools.

### When will a new version of tool X be available?
We do not provide ETAs for our release schedule.

### Will SMRT Link be available on bioconda?
There are no plans. For the latest SMRT Link release, please refer to
currently available [SMRT Link downloads](http://www.pacb.com/products-and-services/analytical-software/).

### Can I get the exact version of the binaries from SMRT Link version XY through bioconda?
There is no effort to keep official [SMRT Link releases](http://www.pacb.com/products-and-services/analytical-software/)
and bioconda binaries in sync.

### Which version of tool X shall I use, from bioconda or from SMRT Link?
If you need ISO-compliant software that has been fully vetted, you must use our
official [SMRT Link software](http://www.pacb.com/products-and-services/analytical-software/).
Bioconda binaries are pre-release versions that adhere to high standards,
but might generate slightly different output, due to bug fixes and/or new features.

### Why is the official SMRT Tools Guide not in sync with bioconda binaries?
Official documentation provided by PacBio is for binaries distributed in stable
[SMRT Link releases](http://www.pacb.com/products-and-services/analytical-software/).
You can click on package names in the table above to get to unofficial,
best effort documentation. Combo- and meta-packages don't necessarily have
additional documentation, as they serve as lightweight, yet well-tested, sets
of existing packages.

### Which operating systems are supported?
All packages are available for **64-bit linux**. Some are available for **64-bit MacOS**.
For details, please study the [table above](#available-packages).
There are no plans to provide darwin binaries for packages currently missing MacOS.
There are no plans to provide executables for Windows.
We do not provide support for WSL (Windows Subsystem for Linux).

## Disclaimer
THIS WEBSITE AND CONTENT AND ALL SITE-RELATED SERVICES, INCLUDING ANY DATA, ARE PROVIDED "AS IS," WITH ALL FAULTS, WITH NO REPRESENTATIONS OR WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTIES OF MERCHANTABILITY, SATISFACTORY QUALITY, NON-INFRINGEMENT OR FITNESS FOR A PARTICULAR PURPOSE. YOU ASSUME TOTAL RESPONSIBILITY AND RISK FOR YOUR USE OF THIS SITE, ALL SITE-RELATED SERVICES, AND ANY THIRD PARTY WEBSITES OR APPLICATIONS. NO ORAL OR WRITTEN INFORMATION OR ADVICE SHALL CREATE A WARRANTY OF ANY KIND. ANY REFERENCES TO SPECIFIC PRODUCTS OR SERVICES ON THE WEBSITES DO NOT CONSTITUTE OR IMPLY A RECOMMENDATION OR ENDORSEMENT BY PACIFIC BIOSCIENCES.
