# અક્ષર Akshar Boy

A Game Boy–style web game for learning the Gujarati alphabet.

**▶ Play: https://parmsam.github.io/akshar-boy/**

## Modes

- **LEARN** — browse the letter chart; each card shows the romanization, a pronunciation hint and an example word (ક → કમળ *kamal*, lotus).
- **QUIZ** — see a letter, pick its sound. 10 questions, 3 lives, streak bonus.
- **FIND** — hear/read a sound, pick the letter.
- **BLITZ** — 45 seconds, as many as you can.

Practice all letters, vowels only, or consonants only. Letters you miss come back more often; a letter counts as mastered at 3+ correct with ≥75% accuracy. Progress and high scores are saved in your browser's localStorage.

## Controls

| Key | Button | Action |
|---|---|---|
| Arrow keys | D-pad | move |
| `X` / `Space` | A | choose · say the letter |
| `Z` / `Esc` | B | back |
| `Enter` | START | start / confirm |
| `Shift` | SELECT | say the example word · replay sound |

On touch screens, tap the on-screen buttons or the answers directly.

## The letter set

The game uses the 49 letters of the traditional school chart: 13 vowels (including the marked forms અં and અઃ), 34 consonants, and the conjuncts ક્ષ and જ્ઞ. There is no single official count — sources range from 45 to 50 depending on whether they include અં/અઃ, ઍ/ઑ and conjuncts — but all agree on 34 consonants.

Capital letters in the romanization (Ta, Da, Na, La, Sha) mark retroflex sounds, made with the tongue curled back.

## Pronunciation audio

Uses the browser's Web Speech API: a Gujarati voice if one is installed, otherwise a Hindi voice (the scripts map letter-for-letter), otherwise the romanization read by an English voice. For authentic audio, install a Gujarati text-to-speech voice in your OS settings.

## Development

It's a single self-contained `index.html` — no build step. Open it in a browser, or serve locally:

```sh
python3 -m http.server
```

Fonts (Press Start 2P, VT323, Noto Sans Gujarati) load from Google Fonts.
