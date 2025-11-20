# SCION Publications Repository
Welcome to the SCION Publications Repository. This repository serves as a comprehensive archive of all publications related to SCION, including research papers, articles, white papers, and technical reports. The contents of this repository is the source for the [SCION publications list on scion.org](https://www.scion.org/research/).

## 📚 Repository Contents
The repository is structured to maintain:

- **Publication List**: A curated and organized list of all Scion-related publications.
- **PDFs**: Direct access to the full-text PDFs for each publication (where applicable).
- **Metadata**: Information such as author names, publication date, and links to external sources (e.g., journal websites) where available.

## 📁 Directory Structure

```
├── pdfs/
│   ├── 2024/
│   │   ├── publication1.pdf
│   │   ├── publication2.pdf
│   │   └── ...
│   ├── 2023/
│   │   ├── publication1.pdf
│   │   ├── publication2.pdf
│   │   └── ...
│   └── ...
├── README.md
├── categories.json
└── publications.bib
```

- **pdfs/**: This folder contains PDFs of the publications organized by year.
- **publications.bib**: A BibTex (like) file that provides the list of all publications with corresponding metadata and links to the PDFs.
- **categories.json**: The categories that papers can belong to, this is used to categorize papers on the overview.

## 📖 How to Use

### Accessing Publications

- You can browse through the `pdfs/` directory to locate a specific paper by year.
- Alternatively, you can check out the [SCION publications list on scion-architecture.org](https://scion-architecture.net/publications/) for a clickable list of publications with links to download PDFs.

### Adding a New Publication

To contribute a new publication, create a PR in which you:

1. **Create a new directory** for the publication year if it doesn’t exist.
2. **Add the PDF file** of the publication to the corresponding year’s directory.
3. **Update the `publications.bib`** with details about the new publication:
   - Title
   - Author(s)
   - Year of publication
   - Month of publication
   - Publication Venue (e.g. Proceedings of the USENIX Security Symposium)
   - Direct link to the PDF in this repository (if possible)
   - DOI (if applicable)
   - Any extra comments can be added to the comments field
   - Category of the Paper

> [!WARNING]
> The publications.bib file is sorted by date descending, please add your publication at the correct location in the file. (E.g. a new publication is added to the top of the file)

## 📜 BibTex Entry Format

Each publication in the `publications.bib` should follow this format:

```
@inproceedings{Author Last Name + Year + Paper Slug,
	title        = Title of Publication,
	author       = Author Name(s),
	year         = Year of Publication,
	month        = Month of Publication,
	booktitle    = Venue of Publication,
	url          = Direct link to the PDF in this repository, otherwise use a link to the DOI,
	doi          = DOI (if applicable),
    comment      = HTML comment (if applicable),
	keywords     = Category of Publication,
}
```

Example:

```
@inproceedings{conext2021deployment,
	title        = {Deployment and Scalability of an Inter-Domain Multi-Path Routing Infrastructure},
	author       = {Cyrill Kr\\"{a}henb\\"{u}hl and Seyedali Tabaeiaghdaei and Christelle Gloor and Jonghoon Kwon and Adrian Perrig and David Hausheer and Dominik Roos},
	year         = {2021},
	month        = {dec},
	booktitle    = {International Conference on emerging Networking EXperiments and Technologies (CoNEXT ’21)},
	url          = {https://scionproto-contrib.github.io/publications/pdfs/2021/2021_conext_deployment.pdf},
	doi          = {10.1145/3485983.3494862},
	comment         = {Best Paper Award},
	keywords     = {networking}
}
```

## 🏷️ Categories

The categories that can be used in the `keywords` attribute are the keys of the map defined in `categories.json`. If your paper does not fit any of the categories defined in there, you can define a new category by adding a new key and value to the map.

## 🛠️ Contributions

We greatly appreciate contributions from the community. If you wish to add or update publications, please submit a pull request following the guidelines above.

## 📧 Contact

For any inquiries or suggestions regarding this repository, feel free to raise an issue.
