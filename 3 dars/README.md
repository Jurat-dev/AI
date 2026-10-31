# 3-dars — yaqinlashayotgan ultra-trail poygalari

ITRA dan yig‘ilgan kelgusi ultra-trail poygalari. Jadval `upcoming-ultra-trails.csv` da, tahlil uchun bo‘sh daftarcha `3_dars.ipynb`.

## Ma’lumotlar

| | |
|---|---|
| Qatorlar | 1233 ta poyga |
| Mamlakatlar | 81 |
| Sanalar | 2026-10-26 — 2027-12-04 |
| GPX havolasi bor | 816 ta poyga |
| Manba | [itra.run](https://itra.run) |
| Yig‘ilgan vaqt | 2026-10-25 |

## Ustunlar

| Ustun | Ma’nosi |
|---|---|
| `event_date` | Poyga sanasi |
| `name` | Masofa nomi (masalan, 100K, 100 Miles) |
| `distance_km` | Masofa, km |
| `elevation_gain_m` | Ko‘tarilish, m |
| `elevation_loss_m` | Tushish, m |
| `gpx_url` | Marshrut GPX havolasi (bo‘sh bo‘lishi mumkin) |
| `event_name` | Tadbir nomi |
| `country` | Mamlakat kodi (ISO 3166-1 alpha-3) |
| `locality` | Joy |
| `source_url` | ITRA sahifasi |
| `source` | Manba (`itra`) |
| `schema_version` | Jadval sxemasi versiyasi |
| `scraped_at` | Yozuv olingan vaqt (UTC) |

## Ochish

```python
import pandas as pd

df = pd.read_csv("upcoming-ultra-trails.csv", parse_dates=["event_date", "scraped_at"])
df.head()
```
