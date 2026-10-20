# Kalusugan (Health)

4 datasets — 796 records

> Browse at [listbase.org/tl/health/](https://listbase.org/tl/health/)

## Datasets

| Name | Records | Size | CSV | Excel | Preview |
|------|---------|------|-----|-------|---------|
| [Mga Pasilidad Pangkalusugang Akreditado ng Maxicare sa Pilipinas](tl-pasilidad-pangkalusugan-maxicare.json) | 399 | 156 KB | [CSV](tl-pasilidad-pangkalusugan-maxicare_TL.csv) | [Excel](tl-pasilidad-pangkalusugan-maxicare_TL.xlsx) | [View](https://listbase.org/tl/health/tl-pasilidad-pangkalusugan-maxicare/) |
| [Mga Klinikang Dental na Akreditado ng Maxicare](tl-klinikang-dental-maxicare.json) | 156 | 65 KB | [CSV](tl-klinikang-dental-maxicare_TL.csv) | [Excel](tl-klinikang-dental-maxicare_TL.xlsx) | [View](https://listbase.org/tl/health/tl-klinikang-dental-maxicare/) |
| [Mga Ospital na Akreditado ng Maxicare](tl-ospital-maxicare.json) | 145 | 54 KB | [CSV](tl-ospital-maxicare_TL.csv) | [Excel](tl-ospital-maxicare_TL.xlsx) | [View](https://listbase.org/tl/health/tl-ospital-maxicare/) |
| [Mga Klinikang Akreditado ng Maxicare](tl-klinika-maxicare.json) | 96 | 39 KB | [CSV](tl-klinika-maxicare_TL.csv) | [Excel](tl-klinika-maxicare_TL.xlsx) | [View](https://listbase.org/tl/health/tl-klinika-maxicare/) |

## Quick Start

```bash
# List all health datasets
curl https://cdn.tl.listbase.org/index.json | jq '.datasets[] | select(.category=="health") | .id'

# Fetch a dataset
curl https://cdn.tl.listbase.org/health/tl-pasilidad-pangkalusugan-maxicare.json
```

---

[← Back to all categories](../README.md) · [Browse on ListBase](https://listbase.org/tl/health/)
