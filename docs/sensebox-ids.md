# HiveBox – SenseBox Configuration

HiveBox uses three SenseBoxes from [openSenseMap](https://opensensemap.org/) to retrieve environmental sensor measurements, including temperature.

## Selected SenseBox IDs

| # | SenseBox Name | SenseBox ID | Temperature Sensor |
|---|---|---|---|
| 1 | Groß Glienicke | `5eba5fbad46fb8001b799786` | Yes |
| 2 | Mqd_SchuWg_3A | `5c21ff8f919bf8001adf2488` | Yes |
| 3 | Natur Pur | `5ade1acf223bd80019a1011c` | Yes |

## Data Source

[openSenseMap](https://opensensemap.org/)

The application retrieves sensor measurements through the openSenseMap REST API.

**API Base URL:**
`https://api.opensensemap.org/boxes/`

## Data Validation

All three SenseBoxes were successfully queried using Python and the `requests` library.

The following temperature readings were observed during testing:

| SenseBox | Temperature | Last Measurement |
|---|---:|---|
| Groß Glienicke | 9.45 °C | 2026-10-31 |
| Mqd_SchuWg_3A | 12.36 °C | 2026-10-31 |
| Natur Pur | 12.20 °C | 2026-10-17 |

## Notes

- All selected SenseBoxes provide temperature measurements in Celsius (°C).
- The latest temperature measurement timestamps may differ between SenseBoxes.
- The third SenseBox had an older temperature reading during validation.
- Sensor measurements may change over time.

