# Deckscope

A single-file, in-browser audio analyzer for electronic music. Open `index.html` in a browser, then drop in a track (WAV, AIFF, MP3, AAC/M4A, FLAC, OGG). Nothing is uploaded.

What it measures:

- **Tempo**: BPM from a spectral-flux onset curve and autocorrelation with a club-tempo prior. The beat grid is refined across the whole track and locked to the kick using low-band onsets.
- **Key**: chromagram of tonal spectral peaks matched against Krumhansl–Kessler profiles. It shows the Camelot code and harmonically compatible keys.
- **Loudness**: ITU-R BS.1770 integrated LUFS, short-term max, loudness range, and an estimated 4× interpolated true peak.
- **Frequency balance**: energy share across sub, bass, mids and air, plus a track-average spectrum and a live analyzer during playback.
- **Stereo**: phase correlation (full band and below 120 Hz) and a club mono check.
- **Arrangement**: intro, drop, breakdown, build and outro, estimated from per-bar band energy. The overview waveform is colored by band (lows, mids, highs).
- **Mixdown & mastering check**: a 0–100 readiness score with pass/check/fix items and advice. *Mixdown* mode checks a premaster: −6 to −3 dBFS headroom, no master-bus limiting, and dynamics left for mastering. *Master* mode checks loudness and true peak against Club (−8 LUFS), Spotify/YouTube (−14) or Apple Music (−16). Both modes also check clipping, DC offset, mono compatibility, sub-bass phase, width, tonal balance and silence at the start or end. Includes a short-term loudness curve.
- **Tonal balance**: 1/3-octave curve compared with a target range. Targets are approximate genre curves (EDM, techno, house, drum & bass, bass music) or a reference track. Shows Low / Low-mid / High-mid / High meters, a whole-track or drops-only scope, and a live line while playing.
- **Reference track**: load a released track to use as the tonal target, compare loudness, punch and width, and A/B it against your mix at matched loudness (press `B`).

The genre curves are approximations of typical releases, not measured averages; a reference track gives the most reliable comparison.

The page opens with a synthesised 126 BPM A-minor demo so every panel is populated.
