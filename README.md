---

# my-jellyfin-css.css:

My current custom CSS, which has gradually evolved from Jellyfin vanilla over time, tested and used on Jellyfin Web with Windows 11, Jellyfin 10.10.7, and Chrome.

---

# imdb-top250.css: IMDb Top 250 Icon Mod for Jellyfin

Custom CSS for Jellyfin Web.
Tested on Windows 11, Jellyfin 10.10.7, Chrome.

## Description
This mod replaces the default IMDb external link icon in Jellyfin with a special IMDb Top 250 icon
for movies that are part of the IMDb Top 250 list.

Detection is done purely via CSS by matching hardcoded IMDb IDs.
If a movie’s IMDb ID is part of the Top 250 list, the custom icon is shown instead of the normal IMDb logo.

IMPORTANT: The IMDb Top 250 list is hardcoded. It does not update automatically when IMDb changes rankings.

## Dependency (Required)
This mod is based on and depends on the custom CSS project by Druidblack and will not work without it:
https://github.com/Druidblack/jellyfin-icon-metadata

## Installation
The following CSS (Druidblack Jellyfin Icon Metadata) must be imported before this mod:
```css
@import url("https://cdn.jsdelivr.net/gh/Druidblack/jellyfin-icon-metadata@main/public-icon.css");
```

This mod, the IMDb Top 250 Icon Mod, must be imported afterwards:
```css
@import url("https://cdn.jsdelivr.net/gh/chrissix666/Jellyfin-CSS-Mods@main/imdb-top250.css");
```

Place these imports in Jellyfin:
Dashboard → General → Custom CSS

## What this mod does
- Detects movies that are part of the IMDb Top 250
- Replaces the standard IMDb icon with a custom Top 250 icon
- CSS-only (no plugins, no JavaScript)

## Notes
- IMDb Top 250 detection is based on hardcoded IMDb IDs
- The list reflects the Top 250 at the time of creation
- Updates require manual changes to the CSS file

## Credits
Base icon system by Druidblack:
https://github.com/Druidblack/jellyfin-icon-metadata

## License
MIT / custom Jellyfin modifications.
IMDb logos and branding belong to their respective owners.

---
