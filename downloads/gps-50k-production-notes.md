# TECH UNMASKED — GPS mini 50K

30 seconds, 1080×1920, H.264/AAC, 30 fps. Four editable Remotion scenes with photographic torn-cardboard dioramas. Includes independent lid and SIM cutouts, finder/position pulses, macro shot changes, example LBS displacement, a separately animated collapsing paper tower and split 2G tag, paper transitions and CTA at 25–30 seconds. Transform animation uses a 15-step-per-second stop-motion cadence.

## Audio and captions

The user explicitly selected picture/SFX only, to add their preferred male Vietnamese narration later. NO synthetic narrator was generated or included. The audio contains original synthesized mechanical/paper/radar effects and a quiet original dark-synth bed. The full provisional script is NOT burned into the MP4; the MP4 retains short scene headings, essential labels and qualifiers. The separate SRT has 15 editorial cues planned for the 30-second structure. It is not an audio transcription or a claim of alignment to a real recording. Retime it after importing the intended voice recording.

## Claims and visual scope

This is an illustrative model of some GF-07-style GSM/LBS variants described in the user's brief. It does not identify a real tested unit or imply every cheap tracker lacks GPS. The empty component footprint is a deliberate teaching diagram, not an authenticated PCB layout. The price and 3 km distance are illustrative; LBS accuracy varies with network density and estimation method. The tower's physical collapse is a metaphor for service loss.

The brief asserted a completed nationwide 2G shutdown in September 2026. Official-source access was blocked by the environment's network policy, so that date and assertion are not repeated in the film or provisional voice script. They are replaced with the conditional statement that a 2G-only device loses connectivity when its network stops serving it, subject to device, operator and local coverage. This is not independent confirmation of the current shutdown status in Vietnam.

Attach an actual matching GPS teardown long video in YouTube Studio as Related Video before posting. The illustrated arrow does not itself create a clickable link. A separate PNG is not automatically the Shorts cover.

## Editing

`npm ci` on a fresh checkout; `npm run dev` starts Studio on port 3012. `GPS50K` is the main composition. Individual scenes are also registered. Public assets include original art and clean plates for moving components. `scripts/inspect.cjs` exports review frames and artwork. `scripts/export-assets.cjs` exports the four finished hero frames with labels. Thumbnail is a 1080×1920 Still.

Render `GPS50K` muted to `out/gps-50k-native.mp4`, then run `python scripts/finalize.py` to mux SFX. Inspection scripts use a system-specific Chromium executable path; substitute your own Chrome path outside this environment. `scripts/audio.py` and `scripts/validate.py` require numpy and soundfile. Fonts are DejaVu, license in public/licenses.
