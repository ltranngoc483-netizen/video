# The Unsolved Archive — Kuchisake-onna, 11-minute documentary

Complete 40-scene English documentary draft, 660 seconds, 1920×1080, 16:9, 30 fps delivery. Four acts begin at 00:00, 02:30, 05:30 and 08:30. Individual scene lengths have been balanced within each act for even narration pace; the total and chapter boundaries remain unchanged.

## Picture and motion

Seven new photographic paper-diorama environments and two new transparent prop atlases support 92 independently placed paper/card/figure layers. Sharp masked/unmasked portraits and the escorted group share the previously established visual identity. Scenes use moving paper cutouts, physical card entrances, alternating camera crops and torn-paper wipes. Native paper motion is sampled at 12 fps inside the normal 30 fps viewing file.

The editable React timeline contains forty authored Sequence nodes and forty registered scene compositions. Remotion renders the transparent foreground/HUD layers from that source; FFmpeg animates those layers, the camera and transitions at native paper cadence, burns captions, and joins the scene clips. This hybrid renderer avoids requiring a browser to raster every frame of the full eleven-minute film. Studio offers the corresponding editable scene preview. The final MP4 is the authoritative delivery.

## Narration and sound

The narrator is the locally approved US male Kokoro am_michael draft voice, NOT ElevenLabs Marcus. No ElevenLabs call or cloning was used. Foreign names have phonetic reading guidance. Speech is generated in sentence/phrase chunks, with pitch-preserving tempo changes balanced within each act. The 254-cue SRT is phrase aligned to those generated clips; it is not a word-level forced alignment. Original synthesized paper, footstep, bell, mechanical and ambient-bass effects sit beneath speech. Generated narration WAVs are included in the editable project, so model downloads are not required for playback/editing.

## Evidence boundaries

The source is the user's supplied research/script brief. Its named leads include Nippon.com, National Diet Library/Gifu library reference records and folklore archives, but full article URLs/primary newspaper scans were not supplied or independently reviewed in this production. The film attributes newspaper/library references as publication records, not paranormal proof. It does not claim this environment authenticated original police files.

The samurai-wife story is explicitly folklore; onryō and social-anxiety explanations are marked as interpretations. The Himeji imitator passage is a secondary account whose original arrest record is not established here. Newspaper-style pages and period locations are generated reconstructions; no authentic masthead, police seal, invented victim or fabricated quotation is used. The mouth is a cyan seam in cardboard, without realistic injury or blood; children are safely escorted. Escape rules are presented as inconsistent regional fiction, never verified protection.

The title/thumbnail framing uses the 1979 rumor panic rather than promising a verified supernatural 'true origin' or an authenticated police archive. Channel branding is THE UNSOLVED ARCHIVE; the old channel slogan is absent from the finished narration and pictures.

Japan's coastline is derived from Natural Earth geometry in the public datasets/geo-countries repository: https://github.com/datasets/geo-countries. Map threads are illustrative rumor-network lines, not verified sighting locations. DejaVu font license is included in public/licenses. Images are generated illustrations, not archival photographs.

## Rebuilding and editing

1. Install Node dependencies with `npm ci`. `npm run dev` opens Studio on port3015. Main composition: KuchisakeDocumentary. Individual scenes are Scene01–Scene40.
2. `node scripts/export-layers.cjs` exports the foreground/HUD layers and wipe. Set its browser executable to your installed Chrome path when using another computer.
3. Run `python scripts/audio.py` with numpy/soundfile and FFmpeg installed to rebuild the combined audio from the included voices. `scripts/voice.py` is only needed to regenerate voices; it additionally needs Kokoro ONNX and external model files.
4. `python scripts/render-scenes.py` renders forty resumable scene clips. It caches decoded RGBA images under out/raw-cache for speed; allow roughly 2GB of scratch space. It uses two workers and bounds video bitrate so the full download fits below the repository's file limit. Paper cadence is 12 fps, delivery is 30 fps.
5. `python scripts/finalize.py` joins the clips and audio. `python scripts/validate.py` checks full decoding, metadata, all forty speaking sections and subtitle bounds. Thumbnails export through scripts/export-thumbnails.cjs.

The `out` directory, raw cache and node_modules are not part of the editable download. Rebuilding creates them. Local rendering scripts use the execution environment's Chromium wrapper by default; replace that path on another machine. The brief's original scene timestamps are reference guidance; source scenes.json and the supplied screenplay markdown contain the final balanced timing.
