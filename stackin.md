# "Stackin Bands" — Phonk Standalone Single

**Title:** Stackin Bands · *triple entendre: hospital wristbands collected (V1 ER motif) / dollar bands stacked (tip-jar singles, subverted trap trope) / sonic bands stacked (the act of producing the song itself)*
**Lineage:** Memphis phonk · **BPM:** 140 (half-time feel ~70) · **Key:** D minor · **DAW:** Ableton 12 (stock plugins only)
**Status:** Lyrics locked · Markup complete (V1 + hook + V2) · Beat spec committed · Production checklist embedded · Release plan: standalone single

---

## 1. Final Verse 1 (16 bars)

```
L1:  Discharge papers in his fist, edges blurred
L2:  Paper bag of clothes, wristband uncut, no word
L3:  Sky hasn't decided, grey blue with a copper burn
L4:  Waits at the curb too long, no place left to return
L5:  No blink, no flinch, mind on full rewind
L6:  Intercom dims behind him, soft and so kind
L7:  Card declined by vending, the hunger refined
L8:  Wristband his only ID, his pockets left behind
L9:  Behind him now the sky is bright blue
L10: Just an irrelevant stranger to me and you
L11: That doesn't mean a stranger don't matter
L12: After all, we could end up in tatters, too
L13: Sometimes it's worth dropping a dime
L14: A quarter, a dollar, or even some time
L15: To help out the next homie in line
L16: Cuz the wristband on the next one might be mine
```

## 2. Hook

```
H1: We could end up in tatters, too
H2: We could end up in tatters, too
H3: Just a stranger 'til the wristband reads you
H4: We could end up in tatters, too
```

---

## 3. Structural Summary (Verse)

| Element | Detail |
|---|---|
| Three-act arc | L1–9 documentary → L10–12 indictment + memento mori → L13–16 prescription with personal stake |
| Wristband motif | L2 uncut → L8 only ID → L16 might be mine → H3 reads you |
| Sky motif | L3 hasn't decided → L9 bright blue (light rises outside as light dims inside) |
| P-alliteration | L1 papers → L2 paper → L8 pockets |
| Pronoun ladder | 3rd-person → me/you → we → homie → mine → you (hook) |
| Internal slip rhymes | fist/wrist · blink/flinch · declined/refined · matter/tatters · quarter/dollar (5 across 16 bars) |
| Domains used | Pure street observation — no personal life domains active |

---

## 4. Beat Spec — Memphis Phonk

### 4.1 Tempo / key / mode
- **140 BPM**, half-time perceived ~70
- **D minor** (alt: A minor)
- Natural minor + tritone (Ab) on lead lines for menace

### 4.2 Drum kit
| Element | Spec |
|---|---|
| Kick | Lo-fi 808 kick, tape-saturated, ~80 Hz body, slight pitch wobble (DJ Screw / Three 6 era) |
| Snare | Saturated trap snare layered with vinyl crackle. 200 Hz body, top-end rolled off above 6 kHz (no modern crack) |
| Clap | OFF or very low — Memphis is snare-driven |
| Closed hat | Lo-fi 1/8 pulse, tape-saturated, narrow stereo, LOW density vs Atlanta |
| **Cowbell** | **Required.** Off-beats. 800 Hz–1.5 kHz body. Three 6 / Tommy Wright signature |
| Vinyl crackle | Constant low-level layer at -30 dB. Source: free vinyl crackle audio loop (Splice, free packs, or Ableton's own Sample > Vinyl folder if available) on dedicated audio track. |

### 4.3 808 design
| Param | Value |
|---|---|
| Tuning | D1 root |
| Glide | 50–100ms (minimal — Memphis is staccato/drone, not slide) |
| Saturation | Stock chain: Saturator (Soft Sine, Drive 4–6 dB) → Redux (Bit 14, Downsample 2) → EQ Eight (sub bump 80 Hz, mud cut 250 Hz, top roll 6 kHz). Full settings in §5.5.5. |
| Pattern | Sparse. Root on 1, root on 3 most bars. Walk every 4–8 bars. NOT melodic 808 lines. |
| Layering | Sub layer (sine, 30–50 Hz) + saturated mid (the character). Skip distortion grit layer. |

### 4.4 Sample / melodic loop
**Source:** Pitched-down minor organ + female vocal chop, vinyl-saturated. 4-bar loop, repeats throughout.
**Why this pick:** "Intercom dims behind him, soft and so kind" — the loop literally IS the intercom fading. Self-mirroring imagery.
**Alternates:** dark string section with tritone hits (more cinematic), or lo-fi piano loop (more sparse).

### 4.5 Arrangement (~2:30, two-verse capacity)
```
Intro (8):    Sample chop + tape hiss + occasional cowbell
Drop 1 (16):  Full kit + 808 + sample. VERSE 1 here.
Break (4):    Drums strip, sample + 808 only
Hook (8):     Full kit returns, slight hat density bump
Drop 2 (16):  VERSE 2
Hook (8):     Final, vocal chop ad-libs over
Outro (4):    Tape stop + filter sweep, sample bleeds out
```

### 4.6 Mix targets
| Element | Target |
|---|---|
| Integrated LUFS | -9 to -7 |
| True peak | -1.0 dBTP |
| Kick | 80 Hz body, lo-fi rolloff above 8 kHz |
| 808 sub | 50 Hz fundamental, saturated mids 200–600 Hz |
| Snare | 200 Hz body, top rolled off above 6 kHz |
| Cowbell | 800 Hz–1.5 kHz, panned slightly off-center |
| Hat | 8 kHz top, narrow stereo |
| Master bus | Stock chain: Saturator (Soft, Drive 2–3 dB) → Glue Compressor (Ratio 2:1, Attack 10ms, Release Auto, GR 1–2 dB) → Limiter (-1.0 dBTP). Full settings in §5.5.6. |

**Vocal-specific:**
- Vocal forward (-3 to -1 dB below loudest sample peak) — documentary verse needs intelligibility
- Light tape sat on vocal bus (matches beat aesthetic)
- L1–L8 dense — *don't* clutter with delay/reverb during these bars
- Hook vocal can have 1/8-dotted delay or short plate to lift the chant

---

## 5. Drum Pattern Detail (16-step grid, 1/16 resolution)

**Swing:** 58% (Memphis canonical 56–60% range — heavy shuffle from DR-110 origins)

### 5.1 Main loop pattern (bars 1–3 of 4-bar phrase)

```
Beat:     1   e   &   a   2   e   &   a   3   e   &   a   4   e   &   a
Kick:     X   .   .   .   .   .   .   .   X   .   .   .   .   .   .   .
Snare:    .   .   .   .   .   .   .   .   X   .   .   .   .   .   .   .
Hat (cl): X   .   X   .   X   .   X   .   X   .   X   .   X   .   X   .
Cowbell:  .   .   X   .   .   .   X   .   .   .   X   .   .   .   X   .
Crackle:  ──────────────── continuous low layer (-30 dB) ──────────────
```

- Kick: 1 and 3 (half-time, Memphis canonical)
- Snare: 3 only (half-time default)
- Hat: 1/8 pulse, every "1, &, 2, &, 3, &, 4, &"
- Cowbell: every off-beat ("and" of each beat) — hypnotic core
- Velocity humanization: ±15% per hit on hat, ±10% on kick/snare

### 5.2 Bar 4 (fill / phrase-end variation)

```
Beat:     1   e   &   a   2   e   &   a   3   e   &   a   4   e   &   a
Kick:     X   .   .   .   .   .   .   .   X   .   .   .   .   .   .   .
Snare:    .   .   .   .   .   .   .   .   X   .   .   .   .   .   .   X
Hat (cl): X   .   X   .   X   .   X   .   X   .   X   .   X   .   X TT  (1/16T roll last 1/16)
Cowbell:  .   .   X   .   .   .   X   .   .   .   X   .   .   .   X   .
```

- Last 16th of bar 4 hat: **1/16T triplet roll** (3 hits in space of 1)
- Velocity ramp on roll: 60% → 80% → 100%
- Last 16th snare hit (pre-flam to bar 1 of next phrase): -6 dB below main snare velocity
- This is the only bar with rolls — keep them rare in Memphis (rolls are an Atlanta thing; Memphis prefers space)

### 5.3 Break section pattern (4 bars after V1)

```
Beat:     1   e   &   a   2   e   &   a   3   e   &   a   4   e   &   a
Kick:     X   .   .   .   .   .   .   .   .   .   .   .   .   .   .   .
Snare:    .   .   .   .   .   .   .   .   .   .   .   .   .   .   .   .
Hat (cl): .   .   .   .   .   .   .   .   .   .   .   .   .   .   .   .
Cowbell:  .   .   X   .   .   .   X   .   .   .   X   .   .   .   X   .
Crackle:  ──────────────── continuous ────────────────
```

- Kick on 1 only (anchor, beat is "stripped" but not silent)
- Cowbell continues — hypnotic carry, signals listener "you're still in the song"
- Sample + 808 only carry harmonic content

### 5.4 Optional perc additions
| Element | When | Pattern |
|---|---|---|
| Horror sample stab | Bar 1 of intro, bar 1 of drop 2 | One-shot, panned, tape-saturated |
| Tape noise sweep | Transition into break | Filter-swept noise, 4-bar fade |
| Vocal-chop ad-libs | Hook bars only | Pitched-down "yeah" / "uh" panned wide |

### 5.5 Ableton 12 implementation

#### 5.5.1 Project architecture

**Track layout:**

| Track # | Type | Contents | Output routing |
|---|---|---|---|
| 1 | MIDI → Drum Rack | **Kit:** kick (pad C1), snare (D1), closed hat (F#1), cowbell (A#1) — each pad loads a Simpler with one sample | → Drum Bus |
| 2 | MIDI → Operator (or Simpler) | **808** — mono mode for any pitch glide between notes. Simpler is simpler; Operator gives FM-synthesis flexibility for designing 808s from scratch | → 808 Bus |
| 3 | Audio | **Vinyl crackle loop** — 8-bar audio clip looped throughout song at -30 dB | → Drum Bus |
| 4 | MIDI → Sampler | **Melodic loop / sample chop** — pitched-down minor organ + female vocal chop | → Master |
| 5 | Audio (or Return) | **Hook vocal ad-libs** — pitched-down "tatters... tatters..." chops, panned wide | → Master |
| 6 | Audio | **Lead vocal** | → Vocal Bus |

**Bus structure:**

```
Drum Bus  ─┐
           ├──→ Master Bus ──→ Limiter → Out
808 Bus   ─┤
Vocal Bus ─┤
Sample    ─┘
```

- **Drum Bus** = combined Drum Rack + crackle. Light glue compression (1–2 dB GR), tape sat (next section)
- **808 Bus** = isolated for parallel saturation chain (next section)
- **Vocal Bus** = light tape sat + delay/plate send for hook only
- **Master Bus** = final glue + saturation + limiter

**Why 808 lives outside the Drum Rack:** mono operation (for glide between notes), independent saturation chain, ability to write melodic 808 patterns later without restructuring. Drum Rack pads can play chromatically but the architecture is clunkier than a dedicated track.

#### 5.5.2 Swing setup (Groove Pool walkthrough)

1. **Open Groove Pool:** wave icon at bottom of main window, or View menu → Show Groove Pool
2. **Find groove:** Browser → Categories → Grooves → MPC60 folder → `MPC60-1-16.agr`
3. **Load:** drag into Groove Pool panel
4. **Apply to drum clip:** select MIDI clip → Clip View → Groove dropdown → set to `MPC60-1-16`
5. **Tune sliders in Groove Pool:**

| Slider | Value | Why |
|---|---|---|
| Base | 1/16 | Matches groove's grid resolution |
| Quantize | 0% (off) | Don't re-quantize after applying groove |
| **Timing** | **60–65%** | ≈ 58% off-beat shuffle (Memphis canonical) |
| **Random** | **3–5%** | Micro-humanization. Higher = sloppy. |
| Velocity | 0% | You'll handle velocity manually (see 5.5.6) |

6. **Optional commit:** right-click clip → Commit Groove (bakes in changes). Don't commit until final bounce — keeps A/B testing possible.

**Tuning if it sounds wrong:**
- Too floppy / late → drop Timing to 55%
- Too straight / robotic → push Timing to 70% (approaches pluggnb shuffle territory)

#### 5.5.3 1/16T roll — Method A (manual MIDI, deterministic)

For studio production / consistent loops:

1. Open the drum clip's MIDI editor (double-click clip)
2. Zoom to the last 16th of bar 4 (the very end of the 4-bar phrase)
3. Switch grid resolution to 1/48 (right-click ruler → Fixed Grid → 1/48 — this is 1/16T)
   - Or: View menu → Adaptive Grid → set to 1/48 narrow zoom
4. Place 3 closed-hat notes within the last 16th, evenly spaced on the 1/48 grid
5. Set velocities: 60, 80, 100 (left-to-right ramp)
6. Verify the 3 hits land *inside* the last 16th — not bleeding into the next bar's downbeat

**Result:** every play is identical. Predictable. Ideal for fixed loops.

#### 5.5.4 1/16T roll — Method B (live with controller)

For performance feel / one-pass tracking / live use:

1. Drum Rack hat pad — confirm it has a **choke group** (Drum Rack → pad menu → Choke Group → set to same group as itself; this prevents overlapping samples from stacking)
2. Set controller to velocity-sensitive mode (Push 3 default; MPK Mini Pro: confirm pads not in Fixed Velocity)
3. Arm the drum track, press record, hit the hat pad 3 times rapidly on the last 16th
4. After recording: quantize to 1/48 grid (Edit menu → Quantize Settings → 1/48 → apply) but **preserve velocity** (uncheck "Velocity Amount" or keep low)
5. Audition; re-record if velocity ramp didn't land naturally

**Result:** micro-variation between bars. More humanization, less control. Better for live sessions or single-pass studio takes.

**When to pick A vs B:** A for production loops (every bar identical). B for live performance or tracking sessions where humanization > consistency.

#### 5.5.5 808 saturation chain (stock — 808 Bus)

In order on the 808 Bus track:

| Position | Plugin | Settings | Function |
|---|---|---|---|
| 1 | **Saturator** | Type: Soft Sine. Drive: 4–6 dB. Output: -2 dB (compensate). DC switch: ON. | Adds harmonic content, gentle compression-like behavior |
| 2 | **Redux** | Bit: 14. Downsample: 2. (Subtle — you should barely hear bitcrush as standalone) | Lo-fi character without obvious artifacting |
| 3 | **EQ Eight** | Low shelf +2 dB at 80 Hz. Bell cut -2 dB at 250 Hz (Q 0.7). High shelf cut -3 dB at 6 kHz. | Sub bump, mud removal, top-end roll-off (Memphis = no top end on 808) |

**Tuning notes:**
- Saturator's Drive setting is taste-dependent. 4 dB = subtle, 6 dB = audible but musical, 8+ dB = aggressive (probably too much for Memphis).
- If 808 starts losing fundamental, reduce Drive and increase EQ low-shelf instead.
- Soft Sine mode is the gentlest curve. Try Analog Clip mode if you want harder character (more aggressive harmonic generation).

#### 5.5.6 Master bus chain (stock — Master)

In order on the Master:

| Position | Plugin | Settings | Function |
|---|---|---|---|
| 1 | **Saturator** | Type: Soft. Drive: 2–3 dB. Output: -1 dB. | Subtle harmonic glue across full mix |
| 2 | **Glue Compressor** | Threshold: set so GR meters 1–2 dB on loudest sections. Ratio: 2:1. Attack: 10ms. Release: Auto. Makeup: by ear (compensate GR). | Mix cohesion — ties drums + 808 + sample + vocals |
| 3 | **Limiter** (or 3rd-party brickwall) | Ceiling: -1.0 dBTP. Gain: push until hitting -8 to -7 LUFS integrated (use Ableton's loudness meter or VU Meter Max for L4M to verify). | Final loudness ceiling |

**Order matters:** saturation BEFORE compression on master. Saturation generates harmonics; compression shapes the result. Reversed = compressor reacts to undistorted signal, saturator slams its output, sounds messy.

**LUFS targeting:** integrated -8 to -7 LUFS (phonk lineage range). Don't mix to streaming targets (-14 LUFS Spotify, -16 Apple) — those are playback normalization, not master targets. Modern phonk releases sit hot (-8 to -7) and accept the streaming turn-down for small-speaker density.

#### 5.5.7 Snare/hat lo-fi processing (Drum Rack pad inserts)

Replaces MPC's AIR Lo-Fi:

| Element | Plugin | Settings |
|---|---|---|
| Snare pad insert | **Redux** | Bit: 12. Downsample: 4–6. Effective sample rate ~16k (matches MPC AIR Lo-Fi target). |
| Closed hat pad insert | **Redux** | Bit: 12. Downsample: 4. Slightly less aggressive than snare. |
| Cowbell pad insert | (none) | Cowbell stays cleaner — it carries rhythmic clarity. Light Saturator if any character needed. |

#### 5.5.8 Velocity workflow — Method A (MIDI editor, deterministic)

For full studio control:

1. Open drum clip MIDI editor
2. Use velocity lane (bottom strip in MIDI editor) to manually set values per hit
3. **Hat pattern velocity humanization:** select all hat notes → MIDI tools → Velocity → Randomize → ±15% (or use the Velocity Random slider in Note Properties)
4. **Roll velocity ramp:** set the 3 roll hits to 60, 80, 100 manually (see 5.5.3)
5. **Snare accents:** main snare on beat 3 = 100. Last-16th pre-flam snare in bar 4 = 70 (-6 dB equivalent).
6. **Kick:** uniform 100, slight randomization ±5% if desired
7. **Cowbell:** ±10% randomization on velocities

#### 5.5.9 Velocity workflow — Method B (live controller)

For natural performance feel:

1. Use velocity-sensitive controller (Push 3, MPK Mini/Mid/Pro, Maschine, etc.)
2. Confirm Fixed Velocity is OFF on the controller
3. Record drum performance live — velocity captured from striking force
4. **After recording:** quantize timing only, preserve velocity
   - Edit → Quantize Settings → set Velocity Amount = 0% → apply
5. **Clean up missed hits in MIDI editor** while keeping captured velocities for hits you keep
6. **Optionally apply MPE if controller supports it** (Push 3 does) — pad pressure can map to filter or pitch in Drum Rack pads for dynamic timbral variation

**Hybrid recommendation:** even though A and B are documented as parallel methods, a one-pass workflow that combines both (live record → MIDI editor cleanup) is often the most efficient route to humanized-but-controlled drums. Use B for capture, A for surgical fixes.

### 5.6 Pocket considerations (drum × vocal)
- L7 is the densest bar (12 syl). The cowbell-on-off-beats pattern can collide with internal pauses there. **Drop cowbell hits during L7 only** — let the bar breathe.
- L9 is short (7 syl) and held. **Strip hat hits during L9** — beat carries kick + 808 + cowbell. The vocal sits in the gap.
- Hook section: bring full hat density back. Hook is hypnotic — drums chant alongside the voice.

---

## 6. Hook Melody — D minor

**Vocal range note:** Sketched in baritone/tenor chest register (D3–D4). Transpose if Vikram's chest range differs; the *shape* is what matters.

### 6.1 Scale context
D natural minor: D · E · F · G · A · Bb · C
Phonk colors: **Bb (b6)** for darkness, **Ab (b5/tritone)** for menace (use sparingly on lead, not vocal melody)

### 6.2 H1 / H2 / H4 melody (identical — chant repetition)

```
Lyric:  We    could    end    up     in     tat-       ters    too
Note:   A3    A3       Bb3    A3     G3     F3 (held)  F3      D3
Scale:  5     5        b6     5      4      b3 (vib)   b3      root
Beats:  1     &        2      &      3      &  (1/4)   .       4
```

- **Shape:** rises one step (5 → b6), falls back, descends to b3, drops to root on "too"
- **"tat-" held with vibrato** — hold ~0.5 beat, slight pulse between F3 and Eb3 (or wide vibrato on F3) for the `~tatters~` markup wobble
- **"too" on D3 (root)** — finality. The line resolves down.
- **Memphis canonical move:** the b6 (Bb3) on "end" is the dark color. That single note carries the mood.

### 6.3 H3 melody (variant — climbs for tension)

```
Lyric:  Just  a    stran-  -ger  'til  the   wrist-  -band  reads  you
Note:   F3    F3   A3      Bb3   A3    G3    A3      C4     Bb3    A3
Scale:  b3    b3   5       b6    5     4     5       b7     b6     5
Beats:  1     &    2       &     3.    e     &.      a.     4      .
```

- **Shape:** starts low (b3), climbs to peak (b7 = C4 on "wristband"), descends to 5
- **C4 (b7) on "-band"** — the highest note in the hook, lands on the verse's central motif word. Wristband peaks.
- **Resolves to A3 (5)** — leaves tension unresolved, so H4's return to the falling pattern (A3 → D3) feels like release
- **"wrist-band" gets the climb** — match the markup's `**wristband**` hard stress with the melodic peak

### 6.4 Phrasing notes
- All four hook lines share the same rhythmic spine (matches the lyric repetition)
- H3 breaks the melodic spine but rejoins on H4 — call/response feel
- Vibrato (`~tatters~`) only on H1, H2, H4 "tat-" syllable — H3 stays clean for contrast
- Vocal-chop ad-libs (pitched-down "tatters... tatters...") panned wide, layered behind H4

### 6.5 Hook backing harmony
- Sample loop already provides D minor harmonic backing
- If wanting a separate harmony layer: simple Dm chord pad (D3 + F3 + A3) sustained under each hook line
- Optional bass voice doubling melody an octave down (D2 instead of D3) for chest weight on H4 only

---

## 7. Performance Markup (full mode)

### 7.1 Annotated script

```
[VERSE 1]
[BEAT enters at bar 9 — verse begins on the beat drop]

⟦chest⟧ [pocket]

L1:  **Discharge** papers in his fist · edges blurred /
L2:  Paper bag of clothes · **wristband** uncut · no word /
L3:  *Sky* hasn't decided · grey blue with a **copper** burn /
L4:  Waits at the curb too long · no place left to return //

L5:  No blink · no flinch · **mind** on full rewind /
L6:  Intercom *dims* behind him · soft and so kind /
L7:  Card **declined** by vending · the hunger **refined** /
L8:  {callback→L2} Wristband his only ID · his pockets left behind //

L9:  *Behind him* now the sky is bright blue↑ //

⟦chest⟧ [pocket] (lens turns — narrator emerges)

L10: [push] *Just* an irrelevant **stranger** to me and you↓ /
L11: That doesn't mean a *stranger* don't matter /
L12: After all · we could end up in **tatters** · too //

⟦talk⟧ [pocket] (prescriptive pivot — conversational register)

L13: Sometimes it's worth dropping a *dime* /
L14: A quarter · a dollar · or even some *time* /
L15: To help out the next homie in line /

⟦chest⟧ ⟦grit⟧ [pocket] (return to weight + personal stake)

L16: {callback→L2,L8} Cuz the **wristband** on the next one might be **mine** //

[BREAK — 4 bars, drums strip, sample + 808 only]

[HOOK]

⟦chest⟧ [half] [pocket]

H1: We could end up in ~tatters~ · too /
H2: We could end up in ~tatters~ · too /
H3: {callback→L16} Just a *stranger* 'til the **wristband** reads you /
H4: We could end up in ~tatters~ · too //

[AD-LIB: tatters... tatters... — whispered echo, panned, tape-saturated]
```

### 7.2 Energy arc

```
L1 ────── L9       documentary plateau (low-mid intensity, chest, pocket-back)
        L9 //      held breath at threshold
L10 ─── L12        indictment peak (slight push on L10, then settle)
L13 ─── L15        conversational valley (talk register, lighter dynamics)
L16                personal-stake peak (chest+grit, heaviest bar)
HOOK               hypnotic plateau (chant register, half-time feel)
```

The intentional dip in L13–15 is what makes L16 land. Without the valley, no peak.

### 7.3 Breath / pocket / texture summary
| Element | Map |
|---|---|
| Pocket | All bars `[pocket]` except L10 `[push]` |
| Texture | `⟦chest⟧` L1–L12, L16, hook · `⟦talk⟧` L13–L15 · `⟦grit⟧` adds to L16 only |
| Pitch | L9 ↑ (slight rise on "blue") · L10 ↓ (drop on "you") · L16 flat (texture carries) |
| Long pauses (//) | L4, L8, L9, L12, L16, H4 |

### 7.4 Callback map
| Motif | Hits | Performance note |
|---|---|---|
| Wristband | L2 → L8 → L16 → H3 | Lean slightly harder on each successive instance |
| Sky | L3 → L9 | L9 echoes "decision" L3 deferred |
| Stranger | L10 → L11 → H3 | Each shifts meaning: dismissal → defense → indictment |

---

## 8. Verse 2 — Final (8-bar phonk coda)

```
V2 L1: I used to be a hacker, coach, guide to others
V2 L2: And that's me whose card was declined, brother
V2 L3: I used to go so hard so long so far
V2 L4: But now my value is tied to a tip jar
V2 L5: I'm behind the counter committing thought crimes
V2 L6: Fighting to build a plan before I'm outta time
V2 L7: Makin' a step that'll cause a faultline
V2 L8: Decades of expertise sold like it's worth a dime
```

### 8.1 Lane / lens

V1 was framed as documentary (third-person observation of a stranger). V2 reveals the documentary was **deferred confession** — the L1 stranger was the narrator's projected shadow. V1's L10 lens-break (`me and you`) and L16 stake (`might be mine`) were foreshadowing this. The song retroactively becomes self-portrait.

### 8.2 V2 structural arc (compressed mirror of V1)

| V1 (16 bars) | V2 (8 bars) |
|---|---|
| L1–9 documentary | V2 L1–2 confession reveal (dense, 13/11 syl) |
| L10–12 indictment | V2 L3–4 weight valley (sparse-ish, 10/11 syl, the "but now" pivot) |
| L13–16 prescription/stake | V2 L5–8 testimony (denser, 11/11/9/11 syl, knowledge-worker reality) |

Half the bars, full the arc.

### 8.3 V1 ↔ V2 callback web

| V1 | V2 | Function |
|---|---|---|
| L7 "Card declined by vending" | V2 L2 "me whose card was declined, brother" | Card-decline reread: V1 stranger = V2 narrator |
| L13 "dropping a dime" (charity advice) | V2 L8 "worth a dime" (self-devaluation) | Same word, opposite valence — verse weaponizes its own earlier line |
| L1 "papers in his fist" | V2 L1 "hacker, coach, guide" | What those hands used to do |
| L9 "Behind him now the sky" | V2 L5 "I'm behind the counter" | "Behind" repeats — narrator is always positioned behind something |

These callbacks emerged organically during writing rather than being engineered upfront.

### 8.4 V2 rhyme architecture

- L1/L2: slip pair `others / brother` (-uthers/-other)
- L3/L4: perfect couplet `far / jar` (-ar)
- L5–L8: 4-bar slip cluster `crimes / time / faultline / dime` (-ime/-ime/-ine+ault/-ime). Mirrors V1 L5–L8's 4-bar mono structure — V2 quotes V1's *form* even as content diverges.

### 8.5 Why 8 bars (not 16)

Phonk-canonical brevity. V2 executes its job by L8 (confession lands, dime callback closes). Extending to 16 risks diluting the hit. Total song runtime ~2:00–2:15 = phonk standard. The 8-bar V2 *is* the structure, not a half-structure.

### 8.6 Song flow (final)

```
Intro (8)         Sample chop + tape hiss + cowbell
Drop 1 (16)       VERSE 1
Break (4)         Drums strip, sample + 808 only
Hook (8)
Drop 2 (8)        VERSE 2 (half-length)
Hook (8)          Final, vocal chop ad-libs over
Outro (4)         Tape stop + filter sweep
```

Total ~64 bars at 140 BPM half-time = ~1:50–2:00. Adjust intro/outro length to taste.

### 8.7 V2 Performance Markup (full mode)

```
[VERSE 2 — Drop 2, drops at bar 41 of arrangement]

⟦chest⟧ [pocket] (confession reveal — narrator emerges as the L1 stranger)

V2 L1: I *used to be* a **hacker** · **coach** · **guide** to others /
V2 L2: {callback→V1 L7} And that's me whose card was **declined** · brother↓ //

⟦chest⟧ [pocket] (weight valley — the "but now" pivot)

V2 L3: I used to go *so hard* · *so long* · *so far* /
V2 L4: But now my **value** is tied to a tip jar↓ //

⟦chest⟧ ⟦grit⟧ [pocket] (testimony — knowledge worker present-tense)

V2 L5: {callback→V1 L9} I'm *behind* the counter · committing thought crimes /
V2 L6: [push] Fighting to build a plan before I'm outta time /
V2 L7: Makin' a **step** that'll cause a **faultline** /
V2 L8: {callback→V1 L13} Decades of expertise sold like it's worth a **dime** //

[OUTRO BUILD: tape stop begins under L8 sustain on "dime"]
```

**V2 energy arc:**
```
V2 L1–2     reveal plateau (chest, pocket-back, confession lands quietly)
V2 L3–4     valley (sparse-ish, "but now" hangs — let L4 die)
V2 L5–8     testimony rise (chest+grit, builds to L7 [push], climaxes on L8)
            L8 "dime" sustain → tape stop → song exit
```

**Texture:** ⟦chest⟧ all bars; ⟦grit⟧ added L5–L8 only (matches V1 L16's stake-bar texture)

**Pocket:** all `[pocket]` except V2 L6 `[push]` — the only push in V2, mirrors V1 L10's single push. Both are forward-leaning urgency moments in otherwise behind-the-beat verses.

**Pitch:** L2 ↓ on "brother" · L4 ↓ on "tip jar" (paired descents — both halves of "I was/I am" die at bar's end) · L5–L8 flat (texture carries weight)

**V2-specific ad-libs:**
- After L2 "brother" — whispered echo `declined... declined...` pitched -3 semis, panned wide, tape-saturated
- After L8 "dime" — whispered echo `dime... dime... dime...` pitched DOWN further each repetition (-2, -4, -6 semis) progressing with tape stop. Sample's death and the word's devaluation merge.

**V2 callback resolution:**
- V1 L7 "card declined" → V2 L2 "card was declined, brother" (confession)
- V1 L9 "Behind him" → V2 L5 "I'm behind the counter" (spatial position locks)
- V1 L13 "dropping a dime" → V2 L8 "worth a dime" (charity → self-devaluation)
- V1 L1 "papers in his fist" → V2 L1 "hacker, coach, guide" (what those hands used to do)


---

## 9. Production Checklist (Release-Ready)

Phased build with completion gates. ADHD-context: don't skip phases, don't move to next phase until current gate is met.

### 9.1 Vocal capture chain

**Owned gear (per inventory):** Zoom H6 with MSH-6 capsule. Prior diagnosis on H6 hip-hop track: excessive preamp gain + untreated room. Both fixable without new purchase.

**Recommended capture path (using owned gear):**

| Step | Setting / Action |
|---|---|
| Mic capsule | MSH-6 (mid-side stereo) — acceptable for vocal but not ideal. **Better:** if budget allows, Shure SM7B (~$400) or Rode NT1 (~$250) plus a budget audio interface (Focusrite Scarlett 2i2, ~$180). Wishlist note, not required. |
| H6 input | XY capsule pointed straight at mouth, ~6–8" distance. MSH-6 alternate: position mid-capsule cardioid pattern toward mouth, side capsules attenuated. |
| Preamp gain | **CRITICAL FIX** from prior session: target peak around -12 to -6 dBFS on H6 meter. If meter pegs near 0, gain too hot — back off. H6's preamp noise increases above ~70% gain; stay below that. |
| Room treatment (cheap fix) | Build a vocal booth: closet with hanging clothes, OR mattress propped behind mic, OR moving blankets on stands forming a 3-sided enclosure. Goal: kill back-wall reflection. Sit ~3 feet from any hard surface. |
| Pop filter | Required. DIY: pantyhose stretched over a wire hanger 4" from mic. |
| Monitoring | 64 Audio A12t IEMs (owned) — closed isolation, perfect for tracking. Send vocal pre-FX through H6 monitoring at low level to avoid bleed. |
| File format | Record at 24-bit / 48 kHz WAV. H6 supports this — set in H6 settings. |
| Take protocol | 3 full takes minimum, then doubles for hook (4 layers — main, double, low octave, ad-libs). Comp later in Ableton. |

**Gate:** vocal takes have NO audible room reverb tail, NO hiss above -50 dBFS noise floor, NO clipping. If any present, re-track.

### 9.2 Vocal processing chain (Ableton stock + Auto-Tune Unlimited)

In order on the Vocal Bus:

| Position | Plugin | Settings | Function |
|---|---|---|---|
| 1 | **Gate** (Ableton) | Threshold: -45 dB. Attack: 1ms. Hold: 10ms. Release: 100ms. | Cut room noise between phrases |
| 2 | **EQ Eight** (HP filter) | High-pass at 80 Hz, slope 24 dB/oct | Remove sub rumble (proximity effect, traffic) |
| 3 | **Auto-Tune Unlimited** | **Documentary verses (V1 L1–9, V2 L1–4):** Retune speed 30–50 (transparent — pitch correction without artifact). Key: D minor. <br> **Indictment + testimony (V1 L10–16, V2 L5–8):** Same transparent setting. <br> **Hook:** Retune speed 20–30 (slightly tighter — chant feel, slight processed character but not T-Pain). Avoid hard-tune. | Pitch correction with phonk-appropriate transparency |
| 4 | **Compressor** (Ableton) | Threshold to hit 4–6 dB GR on loudest phrases. Ratio 3:1. Attack 5ms. Release Auto. Makeup: by ear. | Tame dynamics for documentary intelligibility |
| 5 | **EQ Eight** (corrective) | Cut 200–400 Hz mud (-2 dB, Q 0.7, sweep to find boxiness). Cut 2.5–4 kHz harshness if needed. Boost 8–10 kHz +1 dB for air. | Vocal seat in mix |
| 6 | **De-Esser** (Multiband Dynamics in De-Ess preset) | Threshold to catch sibilance peaks. Frequency 5–8 kHz. | Tame "s" / "sh" peaks |
| 7 | **Saturator** | Type: Soft. Drive: 1–2 dB. | Match beat aesthetic, glue vocal to phonk character |

**Sends (parallel):**
- Send 1: **Plate reverb** (Ableton Reverb, Plate algorithm, 1.2s decay, pre-delay 30ms) — only on hook bars. Send level: -18 dB. Bypass during V1 L1–L8 (dense lyrics need clarity).
- Send 2: **1/8-dotted delay** (Ableton Delay or Echo) — only on hook bars and last word of each verse-section. Send level: -22 dB. Feedback 25%. Filter low-cut at 300 Hz.

**Hook layering (4 stacked vocals):**
1. Main vocal (lead, center)
2. Double (panned ~10 L)
3. Octave-down (panned ~10 R, low-pass at 4 kHz, -6 dB)
4. Ad-libs (`tatters... tatters...` whispered, panned wide L/R alternating)

### 9.3 Reference tracks (A/B during mix)

Listen at matched volume (use VU Meter Max for L4M plugin or Ableton's loudness tool). Match low-end weight, vocal forwardness, top-end roll-off character.

| Tier | Reference type | Use case |
|---|---|---|
| Memphis canonical | Three 6 Mafia (early catalog), Tommy Wright III, DJ Paul + Juicy J early productions | Tonal target — lo-fi tape, narrow stereo, dark mid-range |
| Modern Memphis revival | DJ Smokey, Soudiere, Pharmacist | Production-quality target with same lineage feel |
| Confessional phonk | $uicideboy$ (early Grey/Black era — circa "Kill Yourself" trilogy aesthetic) | Vocal-forward + Memphis-influenced; closest to this song's lyrical register |
| Loudness reference | Any modern phonk release on Spotify | Master loudness target (typically -8 to -7 LUFS integrated) |

**A/B protocol:** every mix decision, 30 seconds your track / 30 seconds reference / 30 seconds your track, matched volume. If your track sounds noticeably different in low-end weight or vocal level, reassess.

### 9.4 Stem export protocol

**When:** after mix is locked, before mastering.

**Format:** 24-bit WAV, 48 kHz (project sample rate), no master bus processing on stems.

**Stem list (export each as individual file):**

| # | Stem name | Contents |
|---|---|---|
| 1 | `01_kick.wav` | Kick drum, dry |
| 2 | `02_snare.wav` | Snare, dry |
| 3 | `03_hat.wav` | Closed hat, dry |
| 4 | `04_cowbell.wav` | Cowbell pattern, dry |
| 5 | `05_crackle.wav` | Vinyl crackle layer |
| 6 | `06_808.wav` | 808 with full saturation chain printed |
| 7 | `07_sample_loop.wav` | Melodic sample / organ + vocal chop |
| 8 | `08_vocal_lead.wav` | Lead vocal with full processing chain printed |
| 9 | `09_vocal_hook_layers.wav` | Hook stack (double + octave-down + ad-libs combined) |
| 10 | `10_master_reference.wav` | Full mix bounce, no master bus FX (for mastering engineer reference) |

**Naming convention:** `stackin-bands_v[version]_stems_[date]/##_stemname.wav`

**Archive location:** project folder + cloud backup (Google Drive recommended given existing `things-i-own` workflow). Don't lose stems — they enable remixes, live performance, and re-mastering.

### 9.5 Mastering protocol

**Self-master OR send out?** Self-master is fine for first single; pro-master if budget allows ($30–80 typical for phonk on platforms like Bandlab or low-tier engineers).

**Self-master chain (Ableton stock + careful gain staging):**

In order on Master:

| Position | Plugin | Settings |
|---|---|---|
| 1 | **EQ Eight** (corrective) | Subtle: HP at 25 Hz (kill sub-sonic). High-shelf cut -1 dB at 12 kHz if too bright. |
| 2 | **Saturator** | Type: Soft. Drive: 2–3 dB. (Already specced in §5.5.6.) |
| 3 | **Multiband Dynamics** (or Glue Compressor) | Glue Comp: Ratio 2:1, Attack 10ms, Release Auto, GR 1–2 dB. |
| 4 | **EQ Eight** (final tonal) | Optional shelf: +0.5 dB at 8 kHz for air, +0.3 dB at 60 Hz for low weight. Subtle only. |
| 5 | **Limiter** | Ceiling: -1.0 dBTP. Gain: push until hitting -8 to -7 LUFS integrated. Verify with Ableton's loudness meter or VU Meter Max for L4M. |

**Verification before bounce:**
- Integrated LUFS: -8 to -7 (phonk standard)
- Short-term LUFS max: -6 (loudest 3-sec window)
- True peak: -1.0 dBTP (no overs)
- Sample peak: should be below -1.0 dBFS after limiter
- DC offset: 0 (Ableton handles this)

**Distribution format (master file):**
- Spotify / Apple Music / YouTube Music (via DistroKid, TuneCore, etc.): 16-bit / 44.1 kHz WAV, dithered from 24-bit master
- Bandcamp: upload 24-bit / 48 kHz WAV (preserves quality, Bandcamp transcodes)
- SoundCloud: 16-bit / 44.1 kHz WAV or 320 kbps MP3
- Backup: keep 24-bit / 48 kHz master WAV indefinitely

**Dither:** when bouncing 16-bit from 24-bit project, enable dither in Ableton's Render dialog (POW-r 1, 2, or 3 — try POW-r 2 for music with both transients and sustain).

### 9.6 Session order (phased build with gates)

**Phase 1 — Beat skeleton** (target: 1–2 sessions)
- Build Drum Rack (kick + snare + hat + cowbell)
- Lay 4-bar drum pattern (§5.1) + 1 bar fill (§5.2)
- Add 808 on separate track with saturation chain (§5.5.5)
- Source + chop sample loop (§4.4 — pitched-down minor organ + vocal chop)
- Apply Groove Pool (§5.5.2)
- **Gate:** loop sounds like phonk for 8 bars without getting boring. If not, fix sample or 808 pattern before moving on.

**Phase 2 — Beat arrangement** (target: 1 session)
- Build full song structure (§4.5): intro → drop 1 → break → hook → drop 2 → hook → outro
- No vocals yet
- Add tape stop, filter sweeps, perc additions (§5.4)
- **Gate:** instrumental sustains interest for 2 minutes solo. If not, add variation.

**Phase 3 — Vocal recording** (target: 1–2 sessions)
- Set up capture chain (§9.1)
- Track lead vocal: 3 full takes, comped after
- Track hook layers (4 stacks)
- Track ad-libs (V2 "declined" echo, "dime" pitched-down decays)
- **Gate:** clean takes (no clipping, no room reverb, no excessive hiss). Re-track if not.

**Phase 4 — Vocal editing** (target: 1 session)
- Comp best takes per phrase
- Time-align doubles to lead
- Tune through Auto-Tune Unlimited (§9.2 step 3)
- Apply full vocal processing chain (§9.2)
- **Gate:** vocals sit in pocket, intelligible, no obvious tuning artifacts. Match to V1 L1–L9 documentary clarity benchmark.

**Phase 5 — Mixing** (target: 2 sessions)
- Balance levels (start with vocal, build instrumental around)
- Apply drum bus + 808 bus + master bus chains
- A/B against references (§9.3)
- Sends (plate, delay) for hook only
- **Gate:** mix translates on at least 3 systems (IEMs, phone speaker, car if possible). Vocal intelligible on phone speaker.

**Phase 6 — Mastering** (target: 1 session)
- Apply mastering chain (§9.5)
- Verify LUFS, true peak, sample peak
- Bounce 24-bit master + 16-bit/44.1 distribution copy
- **Gate:** master matches reference loudness without obvious distortion or pumping.

**Phase 7 — Stems + metadata + release** (target: 1 session)
- Export stems (§9.4)
- Fill release metadata (§9.7)
- Upload to distributor
- **Gate:** all files archived, distributor confirms ingestion.

**Anti-hyperfocus reminder:** if any phase exceeds 2 sessions, stop. Walk away. The 85% rule applies — get it to 85% then move on. Polish in mastering, not in earlier phases.

### 9.7 Release metadata template

```yaml
title: "Stackin Bands"
artist: [DECIDE — Wabi-Sabi? VIKTECH? new alias?]
genre_primary: Phonk
genre_secondary: Memphis Phonk
bpm: 140
key: D minor
duration: ~2:00
isrc: [auto-assigned by distributor]
release_date: [TBD]
explicit: [Y/N — V2 has "brother" + "ain't" + worth-a-dime — not explicit, but consider whether language flags any platform]
distributor: [DistroKid / TuneCore / Routenote / Amuse]
platforms: Spotify, Apple Music, YouTube Music, Bandcamp, SoundCloud
cover_art: [TBD — see brief below]
description_short: |
  Memphis phonk debut single. Threshold-person ER scene from outside, then inside.
  A meditation on devaluation, recognition, and the wristbands you carry.
tags: phonk, memphis phonk, milwaukee, wabi-sabi, viktech, alternative hip-hop, lo-fi
```

**Artist-name decision flag:** unresolved. Wabi-Sabi is your established music alias for the DnB album project. Releasing phonk under same name = brand cohesion (one artist project, multi-genre output) vs brand fracture (Wabi-Sabi means DnB to listeners). VIKTECH is your decade-old personal brand. New alias = cleanest separation. **Decide before distributor upload.**

**Cover art brief (for AI image gen or designer):**
- Single hospital wristband, frayed, lying on wet pavement at dawn
- Gray-blue sky with copper sunrise burn at horizon
- Square format (3000x3000 px for streaming), or 1:1 with safe area for thumbnail crop
- Aesthetic: lo-fi, slight VHS grain, desaturated except for the orange horizon
- Title text optional — many phonk releases skip on-cover text

### 9.8 Project versioning protocol

**Filename convention:** `stackin-bands_v[major].[minor]_[YYYY-MM-DD].als`

Examples:
- `stackin-bands_v1.0_2026-05-04.als` (initial beat skeleton)
- `stackin-bands_v1.1_2026-05-05.als` (beat arrangement)
- `stackin-bands_v2.0_2026-05-08.als` (vocals tracked — major version bump for major phase change)
- `stackin-bands_v3.0_2026-05-12.als` (mix-locked)
- `stackin-bands_v4.0_2026-05-13.als` (master)

**Save protocol:**
- Save at end of every session (Ctrl+S)
- "Save As" with new version number for major phase transitions or before risky changes
- Daily snapshot: copy current `.als` to `_archive/` subfolder with date stamp

**Backup:**
- Local: project folder on internal drive
- Cloud: Google Drive (mirrors `things-i-own` workflow)
- External: SSD or USB stick — full project including samples + stems, weekly snapshot

**Named milestones to preserve forever:**
1. Beat-locked version (Phase 2 complete)
2. Vocal-locked version (Phase 4 complete)
3. Mix-locked version (Phase 5 complete)
4. Master version (Phase 6 complete) — never overwrite

### 9.9 Live-deployment readiness (lightweight, since standalone single)

You picked standalone single (not part of an album/set), but archive these in case live performance becomes an option later:

- **Stem archive** (already specified in §9.4) — required for Resolume / Ableton Live performance use
- **Instrumental version** — bounce instrumental-only mix during stem export (vocal removed). Useful for performances and for licensing.
- **Acapella version** — bounce vocal-only stems at full mix levels. Useful for remixes if you license it later.
- **Ableton live-set template** — duplicate the project, strip down to performance essentials (stems on tracks, MIDI control mappings, scenes for sections). Save as `stackin-bands_LIVE.als`. Optional. Skip unless live performance is on the calendar.
