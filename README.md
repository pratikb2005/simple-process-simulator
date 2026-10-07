# Simple Process Simulator

A self-contained, browser-based steady-state process simulator (in the spirit of UniSim/ProMax, much simpler).
Everything runs client-side in a single `index.html` — no server, no build step.

**Live app:** enable GitHub Pages for this repo (Settings → Pages → Deploy from branch → `main` / root) and open `https://<your-username>.github.io/<repo-name>/`.

## Features
- Drag-and-drop flowsheet: material streams, valve, heater, cooler, two-stream heat exchanger (zoned heat curve, UA, minimum approach), 2- and 3-phase separators, mixer, splitter, pump, compressor, expander, shortcut distillation column (Fenske–Underwood–Gilliland–Kirkbride).
- Components: N2, CO2, H2S, C1–C10 (incl. iC4, iC5), H2O.
- Peng–Robinson (1978) EOS, Stryjek–Vera α for water, kij table, Michelsen stability + successive substitution flash, free-water phase model, PH/PS/VF flashes, Peneloux-type volume shift.
- Stream workbook, compositions, equipment/energy summary, phase envelope, SI / Field units.
- Recycle handling by tear stream + direct substitution.
- Flowsheets autosave in the browser; Export/Import as JSON.

## Limits
No hydrates, ice, solids or reactions. Column is a shortcut model, not tray-by-tray.
