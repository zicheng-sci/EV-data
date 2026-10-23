# EV data

EV data contains real-world battery operating data from **16 electric buses**, provided by a collaborating industrial partner. Each battery pack consists of **256 series-connected lithium titanate oxide (LTO) cells** and has a **nominal capacity of 115 Ah**.

The onboard battery management system (BMS) records battery pack voltage, cell voltage, current, state of charge (SOC), and temperature probe readings at a **10-second sampling interval**.

## Data organization

The dataset contains **16,568 charging-record CSV files**, organized by vehicle:

```text
.
├── EV data/
│   ├── Vehicle 1/
│   │   └── charge_data/
│   │       ├── 0001.csv
│   │       └── ...
│   ├── ...
│   └── Vehicle 16/
│       └── charge_data/
└── README.md
```

## CSV fields

Each CSV file contains the following seven fields:

| Field | Description |
| --- | --- |
| `voltage` | Battery pack voltage |
| `current` | Battery current |
| `SOC` | State of charge |
| `max_V` | Maximum cell voltage |
| `min_V` | Minimum cell voltage |
| `max_T` | Maximum temperature probe reading |
| `min_T` | Minimum temperature probe reading |
