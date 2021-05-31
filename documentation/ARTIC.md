## genome amplification using ARTIC amplicons 

#### The full document can be read in [this repository][1]

### Background
The [ARTIC Network][2] is a collaborative project between a number of laboratories around the
world that wants to provide protocols and advice on viral outbreaks. Their website states
that part of their goal is to develop "an end-to-end system for processing samples from
viral outbreaks to generate real-time epidemiological information that is interpretable
and actionable by public health bodies."

The ARTIC network has made available laboratory protocols, primer sets and bioinformatics
workflows. The protocol they use relies on targeted amplification of viral sequences using
tiled, multiplexed primers, an approach [first described for Zika virus sequencing][3].

Since this approach, as the ARTIC website states, "has been proven to have high sensitivity
and work directly from clinical samples (compared to metagenomics approaches)", it has been
widely adopted by groups worldwide and a fair percentage of the COVID genome sequences
uploaded to GISAID and raw reads uploaded to the SRA have been produced by this method.

Along with the laboratory protocols for sequencing (both for Illumina and Nanopore
sequencing technologies), several tools and workflows have been developed to handle what
is essentially non-random sequencing data.

### Analyzing ARTIC data with Galaxy

#### What's the point?

Our goal is to enable and provide state-of-the-art workflows for the analysis of SARS-CoV-2
ARTIC data using the Galaxy platform.

While it is possible to treat ARTIC data like regular whole-genome sequencing (WGS) data
and analyze it with WGS workflows like the ones we developed for the [analysis of
within-samples variation][4], failure to take the specific nature of the data, and
specifically the presence of amplicon primer sequences, into account would lead to
suboptimal results.

### Continued [Here][1]




[1]: https://github.com/galaxyproject/SARS-CoV-2/blob/master/artic/README.md
[2]: https://artic.network/
[3]: https://www.nature.com/articles/nprot.2017.066
[4]: https://github.com/galaxyproject/SARS-CoV-2/blob/master/genomics/4-Variation