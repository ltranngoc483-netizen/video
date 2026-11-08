# TECH UNMASKED — Bút ghi âm 150K, bản ghép lời đọc

24.633 seconds · 739 frames · 1080×1920 · H.264/AAC · 30fps. Uses user-supplied `1107 (1)(1).MP3` (24.607s). Four individually editable scenes, thirteen camera/shot beats, moving magnifier, cyan/red audio illustration, stop-motion transforms and paper wipes.

## Changes from the picture/SFX version

Voice pitch, speed and words are preserved; no new voice was synthesized or cloned. Music/SFX are reduced to12% in the mix, with effects retimed to the new visual events. The MP4 ends with the recording rather than retaining a silent30-second tail. Main scene boundaries: frame0/148/403/622/739 (about0/4.93/13.43/20.73/24.63seconds). The CTA runs from the actual related-video invitation at20.72s to the end, around3.9seconds rather than5seconds in the provisional silent edit.

18 caption cues were aligned to onset timestamps recognized from the actual MP3 with local Vietnamese ASR; micro/lọc ồn/cọ áo and punctuation were corrected against the supplied script. Words highlight cyan during speech. Cue times are approximate ASR/editorial boundaries, not a claim of sample-accurate forced alignment. Source transcript and alignment script are included.

The source MP3 is included unmodified as `public/narration.mp3`. No ElevenLabs tool/credential was available or needed for this user-supplied recording. `public/sound-design.wav` is only original sound design; audio source is separate in Studio.

## Illustration and evidence

Device images and internals are generic AI papercraft teaching models, not an authenticated teardown or PCB of a real tested unit. Price150,000đ and48-hour/through-wall questions are the supplied advertising claims being questioned, not measurements. No exact capacity, measured recording distance, verified filtering or claim about all cheap pens is asserted. Cloth noises are illustrative SFX, not recordings of device testing. Cyan represents sound, not a real scanning beam. The brief supplies a general PMC lead without exact article URL/DOI; no paper or device report was independently verified here.

Attach an actual matching long-form teardown in YouTube Studio's Related Video field when it exists. The arrow itself is not clickable. This package does not include a10-minute pen teardown.

## Editing

Install dependencies with `npm install` on a new system, then `npm run dev` (port3017). Main composition `Recorder150KVoice`; standalone scenes `PenHook`, `PenTeardown`, `NoiseStorm`, `PenFunnel`. `src/RecorderVideo.tsx` contains independent scene nodes. `src/captions.json` contains actual MP3 timings; `src/timing.json` records scene/camera timing. Separate still registrations remain available for image editing.

`node scripts/render.cjs --review-only` exports review frames. Without the flag it renders picture; then `python scripts/finalize.py` adds original voice and the reduced mix. `python scripts/validate-voice.py` checks format, length, full decode, captions and source-audio correlation. Renderer Chromium executable is workspace-specific: replace it with your local Chrome. Audio/ASR utilities require numpy/soundfile/sherpa-onnx; voice and sound WAVs are already supplied so no ASR model is needed to edit/render. `scripts/transcribe.py` uses an external local Vietnamese ASR-model path and is only for regenerating the transcript.

Fonts are DejaVu, included with license in `public/licenses`. Art from the preceding approved paper-diorama version is preserved. The unchanged picture/SFX-only release remains available separately.
