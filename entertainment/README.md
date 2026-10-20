# Libangan (Entertainment)

1 datasets — 115 records

> Browse at [listbase.org/tl/entertainment/](https://listbase.org/tl/entertainment/)

## Datasets

| Name | Records | Size | CSV | Excel | Preview |
|------|---------|------|-----|-------|---------|
| [Filipino films (mga pelikulang Pilipino)](tl-pelikulang-pilipino.json) | 115 | 557 KB | [CSV](tl-pelikulang-pilipino_TL.csv) | [Excel](tl-pelikulang-pilipino_TL.xlsx) | [View](https://listbase.org/tl/entertainment/tl-pelikulang-pilipino/) |

## Quick Start

```bash
# List all entertainment datasets
curl https://cdn.tl.listbase.org/index.json | jq '.datasets[] | select(.category=="entertainment") | .id'

# Fetch a dataset
curl https://cdn.tl.listbase.org/entertainment/tl-pelikulang-pilipino.json
```

---

[← Back to all categories](../README.md) · [Browse on ListBase](https://listbase.org/tl/entertainment/)
