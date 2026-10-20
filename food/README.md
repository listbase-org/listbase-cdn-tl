# Pagkain (Food & Nutrition)

1 datasets — 108 records

> Browse at [listbase.org/tl/food/](https://listbase.org/tl/food/)

## Datasets

| Name | Records | Size | CSV | Excel | Preview |
|------|---------|------|-----|-------|---------|
| [Mga Restawran ng Michelin Guide sa Pilipinas](tl-restawran-michelin.json) | 108 | 114 KB | [CSV](tl-restawran-michelin_TL.csv) | [Excel](tl-restawran-michelin_TL.xlsx) | [View](https://listbase.org/tl/food/tl-restawran-michelin/) |

## Quick Start

```bash
# List all food & nutrition datasets
curl https://cdn.tl.listbase.org/index.json | jq '.datasets[] | select(.category=="food") | .id'

# Fetch a dataset
curl https://cdn.tl.listbase.org/food/tl-restawran-michelin.json
```

---

[← Back to all categories](../README.md) · [Browse on ListBase](https://listbase.org/tl/food/)
