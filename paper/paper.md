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
  - name: Next Author
    orcid: 0000-0000-0000-0000
    affiliation: 2
  - name: Next Author
    orcid: 0000-0000-0000-0000
    affiliation: 3
  - name: Next Author
    orcid: 0000-0000-0000-0000
    affiliation: 4
  - name: Next Author
    orcid: 0000-0000-0000-0000
    affiliation: 5
affiliations:
  - name: Institute of Data Science and Biotechnology, Gladstone Institutes, UCSF, San Francisco, CA, USA
    index: 1
  - name: Second Affiliation
    index: 2
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


* Give a lecture on how to use PathVisio, a tool for drawing, editing, and analyzing biological pathways. (pico to all)
  * In some environments (M1 Mac, Ventura 13.4.1), we could not install it following the existing documentation (especially the Java 8 setup), so we hacked a way to install it in those environments and posted an issue on it’s GitHub repository to have them reflected. (ono)
* Create (or edit) and publish several pathway diagrams using PathVisio
  * Representative anthocyanin biosynthetic pathway (WP5391) (Bono)
  * CBD synthetic pathway (WP5392) (Oishi)
  * Network map of SARS-CoV-2 signaling pathway (WP5115) (Ono)

![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

# Future work

In the Python environment, py4cytoscape can be used to convert from DataFrame to Cytoscape format, but it is not possible to further convert from there to WikiPathways format. We believe that the ability to describe a GPML template from a generic description, such as tab-delimited text, would be an efficient pathway rendering method, and we will continue discussions on a conversion tool for this purpose.

## Acknowledgements

We would like to thank the fellow participants at BioHackathon 2023 for their collaboration and constructive advice, which greatly influenced our project. We are grateful to the organizers for providing this platform and the developers of open source language models. Special thanks to our mentors, advisors, and colleagues for their guidance and support. Without their contributions, our project in linked data standardization with LLMs in bioinformatics would not have been possible.

## References

1.
