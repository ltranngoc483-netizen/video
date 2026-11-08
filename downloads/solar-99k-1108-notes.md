# TECH UNMASKED — Solar99K, bản ghép1108.MP3

24.133seconds · 724frames · 1080×1920 · H.264/AAC · 30fps. Uses the supplied1108.MP3 recording(24.111s), with its original tempo, pitch and wording preserved. No replacement voice was generated or cloned, and no ElevenLabs service was used. The original picture/SFX-only release remains separate.

## Sync changes

Scene boundaries at frames0/130/336/600/724, approximately0/4.33/11.20/20.00/24.13seconds. Paper transitions, camera cuts, energy/heat headings and original SFX now follow the recording's speech onsets. No silent tail is retained to extend the film to30s. CTA runs20–24.13s, from the real spoken invitation through the end.

Fifteen captions were aligned to ASR word onsets from the actual MP3, then spelling and units corrected against the supplied script. Spoken quantities are displayed as50.000mAh,3,7V and185Wh for readability; their active highlight spans the spoken quantity. These are approximate ASR/editorial phrase boundaries, not a claim of sample-accurate forced alignment. Main captions sit below the scene title, energy-scene captions below the formula, and CTA captions above the arrow. The SRT is UTF-8 with BOM. Music/SFX is mixed at12% behind the unchanged voice.

The source MP3 is included unmodified as public/narration.mp3, with SHA-256 recorded in validation. Captions, timings, source transcript and alignment script are included. No ASR model is required to edit/render because timing data is already supplied.

## Illustration and calculation

Hardware and ballast remain a papercraft teaching reconstruction, not a real teardown of the99K item. Sand, gray weights and small cells do not establish anything about a particular product, seller or every cheap bank. The large battery block is an abstract energy icon, not a specified cell shape, chemistry or scale. No product capacity, solar wattage, measured charging time or thermal threshold has been tested here.

50,000mAh =50Ah. At nominal3.7V,50Ah ×3.7V =185Wh **if the advertised capacity is true**. This does not guarantee185Wh at USB output, where conversion/losses matter. The condition remains onscreen. Heat warning is conditional, not an inevitable fire/explosion claim. Camping fire in the opening is a separate campsite prop.

The brief supplied an incomplete unwire.hk/+4 citation lead, not exact articles or independent measurements. No external article/product measurement was independently verified in this production. Sound effects are original illustrative synthesis, not real test audio.

Related Video requires an actual matching long film published and attached in YouTube Studio; the arrow itself is not clickable, and this package does not include a10-minute solar teardown.

## Editing

Install dependencies with npm install, then npm run dev(port3021). Full composition Solar99KVoice; individual SolarOffer, BallastReconstruction, EnergyMath, SolarFunnel scenes retain independent registrations. Main timeline has explicit authored scene nodes.

node scripts/render.cjs --review-only exports review frames. --render-only renders picture; then python scripts/finalize.py adds original MP3 and reduced SFX. python scripts/validate-voice.py checks metadata, full decode, speech windows, source hash and audio correlation. Replace the workspace-specific Chromium executable path with your local Chrome. Python audio scripts need numpy/soundfile. Regenerating ASR needs sherpa-onnx and the external local Vietnamese model path in scripts/transcribe.py; it is unnecessary for ordinary rendering. WAVs and all photographic/composited props are supplied. DejaVu font license is in public/licenses.
