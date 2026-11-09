# superstore-in-motion-assets

The backdrop video for the Superstore in Motion Tableau dashboard, served to a Web Page object (1040 x 680 cover, a 30 s loop, h264 + vp9 behind a poster). Source: the lead's superstore_in_motion_30s_1456.mp4 (1456 x 1084, 60 fps, 30.0 s; swapped in 2026-11-06 11:3x — the 8.25-s background_only_full_2912.mp4 was the first cut), transcoded by ffmpeg scale=increase + crop.

- backdrop.html — the cover page the Web Page object points at
- backdrop-1040x680.{mp4,webm}, backdrop-1040x680-poster.jpg

## 2026-11-06 16:5x — v2: the full frame shown
The lead: the video's own titles were cut at full size (scale=increase + crop lost the top and bottom rows). v2 contains the whole 1456 x 1084 frame at 913 x 680 over a blurred cover fill (ffmpeg: scale=increase,crop,gblur sigma 28 as [bg]; scale=-2:680 as [fg]; overlay centred). mp4 h264 crf 24 · webm vp9 crf 34 · poster = frame 0. Sources carry ?v=2 to pass the caches.

## 2026-11-09 — Phase 2, card 1: `sub-category/`
`sub-category/backdrop.html` + `backdrop-1040x680.{mp4,webm}` + poster — the design's `flower_mint.mp4` (1456 x 1084, 30 fps, 30.0 s) at 1040 x 680 COVER (the html's `object-fit: cover`; ffmpeg scale=increase,crop; x264 crf 23 · vp9 crf 34). One folder per Phase 2 card.
