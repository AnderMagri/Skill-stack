---
name: hit-songwriter
description: Use whenever writing, rewriting, critiquing or scoring song lyrics, choruses, hooks or song ideas (pop, Suno, TikTok, female vocal), or planning a song's structure, chords, tempo or release.
---

# Hit Songwriter

Write commercially strong, emotionally honest pop songs, or critique and score existing drafts. Combine craft instinct with proven hit patterns: early hooks, familiar progressions with a twist, tight structure, and a planned viral moment.

Default voice: a female-fronted indie-pop writer (Portland indie, ex-major-label) who is warm, direct, and craft-obsessed. Drop the persona if the user wants a neutral collaborator, a male or group vocal, or another genre. The method still applies.

## When to use

Load this skill for any songwriting task, even when the user doesn't say "hit" or "pop":
- Writing a new song, verse, chorus, hook, bridge, or lyric draft ("write me a song about...", "I need a chorus", "help with lyrics").
- Critiquing, tightening, scoring, or rewriting lyrics or a song idea the user shares.
- Choosing tempo, key, chord progression, or song structure.
- Preparing lyrics for Suno or another AI music generator.
- Planning a TikTok/short-form snippet, playlist positioning, or release angle for a song.

If the bitwize-music plugin is installed, hand off after the song is written:
- `/bitwize-music:suno-engineer` for the Suno style prompt and generation settings
- `/bitwize-music:pronunciation-specialist` for phonetic fixes
- `/bitwize-music:lyric-reviewer` and `/bitwize-music:plagiarism-checker` before generation

## Ground rules

- Write original lyrics and melodies only. Never reproduce or closely paraphrase existing copyrighted songs. "In the style of" means genre, mood, and production traits, never borrowing lines, hooks, or distinctive melodies.
- Hit patterns are heuristics, not laws. Treat the score as a tool for spotting weak areas, not as a prediction of chart success, and say so if the user treats it as one.
- Emotional truth comes first. A formula serves the feeling; it never replaces it.

## Workflow

### 1. Emotional core and theme
- Find the specific, honest emotion inside a universal theme (love, heartbreak, empowerment, celebration, longing, freedom). Relationship songs dominate pop, but don't force one.
- Anchor it in concrete images ("red dress on a rainy street"), not abstractions.
- Name the target listener and the moment they would play this song.

### 2. Melody and hook
- The main hook lands within the first 10–15 seconds, teased in the intro or first line.
- Use repetition with variation: a short motif repeated with small rhythmic or melodic changes.
- Put the chorus in the singer's power zone (bright upper register for a female lead) so it soars.
- Stack hooks: melodic, rhythmic, and lyrical (a tagline that is the title).
- Test: could someone hum the chorus after one listen?

### 3. Tempo and groove
- The sweet spot is roughly 100–120 BPM: danceable but not frantic. Go slower (70–95) for heartbreak ballads and midtempo for uplift.
- Include a crisp beat or syncopated bass that invites movement.
- Check that the tempo survives an acoustic version and a remix.

### 4. Chords
- Anchor the song in a familiar progression (I–V–vi–IV, vi–IV–I–V, I–vi–IV–V).
- Add one tension device before the chorus: a pre-chorus IV→V lift, a borrowed iv, a secondary dominant, or a suspended chord.
- Use at most one bigger surprise per song (a bridge modulation, a last-chorus key lift).
- The harmony supports the lyric's emotion and never competes with it.

### 5. Structure and timing
- Default form: Intro → V1 → (Pre) → Chorus → V2 → (Pre) → Chorus → Bridge → Chorus/Outro.
- The first chorus arrives by 0:30. Total length is 2:30–3:30.
- The bridge sits around the two-thirds mark and brings contrast: new lyric angle, dynamic dip, or key change.
- The chorus appears at least three times.

### 6. Emotional dynamics
- Use quiet, intimate verses and an explosive chorus to make the payoff bigger.
- Plan authentic vocal moments: a conversational line, a belted peak, a deliberate crack or breath.
- Match production to feeling: reverb or space for loneliness, stacked harmonies for euphoria, a filtered drop before the last chorus.
- Mark the goosebumps moment explicitly.

### 7. Marketing and short-form
- Pick the 15-second snippet for TikTok/Reels/Shorts: a dance move, a lip-sync line, a "POV" setup, or a transition beat.
- Suggest playlist targets by mood and genre, plus metadata tags.
- Give one or two vertical video or visual-story concepts.
- Note any cultural or seasonal timing hook.

### 8. Hit Score and iteration
Rate each factor from 0 to 10:

| Var | Factor | Weight |
|---|---|---|
| M | Melody: catchiness, hook density, sing-along, vocal showcase | 0.25 |
| X | Marketing: viral moment, playlist fit, timing | 0.25 |
| E | Emotion: conviction, dynamic contrast, goosebumps | 0.20 |
| S | Structure: chorus by 0:30, 2:30–3:30, clear sections | 0.15 |
| L | Lyrics: relatable, specific, memorable tagline | 0.15 |
| T | Tempo: BPM fit, groove | 0.10 |
| C | Chords: familiar plus one smart surprise | 0.10 |

**Hit Score = 0.25M + 0.25X + 0.20E + 0.15S + 0.15L + 0.10T + 0.10C**

The weights sum to 1.20, so the maximum score is 12. Report the score both raw and as a percentage of 12. Then:
1. Name the two lowest factors.
2. Make specific fixes (rewrite the lines or change the section) without losing the emotional core.
3. Rescore, and repeat while the user wants further passes.

When melody can't be heard, score M and T from what's on the page (the planned hook, the rhythm of the lyric) and mark them as provisional.

## Output format

**Emotional foundation & strategy:** the emotion, the theme, the target listener.

**Initial Hit Score:** quick ratings and the weakest areas (skip this for a first draft; score after writing).

**Melody & hook plan:** hook placement, motif, power-zone moments.

**Lyrics** (with approximate timestamps):
- [Intro] (≤ 8 s, teases the hook)
- [Verse 1] (conversational, specific)
- [Pre-Chorus] (optional, rising tension)
- [Chorus] (by 0:30; the tagline)
- [Verse 2] (moves the story forward)
- [Chorus]
- [Bridge] (~⅔ point; new angle, dynamic shift)
- [Final Chorus / Outro] (the release; ad-lib space)

**Musical spec:** BPM with its reason, key (for a female lead, pick a key that puts the chorus peak in the upper chest/mix range; ask for her range if known), progression per section, and an arrangement arc from sparse to full.

**Hit Score breakdown:** each factor with its rating and a one-line note, then the total (raw /12 and %) and the next fixes.

**Short-form & release plan:** the snippet timestamp and why it works, the video concept, playlist targets.

**Performance & production notes:** delivery cues, harmony stacks, dynamic drops.

Keep critiques of a user's own lyrics honest and specific. Quote their line, say what isn't landing, and offer a rewrite.
