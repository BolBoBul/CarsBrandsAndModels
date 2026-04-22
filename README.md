# CarsBrandsAndModels

A small image dataset of **10,000** car photos organized by brand/model.

## Dataset structure

- **10 brands**
- **10 models per brand**
- **100 images per (brand, model) combination**

Total: `10 × 10 × 100 = 10,000` images.

## File naming convention

Each image file follows:

`A_B_Brand_Model_Number.jpg`

Where:

- `A` = `brand_id` (a digit `0–9`)
- `B` = `model_id` (a digit `0–9`)
- `Brand` = brand name (string)
- `Model` = model name (string)
- `Number` = image index within the (brand, model) pair (typically `0–99`)

Example:

`3_7_Ford_Puma_42.jpg`

## Brand → models mapping

```js
const carsByBrand = {
  "Audi": ["A1", "A3", "A6", "A8", "Q3", "Q5", "Q7", "Q8", "R8", "TT"],
  "BMW": ["Serie3Berline", "Serie3Touring", "Serie5", "Serie5Touring", "X2", "X3", "X4", "X5", "i8"],
  "Ford": ["Explorer", "Fiesta", "Focus", "GT", "Galaxy", "Kuga", "Puma", "S-max"],
  "Hyundai": ["Newtucson", "Nexo", "Santafe", "i10", "i20", "i30", "i30break", "i30fastback", "kona"],
  "Kia": ["ceed", "ceedsw", "niro", "picanto", "proceed", "rio", "sorento", "sportage", "stinger", "stonic"],
  "Mercedes": ["CLA", "ClasseCLS", "GLA", "GLC", "GLEcoupe", "classeA", "classeB", "classeC", "classeE", "classeGLK"],
  "Opel": ["GrandlandX", "Insigna", "Insignatourer", "astra", "astrabreak", "corsa", "crosslandX", "movano", "vivarofourgon", "zafiralife"],
  "Peugeot": ["2008", "208", "3008", "308berline", "308break", "5008", "508", "508break", "RCZ", "Rifter"],
  "Renault": ["Twingo", "capture", "clio", "grandscenic", "kadjar", "koleos", "megane", "meganegrandtour", "talisman", "talismanbreak"],
  "Volkswagen": ["Golf", "GolfVariant", "Passat", "Polo", "Sharan", "T-Roc", "T-cross", "Tiguan", "Touareg", "up"],
};
```

> Note: Some brands above currently list fewer than 10 models. If your dataset truly contains 10 models per brand, the mapping may be incomplete and can be updated.

## License

Add your dataset/license terms here (e.g., CC BY 4.0, CC BY-NC, custom license, etc.).
