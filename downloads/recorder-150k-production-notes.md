# TECH UNMASKED — Bút ghi âm 150K

30s · 1080×1920 · 9:16 · H.264/AAC · 30fps. Four individually editable scenes and thirteen camera/shot beats. Photographic handcrafted cardboard art, magnifying-glass closeups, camera reframing, cyan voice waves, red friction noise, paper wipes, original synth/SFX, CTA held at 25–30s.

## Audio and SRT
The user chose picture/SFX + SRT, to add a preferred male Vietnamese recording later. There is **no narration**. ElevenLabs tools/credentials were not available, so this is not Marcus or ElevenLabs output. `public/sfx-only.wav` and `public/music-bed.wav` are separate editable stems, and `public/sound-design.wav` is the mix. Sound effects are original synthetic illustrations, **not actual test recordings of a recorder pen**.

`recorder-150k-vi-timing-draft.srt` has 13 editorial cues planned for the 30s scene structure, retaining the supplied Vietnamese narration. It is not an audio transcription and has not been aligned to a voice recording. Retime after importing the intended narration; if it exceeds 30s, shorten the narration or extend the edit rather than claiming exact synchronisation. Full narration is not burned into the picture-only MP4; short headings remain.

## Scope and claims
All devices and internals are generic AI-generated papercraft teaching models. They are not a verified teardown, authentic PCB, or evidence concerning a particular seller. The 150,000đ price and 48-hour/through-wall questions are the claims being questioned in the user's creative brief, not measurements. No numerical battery capacity, measured distance or actual noise-reduction capability is asserted. Friction/mechanical vibration may reduce recording quality; increasing distance usually weakens the direct voice relative to ambient sound. Quality varies with microphone, gain, environment, processing, placement and the particular device. No claim that all cheap recorders are fraudulent.

The brief mentions a general pmc.ncbi.nlm.nih.gov lead but supplies no exact paper URL/DOI or test report. No external paper or specific product has been independently verified in this production. Onscreen qualifiers distinguish illustration from actual tests. Cyan is an audio metaphor, not a physical scanning beam.

Only attach an actual matching long-form teardown in YouTube Studio's Related Video field after it exists. The arrow alone is not clickable, and no long-form pen teardown is included here. The standalone cover PNG is not automatically the Shorts thumbnail.

## Editing and rendering
Install dependencies with `npm install` on a fresh system, then `npm run dev` (Studio port3016). Main composition `Recorder150K`, standalone scenes `PenHook`, `PenTeardown`, `NoiseStorm`, `PenFunnel`, stills `Scene01`–`Scene04`, `Thumbnail`. Source `src/RecorderVideo.tsx` contains independently authored scene nodes.

`scripts/render.cjs --review-only` exports 13 review frames and four1080×1920 composed PNGs. Remove the flag to render picture. The Chromium wrapper path in that script is specific to this workspace: replace it with your local Chrome executable. `python scripts/audio.py` regenerates original 48kHz sound stems and provisional SRT (requires numpy/soundfile). `python scripts/finalize.py` combines picture and sound. `python scripts/validate.py` checks the finished file.

Fonts: DejaVu, local files and license under public/licenses. Art generated for this project, including independent animation layers. All source assets and already-generated WAVs are included in the editable project; no voice model needed.
