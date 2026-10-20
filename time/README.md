# Oras at Kalendaryo (Time & Calendar)

2 datasets — 1,389 records

> Browse at [listbase.org/tl/time/](https://listbase.org/tl/time/)

## Datasets

| Name | Records | Size | CSV | Excel | Preview |
|------|---------|------|-----|-------|---------|
| [Mga Pista Opisyal at Espesyal na Araw ng Pilipinas (1988–2030)](tl-mga-pista-opisyal.json) | 708 | 436 KB | [CSV](tl-mga-pista-opisyal_TL.csv) | [Excel](tl-mga-pista-opisyal_TL.xlsx) | [View](https://listbase.org/tl/time/tl-mga-pista-opisyal/) |
| [Mga Pista Opisyal ng Pilipinas — komprehensibo, 4 na wika (1987–2030)](tl-pista-opisyal-completos.json) | 681 | 255 KB | [CSV](tl-pista-opisyal-completos_TL.csv) | [Excel](tl-pista-opisyal-completos_TL.xlsx) | [View](https://listbase.org/tl/time/tl-pista-opisyal-completos/) |

## Quick Start

```bash
# List all time & calendar datasets
curl https://cdn.tl.listbase.org/index.json | jq '.datasets[] | select(.category=="time") | .id'

# Fetch a dataset
curl https://cdn.tl.listbase.org/time/tl-mga-pista-opisyal.json
```

---

[← Back to all categories](../README.md) · [Browse on ListBase](https://listbase.org/tl/time/)
