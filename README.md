# TVS Ronin — Teardown & Rebuild

A **single-file static documentary** that explains every part of a TVS Ronin 225 — what it is,
why it exists, what it connects to, and how each part supports the next (the one-to-one
support chain) — and then walks through a full teardown and rebuild.

Bilingual: **Tamil + English** (Tamil script for explanations, English for technical terms).

## Run locally

Just open `index.html` in any browser. No build step, no dependencies, works fully offline.

## What's inside

- **Anatomy Map** — interactive SVG motorcycle (side view). Click any part to see its job.
  *Dismantle* and *Rebuild* buttons animate the parts off and back on.
- **One-to-One Support Chain** — six dependency chains (Power, Steering, Stopping, Body, Ground, Start & Spark).
- **Teardown & Rebuild Order** — the safe removal sequence (battery first, frame last).
- **Every Part, One by One** — 16 parts, each with what / why / connects / supports / supported-by,
  plus dismantle, rebuild, tip and common-mistake notes. Each card has a mini diagram with that
  part highlighted, and a "Mark as learned" progress tracker (saved in localStorage).
- **Torque Values**, **Tools**, **Glossary**, **Common Mistakes**, **Pre-ride Safety Checklist**.

## Parts covered

Frame, Engine, Fuel Tank, Front Fork, Rear Monoshock & Swingarm, Handlebar & Grips,
Headlamp & Electricals, Front Wheel, Rear Wheel, Brakes & ABS, Exhaust, Chain & Sprockets,
Clutch, Transmission (Gearbox), Battery & Wiring, Seat.

## Key specifications (TVS Ronin)

| Spec | Value |
| --- | --- |
| Engine | Single cylinder, 4-stroke, 4-valve, SOHC |
| Displacement | 225.9 cc, oil-cooled |
| Max power | 15.01 kW (20.4 PS) @ 7750 rpm |
| Max torque | 19.93 Nm @ 3750 rpm |
| Transmission | 5-speed, Assist & Slipper clutch |
| Brakes | 300 mm front disc / 240 mm rear disc, ABS |
| Tyres | 110/70-17 (front) · 130/70-17 (rear), tubeless |
| Kerb weight | 160 kg |
| Fuel tank | 14 L |
| Seat height | 795 mm |
| Ground clearance | 181 mm |
| Wheelbase | 1357 mm |

Specifications are from TVS Motor's official published figures.

## Hero photo

The hero shows a TVS Ronin side-view photo, loaded from a third-party media gallery URL
(the sandbox used to build this could not download the binary, so it is linked rather than
embedded). A **free-licence illustrative motorcycle photo** (Unsplash) is embedded inline as a
graceful fallback, so the page always shows a real bike photo even offline or if the external
image is blocked. If all external images fail, the caption switches to say the photo is
illustrative.

To use your own photo (recommended — accurate, offline-safe and yours): drop your image next to
`index.html`, point the `<img id="roninImg">` `src` at it, and you can delete the fallback block.

## Tech

Pure HTML + CSS + JavaScript in one file. No frameworks. System fonts only — nothing is
fetched from the network, so it renders identically offline.

## License

MIT
