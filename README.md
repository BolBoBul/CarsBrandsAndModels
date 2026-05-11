# CarsBrandsAndModels

A small image dataset of **10,000** car photos organized by brand/model.
Original download link: [here](https://nextcloud.ig.umons.ac.be/s/BooirG6KkHJ58XB)

## Dataset structure

- **10 brands**
- **10 models per brand** (except for `BMW`, `Hyundai` (9) and `Ford` (8))
- **1000 images per brand**

Total: `10 × 1000 = 10,000` images.

## File naming convention

Each image file follows:

`A_Z_Brand_Model_Number.jpg`

Where:

- `A` = `brand_id` (a digit `0–9`)
- `Z` = `model_id` (a digit `0–9`)
- `Brand` = brand name (string)
- `Model` = model name (string)
- `Number` = image global index (a number)

Example:

`3_5_Renault_clio_5062.jpg`

## Brand → models mapping

```js
const carsByBrand = {
  "BMW": ["Serie3Berline", "Serie3Touring", "Serie5", "Serie5Touring", "X2", "X3", "X4", "X5", "i8"],
  "Kia": ["ceed", "ceedsw", "niro", "picanto", "proceed", "rio", "sorento", "sportage", "stinger", "stonic"],
  "Volkswagen": ["Golf", "GolfVariant", "Passat", "Polo", "Sharan", "T-Roc", "T-cross", "Tiguan", "Touareg", "up"],
  "Renault": ["Twingo", "capture", "clio", "grandscenic", "kadjar", "koleos", "megane", "meganegrandtour", "talisman", "talismanbreak"],
  "Opel": ["GrandlandX", "Insigna", "Insignatourer", "astra", "astrabreak", "corsa", "crosslandX", "movano", "vivarofourgon", "zafiralife"],
  "Mercedes": ["CLA", "ClasseCLS", "GLA", "GLC", "GLEcoupe", "classeA", "classeB", "classeC", "classeE", "classeGLK"],
  "Hyundai": ["Newtucson", "Nexo", "Santafe", "i10", "i20", "i30", "i30break", "i30fastback", "kona"],
  "Peugeot": ["2008", "208", "3008", "308berline", "308break", "5008", "508", "508break", "RCZ", "Rifter"],
  "Ford": ["Explorer", "Fiesta", "Focus", "GT", "Galaxy", "Kuga", "Puma", "S-max"],
  "Audi": ["A1", "A3", "A6", "A8", "Q3", "Q5", "Q7", "Q8", "R8", "TT"],
};
```
