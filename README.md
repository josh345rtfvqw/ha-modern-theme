# Modern

A clean, modern theme for Home Assistant. Flat cards with thin borders instead of drop shadows, rounder corners, a neutral grey base and a single blue accent. Light and dark modes are both included and follow your device setting.

## Install with HACS

1. In HACS, open the menu (three dots, top right) and choose **Custom repositories**.
2. Add `https://github.com/josh345rtfvqw/ha-modern-theme` with the type **Theme**.
3. Find **Modern** in HACS and download it.
4. Make sure themes are enabled in `configuration.yaml`:

   ```yaml
   frontend:
     themes: !include_dir_merge_named themes
   ```

5. Restart Home Assistant, or run the `frontend.reload_themes` action if the frontend block was already there.
6. Pick **modern** under your Profile > Theme.

## Colours

Pick the accent colour by choosing the matching theme under Profile > Theme:

| Theme | Accent |
| --- | --- |
| `modern` | Blue |
| `modern-teal` | Teal |
| `modern-green` | Green |
| `modern-purple` | Purple |
| `modern-orange` | Orange |
| `modern-pink` | Pink |

Every variant has light and dark modes.

## Updating

When a new release is published, HACS will show an update. Download it, then run `frontend.reload_themes`.

## Manual install

Copy `themes/modern.yaml` into `/config/themes/` and follow steps 4 to 6 above.
