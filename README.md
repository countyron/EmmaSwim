# Balmoral Swimmer Comparison Tracker

Static GitHub Pages app that tracks and compares Balmoral Beach Club average swim pace per 100 m.

## Add or remove swimmers

Edit `data/config.json`:

```json
{
  "swimmers": [
    "Bennett, Emma",
    "Bennett, Shaun"
  ]
}
```

Use the exact name format shown in Balmoral results, generally `Surname, Firstname`.

## Dashboard modes

- **Single**: view one swimmer's race history.
- **Compare**: tick multiple swimmers and plot them on the same pace chart.
- **Race filter**: show Saturday only, Sunday only, or both.

## Update process

GitHub Actions runs the scraper after Saturday and Sunday races and commits `data/results.json`.
You can also trigger it manually from **Actions → Update Balmoral swim results → Run workflow**.
