# DBahn-berlin data
This repository stores hourly-sampled data under `timetables/` compressed into weekly `.tar.gz` archives.
Additionally, it contains the 15-minutes sampled data under `timetable_changes/` compressed into weekly `.tar.gz` archives.

## Directory Layout
* **Weekly bins:** Fixed 7-day windows anchored at the earliest folder date.
* **Archive name:** `YYMMDD_YYMMDD.tar.gz` (second date is exclusive).
* **Archive contents:** The hourly folders for that week (e.g., 2509021200/, 2509021300/, …).
* **Timetable_changes:** Similar structure but every folder inside contains the timetime changes for every 15 minutes.
```bash
.
└─ timetables/                # compressed weekly bundles
   ├─ 250902_250909.tar.gz    # [2025-09-02, 2025-09-09)  (end date exclusive)
    ├─ 2509021200/            # YYMMDDHHMM  → 2025-09-02 12:00
    │─ ...                    # ...
    │─ 2509092300/            # 2025-09-09 23:00 (example last)
   ├─ 250909_250916.tar.gz
   └─ ...
```

