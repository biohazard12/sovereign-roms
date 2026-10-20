# Sovereign ROMs

Curated ROM catalog for the **Sovereign** Android toolkit by Sovereign Labs.

The Sovereign app's ROM Hub reads `roms.json` from this repo and downloads ROMs straight in-app (with SHA-256 verification before anything is flashed):

```
https://raw.githubusercontent.com/biohazard12/sovereign-roms/main/roms.json
```

## Rules

- Official images only — no scraping, no random mirrors.
- Every entry must have a real `download_url` and a verified `sha256`. No placeholder entries.
- Devices are added gradually (Google first, more brands over time).

## Format

`roms.json` holds a `devices` array. Each device has `brand`, `codename`, `name`, and a `roms` array with `id`, `version`, `build`, `type` (factory/ota), `download_url`, `sha256`, and `size_gb`.
