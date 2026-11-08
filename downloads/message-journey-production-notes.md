# THE INVISIBLE WORLD — What Really Happens When You Send a Message?

30seconds · 1080×1920 · 9:16 · H.264/AAC · 30fps. Four individually registered scenes, fourteen review/shot beats: Send → Encryption → Physical network → Received/CTA. Photographic handcrafted torn cardboard, navy/cyan/cream, masking tape and brass pins; independently animated data cubes, physical locked envelope, rotating paper gears, optical pulses and delivery cue, consistent torn-paper wipes.

## Narration and subtitles

Uses the previously user-approved local US male draft style, Kokoro am_michael, **not ElevenLabs Marcus**. No ElevenLabs tool or credential was available; no voice cloning or identity imitation is used. Narration follows the supplied English wording with natural punctuation. Individual phrases are generated, lightly trimmed, normalised and pitch-preserving tempo-adjusted for the fixed5/10/10/5s scene windows. The encryption section includes a short visual lock/qualifier beat after narration while the scene continues to15s.

Twelve SRT cues use measured generated phrase durations and a0.1s scene lead-in, not arbitrary captions or word-level forced alignment. MP4 has visible English captions. The separate scene PNGs have short English titles and technical qualifiers but **no full narration captions** baked in, to support CapCut editing. English cue timings and source voice phrase JSON are included.

Original sound design combines a quiet synth bed, paper snaps/wipes, haptic clicks, mechanical locks, optical pulse tones and delivery chime. No licensed stock music or external voice recordings are used. Original effect/bed track is mixed at22% behind narration.

## Technical scope

Encryption is conditional: the messaging service must support properly implemented end-to-end encryption. The locked envelope/vault/gears are a metaphor for processing at the sender's phone; servers are not depicted decrypting plaintext. Contents are protected from intermediaries in this model; no promise of universally hidden metadata, secure compromised endpoints, all backups or SMS encryption is made.

The network scene is an illustrative journey, not a measured route or packet capture. Some routes cross submarine fibers and some do not. No guaranteed ocean crossing,60ms latency or60,000-mile distance is asserted. Information is represented as cyan cubes and pulses, not actual luminous cubes inside a handset or a physical envelope travelling inside glass. The optical drawing simplifies engineering details and relative scale.

A delivery indication is illustrative, not a read receipt or a promise of instantaneous delivery. Actual protocols, acknowledgements, offline queueing, device decryption/reassembly and retry behaviour vary by service and are simplified in this30s overview.

The supplied brief references Signal Support and a generic Learning Center lead without exact article URLs. No new service-specific technical audit, route measurement or external source retrieval was performed for this production. General educational framing follows the supplied technical qualifiers.

## Channel and funnel

The latest technology brief explicitly identifies THE INVISIBLE WORLD, used throughout. The Unsolved Archive is the separate folklore channel from previous tasks. CTA occupies25–30s. Before posting, attach an actual matching long documentary in YouTube Studio's Related Video field. The arrow is only a visual cue and is not clickable on its own; no long messaging documentary is included here.

## Editing and export

On a new system, install dependencies with `npm install` and run `npm run dev` (Studio port3019). Full composition `MessageJourney`; standalone scenes `BinarySend`, `CryptoLock`, `FiberFlight`, `ReceiveFunnel`; four Still registrations `Scene01`–`Scene04`. Main timeline has separate authored JSX nodes for the four scenes. Transform motion is sampled at15poses/sec for physical stop-motion cadence while export stays30fps.

`node scripts/render.cjs --review-only` exports review frames and four1080×1920PNG assets. `--render-only` renders picture without repeating those exports. Replace the workspace-specific Chromium path with your own Chrome. `python scripts/audio.py` combines supplied voice clips, synthesizes sound design and exports SRT; `python scripts/finalize.py` muxes audio/video; `python scripts/validate.py` verifies the final output. Audio scripts require numpy/soundfile. All generated WAVs are included, so regenerating voice is unnecessary. TTS regeneration requires Kokoro ONNX and voices at external local paths in scripts/voice.py.

Fonts are DejaVu, included with license. Kokoro-82M/ONNX is distributed under Apache2.0; runtime kokoro-onnx; model sources https://huggingface.co/hexgrad/Kokoro-82M and https://github.com/thewh1teagle/kokoro-onnx . No model weights are included. All photos and physical animation props were generated for this project, then combined with procedural paper/data animation.
