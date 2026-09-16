# CrusadersBeatFlash
An Rhythm Game! , upload any songs it works! (.MP3's Only!) 



CRUSADERS · BeatFlash
https://legendbruh.github.io/CrusadersBeatFlash/

CRUSADERS BeatFlash
is a rhythm/reaction game with three game modes:

🎵 1. BeatFlash

Upload an audio file and the game analyzes the song to detect its beats.

When a beat is detected:

- One of 4 colored pads lights up.
- Tap the correct pad within the reaction window.
- Faster and more accurate taps give more points.
- Consecutive successful hits build your combo.
- Missing or tapping the wrong pad costs a life.

Scoring

- PERFECT: 100 + combo bonus
- GOOD: 50 + combo bonus
- Wrong/Late: lose a life and reset combo

You can customize:

- Lives: 3 to 20
- Difficulty: 2.0s, 1.0s, 0.75s or 0.5s
- Progressive Difficulty: reaction window decreases by 0.1s every 3 seconds
- Beat Sensitivity: controls how aggressively the audio analyzer detects beats
- Audio Calibration: shifts the timing to compensate for device/headphone latency
- Game Speed: 0.5× to 2×

🎯 2. Swipe-io

Instead of following colored pads, a glowing target appears at random positions.

Tap the target before its timer expires.

- Successful hit → points + combo
- Missed target → lose a life
- Higher combo → higher score
- Target lifetime uses the selected difficulty/reaction window

The target continuously respawns, creating a fast reaction-based game.

🏗️ 3. Stack

Inspired by classic stacking games.

A block continuously moves left and right above the tower.

Tap / press Space to drop it.

Your goal is to:

1. Align the moving block with the block below.
2. Drop it.
3. Keep stacking higher.
4. Avoid missing completely.

If the block overlaps only partially, the tower continues but becomes narrower.

A precise alignment gives a PERFECT and preserves the full width.

The game also supports optional music, and detected beats can influence the movement direction.

🎧 Audio System

The game uses the uploaded song directly.

For BeatFlash and optional Stack music, JavaScript:

1. Decodes the audio.
2. Converts it into simplified waveform data.
3. Runs an FFT analysis.
4. Measures changes in frequency energy.
5. Detects peaks.
6. Estimates a BPM.
7. Generates a beat grid.

The game then uses that timing to synchronize gameplay.

📊 End Screen

After the run, CRUSADERS displays:

- Final Score
- Perfect hits
- Good hits
- Misses, or Stack Height
- Best Combo

Then you can PLAY AGAIN.

In short:

«BeatFlash = follow the beat.
Swipe-io = react to the target.
Stack = build the tower.»
