# 🎧 Pitch Lab

Ear-training games. Open it in any browser, on a phone, tablet or computer:

**▶ Play: https://marginalsolutions.github.io/pitch-lab/**

## Games

| Game | What it trains |
|---|---|
| 🕵️ **Note Detective** | *Absolute pitch*: hear a note with no reference and name it. You start with 3 notes (C, G, E) and unlock a new one each time you score 85%+ over 20 answers. A quick "scramble" plays before each note so you can't just compare it to the last one. |
| 📏 **Interval Hunter** | *Relative pitch*: name the distance between two notes. Song hints help you remember each one (e.g. a Perfect 4th is "Here Comes the Bride"). Unlocks up to all 12 intervals, then mixes in descending and played-together intervals. |
| 🎯 **Sharp Ears** | A 30-round higher/lower test that gets harder as you go and measures the smallest pitch difference you can hear, in cents (100 cents = one piano key). |
| 🥁 **Tempo Sense** | Your inner clock. **Guess the BPM**: a beat plays and you set a slider to how fast it is (8 rounds). **Tap the BPM**: you see a tempo like "96 BPM", hear a 4-beat count-in, then tap 8 beats on your own. It scores your speed and your steadiness. |
| 🎙️ **Sing It** *(optional, uses the mic)* | Hear a note, sing it back, and keep the live needle in the green zone. Singing an octave up or down still counts. Choose Deep, Middle or High to fit your voice. |

Each player has their own profile with points, a daily streak and a leaderboard. Progress is saved in the browser on each device, so it doesn't carry over between devices.

## Tips
- Headphones help for the listening games. For **Sing It**, use speakers at a low volume so the mic hears you.
- A few minutes every day works better than one long session.

## Tech
One `index.html` file with no build step. Sound is generated with the Web Audio API, and Sing It detects your pitch in the browser (YIN-style). No audio ever leaves the device.

---

# 💩 Hospital Simulator

*The grossest game in the world*. Retro Atari-style graphics. It works on a PC (keyboard) and on a phone (on-screen joystick + MOP button).

**▶ Play: https://marginalsolutions.github.io/pitch-lab/hospital-simulator/**

### Level 1: Code Brown
You're the new night-shift nurse at St. Grossington's Hospital. All 9 rooms are covered in poop, puke, pee, blood, and (in the Operating Room) guts. Clean them all before the 3:30 timer runs out to unlock Level 2.

- **Create your nurse:** name, city, skin, hair color and style, scrubs color, nurse cap, and a nurse type: *Speedy Sneakers* (faster), *Iron Stomach* (mops faster, never gags) or *Mega Bucket* (holds more).
- **Move:** arrow keys / WASD. **Mop:** hold SPACE on a mess.
- **Bucket:** each mess fills your bucket. When it's full, dump it at a red biohazard bin in the hallway.
- **Watch out:** patients turn green right before they barf or poop on the floor, and stepping in pee or puke makes you slip.
- **Pause:** P. **Mute:** M.

Level 2 is coming soon. Its code is all in `hospital-simulator/index.html`, with no build step.

---

# 🏈 Field Crew

**Set the show:** drag each prop from the sideline onto its glowing spot on the football field. The closer you get, the more beers you win (3 for perfect, 2 for nice, 1 for close).

**Strike it:** after the band plays, drag every prop off the field and down to the sideline in 15 seconds. 1 beer per prop, plus 3 bonus beers if you clear them all. 6 props per show, 27 beers max. Made for a last show.

**▶ Play: https://marginalsolutions.github.io/pitch-lab/field-crew/**

One file, `field-crew/index.html`, with no build step.

---

# 🎼 Clef Hanger

**Snap your sheet music. Change the clef. Switch the instrument.**

**▶ Open: https://marginalsolutions.github.io/pitch-lab/clef-hanger/**

1. **Your music:** take a photo of one page of sheet music, or choose an image, a PDF or a MusicXML file. There's also a built-in sample (Ode to Joy for B♭ clarinet).
2. **What we found:** the clef(s), the key, the time signature and the instrument it's written for. The instrument is read from the label on the page, or guessed from the clef and range. You can correct it.
3. **Convert to:** pick any of about 30 instruments. Clef Hanger rewrites the notes in that instrument's clef and transposition (for example, B♭ clarinet to E♭ alto sax, or treble clef to alto clef for viola). It picks an octave that fits the new instrument's range and marks notes outside that range in red. Then you can **play** it, **download MusicXML** for MuseScore, Finale, Sibelius, Dorico or Noteflight, or **print** it.

**Reading photos and PDFs uses Claude**, so each person enters their own Anthropic API key (from console.anthropic.com). The key stays in that browser, and images go straight from the browser to Anthropic. MusicXML files and the sample work without a key.

One file, `clef-hanger/index.html`, with no build step. Notation and playback use [abcjs](https://www.abcjs.net/).
