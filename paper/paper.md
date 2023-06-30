---
title: 'BioHackJP 2023 Report R3: Expand the pathway analysis environment to non-model organisms'
title_short: 'WikiPathways + Pathway Figure OCR'
tags:
  - Pathways
  - Non-model organisms
  - Literature mining
  - Figure OCR
  - Pathway modeling tools
  - Species annotation
authors:
  - name: Alexander Pico
    orcid: 0000-0001-5706-2163
    affiliation: 1
  - name: Hiromasa Ono
    orcid: 0000-0001-8675-963X
    affiliation: 2
  - name: Ryo Nozu
    orcid: 0000-0002-1099-3152
    affiliation: 3
  - name: Naoya Oishi
    orcid: 0000-0002-7491-4994
    affiliation: 4
  - name: Hidemasa Bono
    orcid: 0000-0003-4413-0651
    affiliation: 5
affiliations:
  - name: Institute of Data Science and Biotechnology, Gladstone Institutes, UCSF, San Francisco, CA, USA
    index: 1
  - name: Database Center for Life Science, Joint Support-Center for Data Science Research, Research Organization of Information and Systems, kashiwa, Japan
    index: 2
  - name: Guraduate School of Integrated Science for Life, Hiroshima University, Higashi-Hiroshima, Japan
    index: 3
  - name: dogrun. Inc, shizuoka, Japan
    index: 4
  - name: Genome Editing Innovation Center, Hiroshima University, Higashi-Hiroshima, Japan
    index: 5
date: 30 June 2023
cito-bibliography: paper.bib
event: BH23JP
biohackathon_name: "BioHackathon Japan 2023"
biohackathon_url:   "https://2023.biohackathon.org/"
biohackathon_location: "Kagawa, Japan, 2023"
group: R3
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackathon-jp/bh23-WikiPathways
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: First Author \emph{et al.}
---

# Background

* Expand the pathway analysis environment to non-model organisms where genome and functional annotations are not organized in the central public database
  * How to make use of Pathway Figure OCR https://pfocr.wikipathways.org/ (in WikiPathways https://www.wikipathways.org/) extracted from PMC
  * Functional annotation of no-model organisms’ genes in omic scale


# Outcomes

- Give a lecture on how to use [PathVisio](https://pathvisio.org), a tool for drawing, editing, and analyzing biological pathways. (pico to all)
    - In a particular environment (M1 Mac, Ventura 13.4.1), we could not install it following the [existing documentation](https://pathvisio.org/downloads) (especially the Java 8 setup), so we hacked a way to install it in those environments and [posted an issue](https://github.com/PathVisio/pathvisio/issues/195) on [it's GitHub repository](https://github.com/PathVisio/pathvisio) so that it could be reflected. (ono)
- Create (or edit) and publish several pathway diagrams using PathVisio
    - Representative anthocyanin biosynthetic pathway ([WP5391](https://www.wikipathways.org/pathways/WP5391.html)) (Bono)
    - CBD synthetic pathway ([WP5392](https://www.wikipathways.org/pathways/WP5392.html)) (Oishi)
    - Network map of SARS-CoV-2 signaling pathway ([WP5115](https://www.wikipathways.org/pathways/WP5115.html)) (Ono)

![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

# Future work

In the Python environment, py4cytoscape can be used to convert from DataFrame to Cytoscape format, but it is not possible to further convert from there to WikiPathways format. We believe that the ability to describe a GPML template from a generic description, such as tab-delimited text, would be an efficient pathway rendering method, and we will continue discussions on a conversion tool for this purpose.

## Acknowledgements

We would like to thank the fellow participants at BioHackathon 2023 for their collaboration and constructive advice, which greatly influenced our project. We are grateful to the organizers for providing this platform and the developers of open source language models. Special thanks to our mentors, advisors, and colleagues for their guidance and support. Without their contributions, our project in linked data standardization with LLMs in bioinformatics would not have been possible.

## References

1.
