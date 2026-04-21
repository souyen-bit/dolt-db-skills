# Costco (COST) — FY2018–FY2025 Financial Analysis

**Generated:** 2026-04-21
**Source:** /analyze-financials skill

---

## Years Analyzed

- **Dolt DB prior:** FY2018–FY2024
- **Yahoo Finance:** FY2021–FY2025
- **Union analyzed:** 2018, 2019, 2020, 2021, 2022, 2023, 2024, 2025

**Note on FY2019 SEC fetch:** The SEC MCP returned quarterly data for FY2019. Annual income statement values are sourced from the FY2020 10-K comparative columns (most recent filing version), which agree exactly with the Dolt values.

---

## Anomaly Detection

### [ERROR] FY2019 — Balance Sheet Copied from FY2018

Every balance sheet field in Dolt for FY2019 is identical to the FY2018 values — a clear copy/paste error. Income statement data is correct but the entire balance sheet must be replaced.

| Field | Dolt (wrong) | SEC Correct |
|-------|------------|-------------|
| Inventory | 11,040,000 | **11,395,000** |
| Current Assets | 20,289,000 | **23,485,000** |
| Total Assets | 40,830,000 | **45,400,000** |
| Current Liabilities | 19,926,000 | **23,237,000** |
| Liabilities | 27,727,000 | **29,816,000** |
| Total SE | 13,103,000 | **15,584,000** |
| Total L&SE | 40,830,000 | **45,400,000** |

Identity check on corrected values: 29,816,000 + 15,584,000 = 45,400,000 ✓

### [WARNING] FY2020 — SGA Restatement (Preopening Reclassified)

The FY2022 10-K restated FY2020 SGA to include preopening expenses (originally a separate $55M line item).

| Source | SGA |
|--------|-----|
| FY2020 10-K (original) | 16,332,000 |
| FY2022 10-K (restated) | **16,387,000** |
| Dolt current | 16,332,000 |

Recommended: **16,387,000**

### [WARNING] FY2021 — SGA Restatement (Preopening Reclassified)

FY2022/FY2023 10-K restated FY2021 SGA to include preopening ($76M).

| Source | SGA |
|--------|-----|
| FY2021 10-K (original) | 18,461,000 |
| FY2022 10-K (restated) | **18,537,000** |
| Dolt current | 18,461,000 |

Recommended: **18,537,000**

### [WARNING] FY2018 & FY2019 — Preopening Excluded from SGA (No Official Restatement)

- FY2018: preopening = 68,000 (SGA as filed = 13,876,000)
- FY2019: preopening = 86,000 (SGA as filed = 14,994,000)

Most recent filings showing these years (FY2020 and FY2021 10-Ks) still present preopening separately. No official restatement exists for these years. Current Dolt values are the best available; no mandatory change.

### [INFO] FY2025 — New Year (Not Yet in Dolt)

FY2025 ended 2025-08-31. SEC and Yahoo agree on all fields. Identity check passes. Row ready to insert.

---

## Gross Margin Sanity Checks (Expected 10–15% for Warehouse Clubs)

| Year | Gross Margin | GM% | Status |
|------|-------------|-----|--------|
| 2018 | 18,424,000 | 13.0% | ✓ |
| 2019 | 19,817,000 | 13.0% | ✓ |
| 2020 | 21,822,000 | 13.1% | ✓ |
| 2021 | 25,245,000 | 12.9% | ✓ |
| 2022 | 27,572,000 | 12.1% | ✓ |
| 2023 | 29,704,000 | 12.3% | ✓ |
| 2024 | 32,095,000 | 12.6% | ✓ |
| 2025 | 35,349,000 | 12.8% | ✓ |

---

## Balance Sheet Identity Checks

| Year | Liabilities + SE | Total Assets | Status |
|------|-----------------|--------------|--------|
| 2018 | 27,727,000 + 13,103,000 = 40,830,000 | 40,830,000 | ✓ |
| 2019 (corrected) | 29,816,000 + 15,584,000 = 45,400,000 | 45,400,000 | ✓ |
| 2019 (Dolt) | 27,727,000 + 13,103,000 = 40,830,000 | 40,830,000 | [ERROR] wrong values |
| 2020 | 36,851,000 + 18,705,000 = 55,556,000 | 55,556,000 | ✓ |
| 2021 | 41,190,000 + 18,078,000 = 59,268,000 | 59,268,000 | ✓ |
| 2022 | 43,519,000 + 20,647,000 = 64,166,000 | 64,166,000 | ✓ |
| 2023 | 43,936,000 + 25,058,000 = 68,994,000 | 68,994,000 | ✓ |
| 2024 | 46,209,000 + 23,622,000 = 69,831,000 | 69,831,000 | ✓ |
| 2025 | 47,935,000 + 29,164,000 = 77,099,000 | 77,099,000 | ✓ |

---

## Side-by-Side Comparison Tables (all values in $thousands)

### FY2018 (reportDate: 2018-09-02)

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 141,576,000 | N/A | 141,576,000 | 141,576,000 |
| Cost of Goods | 123,152,000 | N/A | 123,152,000 | 123,152,000 |
| Gross Margin | 18,424,000 | N/A | 18,424,000 | 18,424,000 |
| SGA | 13,876,000 | N/A | 13,876,000 | 13,876,000 |
| Operating Profit | 4,480,000 | N/A | 4,480,000 | 4,480,000 |
| Net Profit | 3,134,000 | N/A | 3,134,000 | 3,134,000 |
| Inventory | 11,040,000 | N/A | 11,040,000 | 11,040,000 |
| Current Assets | 20,289,000 | N/A | 20,289,000 | 20,289,000 |
| Total Assets | 40,830,000 | N/A | 40,830,000 | 40,830,000 |
| Current Liabilities | 19,926,000 | N/A | 19,926,000 | 19,926,000 |
| Liabilities | 27,727,000 | N/A | 27,727,000 | 27,727,000 |
| Total SE | 13,103,000 | N/A | 13,103,000 | 13,103,000 |
| Total L&SE | 40,830,000 | N/A | 40,830,000 | 40,830,000 |

**Verdict: No changes needed.**

---

### FY2019 (reportDate: 2019-09-01)

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 152,703,000 | N/A | 152,703,000 | 152,703,000 |
| Cost of Goods | 132,886,000 | N/A | 132,886,000 | 132,886,000 |
| Gross Margin | 19,817,000 | N/A | 19,817,000 | 19,817,000 |
| SGA | 14,994,000 | N/A | 14,994,000 | 14,994,000 |
| Operating Profit | 4,737,000 | N/A | 4,737,000 | 4,737,000 |
| Net Profit | 3,659,000 | N/A | 3,659,000 | 3,659,000 |
| Inventory | 11,395,000 | N/A | **11,040,000*** | **11,395,000** |
| Current Assets | 23,485,000 | N/A | **20,289,000*** | **23,485,000** |
| Total Assets | 45,400,000 | N/A | **40,830,000*** | **45,400,000** |
| Current Liabilities | 23,237,000 | N/A | **19,926,000*** | **23,237,000** |
| Liabilities | 29,816,000 | N/A | **27,727,000*** | **29,816,000** |
| Total SE | 15,584,000 | N/A | **13,103,000*** | **15,584,000** |
| Total L&SE | 45,400,000 | N/A | **40,830,000*** | **45,400,000** |

**Verdict: [ERROR] All 7 balance sheet fields are wrong in Dolt. Must correct.**

---

### FY2020 (reportDate: 2020-08-30)

| Field | SEC (original) | SEC (restated FY2022) | Yahoo | Dolt | Recommended |
|-------|----------------|----------------------|-------|------|-------------|
| Net Revenue | 166,761,000 | 166,761,000 | N/A | 166,761,000 | 166,761,000 |
| Cost of Goods | 144,939,000 | 144,939,000 | N/A | 144,939,000 | 144,939,000 |
| Gross Margin | 21,822,000 | 21,822,000 | N/A | 21,822,000 | 21,822,000 |
| SGA | 16,332,000 | **16,387,000*** | N/A | **16,332,000*** | **16,387,000** |
| Operating Profit | 5,435,000 | 5,435,000 | N/A | 5,435,000 | 5,435,000 |
| Net Profit | 4,002,000 | 4,002,000 | N/A | 4,002,000 | 4,002,000 |
| Inventory | 12,242,000 | 12,242,000 | N/A | 12,242,000 | 12,242,000 |
| Current Assets | 28,120,000 | 28,120,000 | N/A | 28,120,000 | 28,120,000 |
| Total Assets | 55,556,000 | 55,556,000 | N/A | 55,556,000 | 55,556,000 |
| Current Liabilities | 24,844,000 | 24,844,000 | N/A | 24,844,000 | 24,844,000 |
| Liabilities | 36,851,000 | 36,851,000 | N/A | 36,851,000 | 36,851,000 |
| Total SE | 18,705,000 | 18,705,000 | N/A | 18,705,000 | 18,705,000 |
| Total L&SE | 55,556,000 | 55,556,000 | N/A | 55,556,000 | 55,556,000 |

**Verdict: [WARNING] Update SGA from 16,332,000 → 16,387,000.**

---

### FY2021 (reportDate: 2021-08-29)

| Field | SEC (original) | SEC (restated FY2022) | Yahoo | Dolt | Recommended |
|-------|----------------|----------------------|-------|------|-------------|
| Net Revenue | 195,929,000 | 195,929,000 | N/A† | 195,929,000 | 195,929,000 |
| Cost of Goods | 170,684,000 | 170,684,000 | N/A† | 170,684,000 | 170,684,000 |
| Gross Margin | 25,245,000 | 25,245,000 | N/A† | 25,245,000 | 25,245,000 |
| SGA | 18,461,000 | **18,537,000*** | N/A† | **18,461,000*** | **18,537,000** |
| Operating Profit | 6,708,000 | 6,708,000 | N/A† | 6,708,000 | 6,708,000 |
| Net Profit | 5,007,000 | 5,007,000 | N/A† | 5,007,000 | 5,007,000 |
| Inventory | 14,215,000 | 14,215,000 | N/A† | 14,215,000 | 14,215,000 |
| Current Assets | 29,505,000 | 29,505,000 | N/A† | 29,505,000 | 29,505,000 |
| Total Assets | 59,268,000 | 59,268,000 | N/A† | 59,268,000 | 59,268,000 |
| Current Liabilities | 29,441,000 | 29,441,000 | N/A† | 29,441,000 | 29,441,000 |
| Liabilities | 41,190,000 | 41,190,000 | N/A† | 41,190,000 | 41,190,000 |
| Total SE | 18,078,000 | 18,078,000 | N/A† | 18,078,000 | 18,078,000 |
| Total L&SE | 59,268,000 | 59,268,000 | N/A† | 59,268,000 | 59,268,000 |

†Yahoo FY2021 data mostly NaN — not usable.

**Verdict: [WARNING] Update SGA from 18,461,000 → 18,537,000.**

---

### FY2022 (reportDate: 2022-08-28)

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 226,954,000 | 226,954,000 | 226,954,000 | 226,954,000 |
| Cost of Goods | 199,382,000 | 199,382,000 | 199,382,000 | 199,382,000 |
| Gross Margin | 27,572,000 | 27,572,000 | 27,572,000 | 27,572,000 |
| SGA | 19,779,000 | 19,779,000 | 19,779,000 | 19,779,000 |
| Operating Profit | 7,793,000 | 7,793,000 | 7,793,000 | 7,793,000 |
| Net Profit | 5,844,000 | 5,844,000 | 5,844,000 | 5,844,000 |
| Inventory | 17,907,000 | 17,907,000 | 17,907,000 | 17,907,000 |
| Current Assets | 32,696,000 | 32,696,000 | 32,696,000 | 32,696,000 |
| Total Assets | 64,166,000 | 64,166,000 | 64,166,000 | 64,166,000 |
| Current Liabilities | 31,998,000 | 31,998,000 | 31,998,000 | 31,998,000 |
| Liabilities | 43,519,000 | 43,519,000 | 43,519,000 | 43,519,000 |
| Total SE | 20,647,000 | 20,647,000 | 20,647,000 | 20,647,000 |
| Total L&SE | 64,166,000 | 64,166,000 | 64,166,000 | 64,166,000 |

**Verdict: No changes needed.**

---

### FY2023 (reportDate: 2023-09-03)

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 242,290,000 | 242,290,000 | 242,290,000 | 242,290,000 |
| Cost of Goods | 212,586,000 | 212,586,000 | 212,586,000 | 212,586,000 |
| Gross Margin | 29,704,000 | 29,704,000 | 29,704,000 | 29,704,000 |
| SGA | 21,590,000 | 21,590,000 | 21,590,000 | 21,590,000 |
| Operating Profit | 8,114,000 | 8,114,000 | 8,114,000 | 8,114,000 |
| Net Profit | 6,292,000 | 6,292,000 | 6,292,000 | 6,292,000 |
| Inventory | 16,651,000 | 16,651,000 | 16,651,000 | 16,651,000 |
| Current Assets | 35,879,000 | 35,879,000 | 35,879,000 | 35,879,000 |
| Total Assets | 68,994,000 | 68,994,000 | 68,994,000 | 68,994,000 |
| Current Liabilities | 33,583,000 | 33,583,000 | 33,583,000 | 33,583,000 |
| Liabilities | 43,936,000 | 43,936,000 | 43,936,000 | 43,936,000 |
| Total SE | 25,058,000 | 25,058,000 | 25,058,000 | 25,058,000 |
| Total L&SE | 68,994,000 | 68,994,000 | 68,994,000 | 68,994,000 |

**Verdict: No changes needed.**

---

### FY2024 (reportDate: 2024-09-01)

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 254,453,000 | 254,453,000 | 254,453,000 | 254,453,000 |
| Cost of Goods | 222,358,000 | 222,358,000 | 222,358,000 | 222,358,000 |
| Gross Margin | 32,095,000 | 32,095,000 | 32,095,000 | 32,095,000 |
| SGA | 22,810,000 | 22,810,000 | 22,810,000 | 22,810,000 |
| Operating Profit | 9,285,000 | 9,285,000 | 9,285,000 | 9,285,000 |
| Net Profit | 7,367,000 | 7,367,000 | 7,367,000 | 7,367,000 |
| Inventory | 18,647,000 | 18,647,000 | 18,647,000 | 18,647,000 |
| Current Assets | 34,246,000 | 34,246,000 | 34,246,000 | 34,246,000 |
| Total Assets | 69,831,000 | 69,831,000 | 69,831,000 | 69,831,000 |
| Current Liabilities | 35,464,000 | 35,464,000 | 35,464,000 | 35,464,000 |
| Liabilities | 46,209,000 | 46,209,000 | 46,209,000 | 46,209,000 |
| Total SE | 23,622,000 | 23,622,000 | 23,622,000 | 23,622,000 |
| Total L&SE | 69,831,000 | 69,831,000 | 69,831,000 | 69,831,000 |

**Verdict: No changes needed.**

---

### FY2025 (reportDate: 2025-08-31) — NEW YEAR

| Field | SEC | Yahoo | Dolt | Recommended |
|-------|-----|-------|------|-------------|
| Net Revenue | 275,235,000 | 275,235,000 | — | **275,235,000** |
| Cost of Goods | 239,886,000 | 239,886,000 | — | **239,886,000** |
| Gross Margin | 35,349,000 | 35,349,000 | — | **35,349,000** |
| SGA | 24,966,000 | 24,966,000 | — | **24,966,000** |
| Operating Profit | 10,383,000 | 10,383,000 | — | **10,383,000** |
| Net Profit | 8,099,000 | 8,099,000 | — | **8,099,000** |
| Inventory | 18,116,000 | 18,116,000 | — | **18,116,000** |
| Current Assets | 38,380,000 | 38,380,000 | — | **38,380,000** |
| Total Assets | 77,099,000 | 77,099,000 | — | **77,099,000** |
| Current Liabilities | 37,108,000 | 37,108,000 | — | **37,108,000** |
| Liabilities | 47,935,000 | 47,935,000 | — | **47,935,000** |
| Total SE | 29,164,000 | 29,164,000 | — | **29,164,000** |
| Total L&SE | 77,099,000 | 77,099,000 | — | **77,099,000** |

**Verdict: SEC and Yahoo agree perfectly. New row ready for insert.**

---

## Reconciled Recommendations Summary

| Year | Action | Key Changes |
|------|--------|-------------|
| 2018 | No change | All fields correct |
| 2019 | **MUST CORRECT [ERROR]** | Replace all 7 balance sheet fields with SEC values |
| 2020 | Update SGA [WARNING] | 16,332,000 → **16,387,000** (FY2022 restatement) |
| 2021 | Update SGA [WARNING] | 18,461,000 → **18,537,000** (FY2022 restatement) |
| 2022 | No change | All fields correct |
| 2023 | No change | All fields correct |
| 2024 | No change | All fields correct |
| 2025 | **Insert new row** | All fields new |

---

## Readiness Signal

**Analysis complete.** Run `/insert-financials COST 2019`, `/insert-financials COST 2020`, `/insert-financials COST 2021`, and `/insert-financials COST 2025` to write these values to the database.

**Unresolved flags before inserting:**

1. **[ERROR] FY2019 balance sheet** — 7 fields carry FY2018 values; correct values verified from FY2019 10-K (balance sheet dated 2019-09-01).
2. **[WARNING] FY2020 SGA** — Current Dolt = 16,332,000; recommended = 16,387,000 (preopening reclassified per FY2022 restatement). Confirm before insert.
3. **[WARNING] FY2021 SGA** — Current Dolt = 18,461,000; recommended = 18,537,000 (preopening reclassified per FY2022/FY2023 restatement). Confirm before insert.
4. FY2018, FY2022, FY2023, FY2024 — No changes needed; no insert required.
