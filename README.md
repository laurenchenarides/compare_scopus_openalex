# Problem setup

The topic of this project is data quality, specifically the quality of metadata used to populate data usage statistics about the authors and their institutions who use USDA produced datasets. This goal of this project is to verify whether the source data correctly identifies and counts unique individuals and institutions.

### Key words
- Record linkage
- De-duplication
- Name entity recognition
- Entity resolution
- Information retrieval

## Tasks

1. **Disambiguate AUTHORS** (`openalex_authors.csv`)

2. **Disambiguate INSTITUTIONS**
   - Use IPEDS - unique institution ID published by the department of education
   - [nces.ed.gov](https://nces.ed.gov)
   - Once you get the IPEDS information, you can look across university types

### Matching Methods
- Rule based (if then)
- Probabilistic (fuzzy matching)
- Machine Learning

#### What other information to create a matching method:
- **Open Alex**
  - Authors
  - Institution
  - ORCIDs
  - DOIs
- **Scopus fields**
  - Information about the publications, etc.
  - Institution
  - SCOPUS Authors
  - SCOPUS ID

## Deliverable

1. After disambiguating the authors and institutions, re-match between Scopus and OpenAlex.
    - How much of Rafael's Venn diagram was noise?
    - How many people do we get before and after deduplication?
2. Create a cross-walk
    - What is the value in publishing with a publisher versus open source?
3. Analysis, described below
    - Where are the gaps in the publications using USDA data?
    - Where could those gaps be closed?

## Resources

- Packages to use record linkages - British Gov website
  [Splink MOJ's open-source library](https://www.gov.uk/government/publications/joined-up-data-in-government-the-future-of-data-linking-methods/splink-mojs-open-source-library-for-probabilistic-record-linkage-at-scale)

- Record linkage examples in Python
  [Coleridge Initiative](https://textbook.coleridgeinitiative.org/chap-link.html)

- NCSES Report -- how to link to the IPEDS data  
  `2024.07.24_NCSES_MSI-Report_rev.docx`  
  *Waiting to receive it from Julia*

## Time frame

- 2-3 months

### Next steps
- Next meeting is set for **November 11th**
- Get familiar with the two different sets
- Get familiar with IPEDS
- How many people do we get before and after de-duplication?
