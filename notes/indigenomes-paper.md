**What question were they answering, and why does it need India-specific data?**

The paper sets out to describe the distribution of genetic variants — their allele counts and frequencies — across the Indian population. Large public references such as gnomAD and the 1000 Genomes Project cover many populations, but India, at roughly 17% of the world's population, is thinly represented in them.

India-specific data matters because of how the population is structured. The country has more than 4,500 anthropologically distinct groups, many of them endogamous, with consanguineous marriage common in some. This produces variants that are frequent within a specific community but rare or absent elsewhere. In a pooled global cohort such variants look rare, and a rarity-based clinical filter would flag them as potentially disease-causing when they are, in context, common and benign.

Without a large-scale Indian reference, those variants are not documented at all. The paper aims to close that gap by cataloguing and annotating them, as a foundation for precision medicine and genetic disease research in India.

**What did they actually build, and from what?**

IndiGenomes is a browsable web database of 55,898,122 single-allelic variants, called from whole-genome sequences of 1,029 self-declared healthy individuals recruited from geographically distinct regions of India. For each variant it reports allele count, allele number, allele frequency, and the number of heterozygous and homozygous carriers, alongside annotations drawn from public resources — functional consequence, pathogenicity predictors, and frequencies in gnomAD, 1000 Genomes, ExAC, ESP6500, and GME, plus ClinVar clinical significance.

Comparison against gnomAD and 1000 Genomes showed 18,016,257 variants (about 32%) present in neither database.

**Limitations stated, and the one I'd add**

The authors do not present a dedicated limitations section. They note that the current release contains single-allelic variants only, with multi-allelic and structural variants deferred to future updates.

The limitation I would add is representation. The cohort is described as geographically distinct, but the paper's own motivation is that Indian genetic diversity is organised by community, not geography — it is endogamy that produces the community-specific variants the resource exists to capture. 1,029 individuals sampled by region cannot cover 4,500 endogamous groups, and the paper does not report which communities are represented or how many samples each contributes. As a result, a user cannot tell whether a variant labelled "common in India" is common across India or common in a handful of well-sampled communities. For the resource's core use case — filtering out benign-but-locally-common variants in a rare-disease pipeline — that distinction is the whole point.

Another limitation is that health status was self-declared by volunteers, not clinically assessed. Late-onset conditions — cardiac disease, many cancers — would not yet have appeared in younger participants, so their variants are in the database under a "healthy" label. The database therefore cannot be read as a catalogue of benign variation. A volunteer pool also likely skews toward urban, educated groups with access to the recruiting institutions, which compounds the community-representation gap above rather than being independent of it.

A secondary concern: the 18 million variants absent from gnomAD and 1000 Genomes are presented without orthogonal validation, so a reader cannot judge what fraction reflect genuine Indian-specific variation versus platform or calling artefacts.
