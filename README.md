# Dutch Names Dataset (First Names & Surnames)

This repository contains structured JSON datasets of **Dutch first names** and **Dutch surnames**, including frequency counts.  
The data was scraped from publicly available online databases maintained by Dutch cultural and genealogical institutions and then cleaned and normalized.

## Contents

- `firstnames.json`  
  All unique first names, sorted alphabetically.

- `firstnames_by_count.json`  
  First names sorted by total frequency (men + women).

- `lastnames.json`  
  All unique surnames, sorted alphabetically.

- `lastnames_by_count.json`  
  Surnames sorted by frequency (number of bearers in 2007).

## Data Processing & Normalization

The datasets in this repository are **not verbatim copies** of the original sources.  
The following transformations were applied:

- **Capitalization normalization**
  - Identical names differing only by capitalization were merged with their respective counts summed.
  - Final formatting follows standard Dutch name conventions (e.g. `van den Berg`).

- **No semantic changes**
  - No names were added, removed, translated, or altered beyond normalization
  - Frequency counts were preserved exactly as scraped

## Data Structure

### First Names
```json
{
  "Voornaam": "Jan",
  "Mannen": 376312,
  "Vrouwen": 685
}
```
### Surnames
```json
{
  "familienaam": "de Jong",
  "aantal_2007": 84092,
  "lemma": "de Jong"
}
```
## License & Attribution

This repository redistributes **scraped and reformatted data** derived from publicly accessible sources for **research, educational, and non-commercial use**.

Original data remains the intellectual property of its respective institutions:

- Meertens Instituut (first names)
- Central Bureau of Genealogy (CBG) (surnames)

## Disclaimer

This dataset is provided **as-is**, without warranty of correctness or completeness.  
It should not be used as an authoritative source for legal, administrative, or genealogical decisions.
