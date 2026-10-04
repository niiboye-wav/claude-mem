# Deckscope

A single-file, in-browser audio analyzer for electronic music. Open `index.html` in a browser, then drop in a track (WAV, AIFF, MP3, AAC/M4A, FLAC, OGG). Nothing is uploaded.

What it measures:

- **Tempo**: BPM from a spectral-flux onset curve and autocorrelation with a club-tempo prior. The beat grid is refined across the whole track and locked to the kick using low-band onsets.
- **Key**: chromagram of tonal spectral peaks matched against Krumhansl–Kessler profiles. It shows the Camelot code and harmonically compatible keys.
- **Loudness**: ITU-R BS.1770 integrated LUFS, short-term max, loudness range, and an estimated 4× interpolated true peak.
- **Frequency balance**: energy share across sub, bass, mids and air, plus a track-average spectrum and a live analyzer during playback.
- **Stereo**: phase correlation (full band and below 120 Hz) and a club mono check.
- **Arrangement**: intro, drop, breakdown, build and outro, estimated from per-bar band energy. The overview waveform is colored by band (lows, mids, highs).

The page opens with a synthesised 126 BPM A-minor demo so every panel is populated.
