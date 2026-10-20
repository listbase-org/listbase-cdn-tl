# ListBase CDN — Filipino (tl)

Open dataset collection for **Filipino** (Filipino).
433 datasets across 16 categories with 441,856 total records.

> Browse and download at [https://listbase.org/tl/](https://listbase.org/tl/)

## Categories

| Category | Datasets |
|----------|----------|
| [Kultura at Relihiyon (Culture & Religion)](culture/) | 38 |
| [Edukasyon (Education)](education/) | 41 |
| [Libangan (Entertainment)](entertainment/) | 1 |
| [Kapaligiran (Environment)](environment/) | 1 |
| [Pananalapi at Kalakalan (Finance & Trade)](finance/) | 1 |
| [Pagkain (Food & Nutrition)](food/) | 1 |
| [Heograpiya (Geography)](geography/) | 35 |
| [Kalusugan (Health)](health/) | 4 |
| [Kasaysayan (History)](history/) | 1 |
| [Wika (Language)](language/) | 1 |
| [Politika (Politics)](politics/) | 110 |
| [Sanggunian (Reference)](reference/) | 169 |
| [Agham (Science)](science/) | 1 |
| [Lipunan (Society)](society/) | 1 |
| [Oras at Kalendaryo (Time & Calendar)](time/) | 2 |
| [Transportasyon (Transport)](transport/) | 26 |

## Usage

### Browse on the web
Visit [listbase.org/tl/](https://listbase.org/tl/) to search, preview, and download in Excel, CSV, or PDF.

### Fetch via CDN
```bash
# Dataset index (metadata only)
curl https://cdn.tl.listbase.org/index.json

# Full dataset (JSON)
curl https://cdn.tl.listbase.org/geography/th-central-provinces.json

# Download as Excel or CSV
curl -O https://cdn.tl.listbase.org/geography/th-central-provinces_TL.xlsx
curl -O https://cdn.tl.listbase.org/geography/th-central-provinces_TL.csv

# Build dump (metadata + sample rows, gzipped)
curl https://cdn.tl.listbase.org/dump.json.gz | gunzip
```

### Use in JavaScript
```js
const res = await fetch('https://cdn.tl.listbase.org/geography/th-central-provinces.json');
const data = await res.json();
console.log(data.name);    // "ภาคกลาง — จังหวัดในภาคกลาง"
console.log(data.rows);    // [{ ... }, ...]
```

## File Structure

```
├── index.json              # Dataset index (metadata + file info)
├── dump.json.gz            # Build dump (metadata + 20 sample rows per dataset)
├── {category}/
│   ├── README.md           # Category overview
│   ├── {dataset}.json      # Full dataset with rows
│   ├── {dataset}_TL.csv   # CSV download
│   └── {dataset}_TL.xlsx  # Excel download
```

## Dataset JSON Format

Each `.json` file contains:

| Field | Description |
|-------|-------------|
| `id` | Unique dataset identifier |
| `name` | Dataset name |
| `description` | What this dataset contains |
| `category` | Category (e.g. geography, finance) |
| `source` | Data source attribution |
| `updated` | Last updated date |
| `record_count` | Number of records |
| `columns` | Column definitions (key, label, type) |
| `rows` | Array of data records |

## License

Data is provided under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
See individual dataset `source` fields for original data attribution.

---

Part of [ListBase](https://listbase.org) — Free Reference Tables & Lists
