# Chinese Vocabulary Tracker (HSK1 & HSK2)

<img width="1200" height="500" alt="image" src="https://github.com/user-attachments/assets/05983d63-0106-4542-82a0-4a83d8f083d1" />


A personal study tracker for ~500 Chinese words from the HSK1 and HSK2 vocabulary lists.

## Structure

| Sheet | Purpose |
|---|---|
| `HSK1`, `HSK2` | Official word lists (word, pinyin, definition), loaded with **Power Query** |
| `Chinese signs` | The two lists combined into one table, with a checkbox column to mark each word as known, Summary counts of known/unknown words per level (`COUNTIF`, `COUNTIFS`) |


## Techniques used
- Power Query (importing and combining tables)
- `COUNTIF` / `COUNTIFS`
- Charts

## How to use
1. Open `Chinese signs`.
2. Tick the **Known signs** checkbox as you learn each word.

