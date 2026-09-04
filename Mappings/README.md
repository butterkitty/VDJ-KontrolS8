# butt3rpuppie — Kontrol S8 Mapping

A custom VirtualDJ controller mapping for the Traktor Kontrol S8, built on top of Atomix Productions' stock `TRAKTORS8` mapper (v850). It keeps everything from the default mapping — pads, FX, browser, EQ, VU meters, etc. — and changes a handful of controls around jog/scratch feel, tempo adjustment, and library scrolling.

## Requirements
- VirtualDJ with support for mapper format v850+ (recent VirtualDJ 2023/8 builds).
- A Traktor Kontrol S8, recognized by VirtualDJ as `TRAKTORS8`.

## Installation
1. Download `Traktor Kontrol S8 - butt3rpuppie.xml`.
2. Copy it into your VirtualDJ `Mappers` folder:
   - macOS: `~/Library/Application Support/VirtualDJ/Mappers/`
   - Windows: `Documents/VirtualDJ/Mappers/`
3. In VirtualDJ, open the controller's mapping settings for the S8 and select **butt3rpuppie** as the active mapper.

## Differences from the default `TRAKTORS8` mapping
Everything not listed here (pads, FX, EQ/gain, crossfader assign, sampler, VU meters, browser sort, deck switch, etc.) is unchanged from Atomix Productions' stock mapping.

| Control | Stock | This mapping |
| --- | --- | --- |
| Jog wheel touch, paused | Scrubs, direction inverted | Scrubs forward at 2x sensitivity, not inverted |
| Shift + jog wheel touch | Nothing | Emulated scratch — your finger drives the track directly, and letting go decays smoothly back to normal speed instead of stopping dead |
| Shift + touch strip, while playing | Jumps play position to the touch point | Emulated scratch (same touch-driven behavior as the jog wheel) instead of jumping position |
| Shift + touch strip, while paused | Jumps play position to the touch point | Unchanged |
| Shift + browse encoder | Scrolls 1 row per detent | Scrolls 4 rows per detent, for fast list navigation |
| Tempo encoder, rotate | Unbound | Nudges pitch ±1.00 BPM per detent, or ±0.05 BPM held with Shift |
| Tempo encoder, push | Unbound | Triggers sync |
| Browse encoder touch + screen option 2/4 buttons | Unbound | While the browse encoder is touched, jumps the browser to the top / bottom of the current list |
| Shift + filter-activate | Stock default action | Cycles the filter's assigned color-FX effect forward/back |

## Credits
Based on Atomix Productions' stock VirtualDJ mapper for the Traktor Kontrol S8 (`TRAKTORS8`, v850).
