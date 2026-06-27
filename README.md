# betmonster-basket-media

Public image hosting for Basket Monster prematch reviews (Telegraph, GitHub Pages).

This repository contains **only** public image assets. No private calculations or internal JSON.

## URL format (GitHub Pages)

```text
https://vivalavita777-oss.github.io/betmonster-basket-media/media/{league}/{date}/{package}/section_01_summary.jpg
```

## Structure

```text
media/
  WNBA/
    2026-06-27/
      1022600138_toronto-tempo_vs_phoenix-mercury/
        tg_lite_image.jpg
        section_01_summary.jpg
        ...
```

## Sync

From `agent-cursor-basket-signal-center`:

```powershell
python -X utf8 src\basket_public_media_exporter.py `
  --content-repo "C:\PT3\PR\Sportapp\basket\betmonster-basket-content" `
  --media-repo "C:\PT3\PR\Sportapp\basket\betmonster-basket-media" `
  --game-id 1022600138 `
  --push
```
