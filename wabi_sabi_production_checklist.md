# WABI-SABI -- Live Set: "Beautiful Decay"

> *A 10-track DnB live set structured as a four-act narrative arc rooted in wabi-sabi philosophy -- the beauty of imperfection, impermanence, and incompleteness. Complete Production & Performance Checklist for Akai MPC Live II.*

---

## Global Set Parameters

### Master Settings

- [ ] Master key: D minor (shifting to F minor in Act III)
  - [ ] D minor = melancholy/introspection
  - [ ] F minor = tension/darkness
  - [ ] **VERIFY:** Play a D minor chord and an F minor chord back to back -- confirm the emotional shift feels right for the arc
- [ ] Tempo range: 87-176 BPM
  - [ ] Halftime passages at 87 feel against 174 grid
  - [ ] **TEST:** Tap tempo on a metronome at 87 and 174 -- internalize both feels before programming
- [ ] Target loudness: -8 to -6 LUFS integrated per track
  - [ ] Peaks at -1 dBTP
  - [ ] Leaves headroom for venue PA limiter
  - [ ] **VERIFY:** Run each finished track through a loudness meter (LUFS) and confirm it falls in -8 to -6 range
  - [ ] **VERIFY:** Check true peak meter -- no sample exceeds -1 dBTP
- [ ] Stereo width: mono below 200 Hz, widen above
  - [ ] Sub bass mono-summed at all times
  - [ ] Stereo field opens proportionally with frequency
  - [ ] **TEST:** Collapse master to mono -- confirm no low-end phase cancellation or volume loss below 200 Hz
  - [ ] **TEST:** Use a stereo correlation meter -- confirm correlation stays above +0.3 on all tracks

### Master Bus Chain

- [ ] Insert 1: Soft-clip saturator
  - [ ] **TEST:** Bypass and re-engage -- confirm it adds warmth without audible distortion on quiet passages
- [ ] Insert 2: Glue compressor
  - [ ] Ratio: 2:1
  - [ ] Attack: 10 ms
  - [ ] Release: 100 ms
  - [ ] GR target: 1-2 dB max -- the imperfections should breathe
  - [ ] **VERIFY:** Watch GR meter during loudest section (Track 9) -- confirm it never exceeds 3 dB
  - [ ] **TEST:** Bypass compressor during Track 1 -- if the difference is dramatic, you are compressing too hard
- [ ] Insert 3: Brickwall limiter at -1 dBTP
  - [ ] **VERIFY:** Limiter activity LED should barely flicker on average material -- only catching transient peaks
  - [ ] **TEST:** Play Track 9 at full level -- confirm limiter is not pumping or audibly squashing

---

## MPC Live II Set Configuration

### Project Architecture

- [ ] Song mode with 10 sequences chained
  - [ ] 1 sequence = 1 track
  - [ ] Verify sequence order: 1 through 10
  - [ ] All sequences set to single play (no loop)
  - [ ] **TEST:** Play Song from beginning -- confirm it advances through all 10 sequences without stopping or looping
  - [ ] **TEST:** Let each sequence end naturally -- confirm it transitions to next without gap or overlap
- [ ] **VERIFY:** Save project after confirming sequence chain -- name with date (e.g., WABISABI_20260408)

### Track Layout (Per Sequence)

- [ ] Track 1: Drum program -- breaks and percussion
- [ ] Track 2: Keygroup program -- bass
- [ ] Track 3: Keygroup program -- synths and pads
- [ ] Track 4: Audio track -- field recordings and textures
- [ ] Track 5: Audio track -- FX and risers
- [ ] **VERIFY:** Solo each track in isolation across ALL 10 sequences -- confirm no silent/missing tracks
- [ ] **VERIFY:** Check MPC CPU meter while all 5 tracks play simultaneously -- confirm no overloads or dropouts
- [ ] **TEST:** Monitor audio output while switching between sequences -- confirm no clicks, pops, or digital artifacts at boundaries

### Q-Link Mapping

- [ ] Q-Link 1: Filter cutoff (low-pass on drum bus)
- [ ] Q-Link 2: Filter cutoff (high-pass on pad bus)
- [ ] Q-Link 3: Reverb send level (global)
- [ ] Q-Link 4: Delay feedback amount
- [ ] Q-Link 5: Master low-pass filter for transitions
  - [ ] Test: sweep each Q-Link 0-100% and confirm range
- [ ] **VERIFY:** Q-Link 1 at 0% should NOT fully kill the drums -- set minimum to ~200 Hz so you never lose the beat entirely
- [ ] **VERIFY:** Q-Link 4 (delay feedback) at 100% should NOT cause runaway feedback -- set max to 85%
- [ ] **TEST:** Sweep Q-Link 5 from full open to fully closed while Track 4 plays -- confirm smooth transition with no stepping or zipper noise
- [ ] **VERIFY:** Q-Link assignments persist after power cycle -- turn MPC off, back on, reload project, re-test

### XYFX Pad

- [ ] X-axis: Filter cutoff (LP, full range 20 Hz - 20 kHz)
- [ ] Y-axis: Reverb wet/dry (0% - 80% max)
  - [ ] Test XYFX with headphones before soundcheck
- [ ] **VERIFY:** Center position of XYFX = neutral (no filtering, no reverb) -- this is your home position
- [ ] **TEST:** Move to all four corners and back to center -- confirm audio returns to unaffected state at center
- [ ] **VERIFY:** Max Y (reverb 80%) does NOT wash out the mix to the point of losing the beat

### Transitions

- [ ] Song mode step-advance enabled
- [ ] Every track tail has 8-bar transition window
  - [ ] Practice manual sequence triggers in transition windows
  - [ ] Fallback: crossfade sequences if manual trigger missed
- [ ] **TEST:** Rehearse every transition 3 times minimum -- focus on the 3 hardest:
  - [ ] Track 3 -> 4 (ambient to jungle punch)
  - [ ] Track 5 -> 6 (liquid to halftime -- tempo feel change)
  - [ ] Track 7 -> 8 (silence gap into full-tempo explosion)
- [ ] **VERIFY:** Time each transition with a stopwatch -- confirm none exceeds 60 seconds or feels rushed under 20 seconds
- [ ] **TEST:** Deliberately miss a manual trigger -- confirm the fallback crossfade catches it cleanly

---

## Act I: Awakening

*The set opens in stillness. Granular textures, field recordings, and whispered breaks.*

---

### Track 1: Dust & Light -- Ambient DnB, 170 BPM

**Concept:** *Sunrise through dirty glass. The sound of something old becoming illuminated.*

#### Sound Design: Granular Textures

- [ ] Sample a bowed metal object or singing bowl
  - [ ] Load into MPC granular engine (Keygroup -> Grain mode)
  - [ ] Grain size: 40-80 ms
  - [ ] Density: 60-70%
  - [ ] Scatter: 30%
  - [ ] Automate grain position slowly across 5-minute runtime
    - [ ] Goal: evolving timbral movement without repetition
- [ ] **TEST:** Solo the granular pad and listen for 60 seconds straight -- confirm the texture evolves and does not feel static or looping
- [ ] **VERIFY:** Grain position automation plays back correctly from start to end -- scrub to 1:00, 2:30, and 4:00 and confirm audibly different timbres at each point
- [ ] **TEST:** Check for digital artifacts or clicks at extreme grain settings -- if present, increase grain size by 10 ms

#### Sound Design: Breaks

- [ ] Source: thinned jungle breaks (Think & Change or Winston)
  - [ ] Program loose, ghosted 2-step pattern
- [ ] HPF at 300 Hz on break bus -- kick is a whisper, not a punch
- [ ] Room reverb: 0.4s decay, 20 ms pre-delay
  - [ ] Goal: small, intimate space
- [ ] **TEST:** Solo breaks with HPF engaged -- confirm the kick is felt as a ghost, not a hit
- [ ] **VERIFY:** Reverb tail does not bleed into the next bar's downbeat -- if it does, shorten decay by 50 ms
- [ ] **TEST:** A/B the breaks with and without reverb -- the reverb should add space, not mud

#### Sound Design: Sub Bass

- [ ] Sine wave sub
  - [ ] Level: -12 dB below final mix level
  - [ ] Mono
  - [ ] HPF at 30 Hz
  - [ ] LPF at 120 Hz
  - [ ] Goal: barely present -- just enough to feel the floor
- [ ] **VERIFY:** Sub is inaudible on laptop speakers but felt on monitors/headphones with sub response
- [ ] **TEST:** Collapse to mono -- confirm sub level stays identical (no phase issues)
- [ ] **TEST:** Mute the sub and listen -- then unmute -- the difference should be felt in the chest, not heard in the ears

#### Sound Design: Atmosphere

- [ ] Layer 2-3 field recordings
  - [ ] Rain on metal
  - [ ] Distant traffic
  - [ ] Tape hiss
- [ ] Level: -18 to -24 dB
- [ ] Pan: 50-70% L/R
- [ ] **TEST:** Mute all field recordings -- the track should feel empty and clinical without them
- [ ] **TEST:** Solo each field recording individually -- confirm none has DC offset, hum, or unwanted low-frequency rumble
- [ ] **VERIFY:** Field recordings do not mask the granular pad upper frequencies -- if they compete, cut 2-4 kHz on the field recordings by 2 dB

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Granular pad | -6 dB | 400 Hz - 4 kHz | Wide (70% L/R) |
| Breaks | -9 dB | 300 Hz - 8 kHz (HPF@300) | Center |
| Sub | -12 dB | 30 - 120 Hz | Mono |
| Field recordings | -18 to -24 dB | 1 - 10 kHz | Spread L/R |

- [ ] **VERIFY:** Meter each element solo'd -- confirm levels match the table above within +/- 1 dB
- [ ] **VERIFY:** Full mix of Track 1 reads -8 LUFS or softer -- this is the quietest track in the set
- [ ] **TEST:** Listen on headphones, then on monitors -- confirm the balance translates between both

#### Transition Out

- [ ] 8-bar tail
  - [ ] Automate grain size: 80 ms -> 200 ms
  - [ ] Texture blurs into a wash
  - [ ] Wash hands off to Track 2 opening melodic phrase
- [ ] **TEST:** Play the last 16 bars of Track 1 into the first 8 bars of Track 2 -- confirm the handoff feels seamless
- [ ] **VERIFY:** No volume spike or drop at the sequence boundary
- [ ] **VERIFY:** The grain wash and Track 2 Rhodes entry overlap smoothly -- no frequency clash in the 400 Hz - 2 kHz range

---

### Track 2: Fading Ink -- Liquid DnB, 172 BPM

**Concept:** *Melody enters like brushstrokes on wet paper -- bleeding at the edges.*

#### Sound Design: Lead Synth ('Watercolor')

- [ ] Source: Rhodes or electric piano sample
- [ ] MPC insert FX chain:
  - [ ] Chorus: rate 0.3 Hz, depth 40%
  - [ ] Plate reverb: 1.8s decay, 30% wet
  - [ ] Tape saturation: drive 15-20%
- [ ] Velocity-map filter cutoff: harder hits open, softer stay muted
- [ ] **TEST:** Play the Rhodes at velocity 30, 60, 90, 127 -- confirm audible timbral difference at each level
- [ ] **TEST:** Bypass the chorus -- the sound should lose its bleeding edge quality and sound flat/dry
- [ ] **VERIFY:** Tape saturation is subtle -- A/B bypass it and listen for warmth, not crunch

#### Sound Design: Percussion ('Brush-Stroke')

- [ ] Layer shaker loops with hand-played rim shots
- [ ] Short bright room reverb: 0.3s decay
  - [ ] HPF at 2 kHz on reverb return only
    - [ ] Goal: airy, papery texture above the breaks
- [ ] Quantize at 55-60% on MPC for human feel
- [ ] **TEST:** Listen to percussion solo'd -- it should sound like a person playing, not a machine
- [ ] **VERIFY:** The reverb return HPF is working -- solo the reverb return and confirm no low-end content below 2 kHz

#### Sound Design: Breaks

- [ ] Source: cleaner break with hi-hat detail (Apache or Skull Snaps)
- [ ] Full frequency, but roll off at 60 Hz (gentle 6 dB/oct)
  - [ ] Sub handles the low end
- [ ] **VERIFY:** Compare break low end with Track 1 breaks -- Track 2 should have slightly more body (HPF at 60 vs 300)
- [ ] **TEST:** Play breaks and sub together -- confirm they do not fight in the 60-120 Hz range

#### Sound Design: Bass

- [ ] Reese bass, detuned 7-10 cents
  - [ ] Filter automation: 2-bar LFO on cutoff (LP 800 Hz -> 2 kHz)
  - [ ] Sidechain from kick:
    - [ ] Ratio: 4:1
    - [ ] Attack: 0.5 ms
    - [ ] Release: 80 ms
- [ ] **TEST:** Solo bass with sidechain active -- confirm the duck is audible but not pumping
- [ ] **VERIFY:** Reese detuning creates movement, not dissonance -- if it sounds out of tune, reduce detune to 5 cents
- [ ] **TEST:** Play bass and breaks together -- the kick should poke through the bass cleanly on every hit

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Rhodes lead | -3 dB | 500 Hz - 5 kHz | Center (chorus stereo) |
| Brush percussion | -8 dB | 2 - 12 kHz | 40% L/R |
| Breaks | -4 dB | 60 Hz - 12 kHz | Center |
| Reese bass | -5 dB | 40 - 800 Hz (auto) | Mono below 200 Hz |

- [ ] **VERIFY:** Meter each element and confirm levels within +/- 1 dB of table
- [ ] **VERIFY:** Full mix reads -7 to -6 LUFS -- slightly louder than Track 1
- [ ] **TEST:** Mono check -- confirm Rhodes chorus width collapses cleanly without phase cancellation

#### Transition Out

- [ ] Rhodes sustains D minor 7th chord
  - [ ] Breaks thin to hi-hats only over 4 bars
  - [ ] Master LP sweep: 8 kHz -> 800 Hz
  - [ ] Pulls audience into Track 3
- [ ] **TEST:** Play last 8 bars of Track 2 into first 8 of Track 3 -- confirm LP sweep feels gradual, not abrupt
- [ ] **VERIFY:** The sustained D minor 7th chord does not clash with Track 3 opening harmony

---

### Track 3: Patina -- Atmospheric DnB, 172 BPM

**Concept:** *Same tempo, deeper layers. Oxidized copper -- beauty through slow chemical change.*

#### Sound Design: Pad Layer

- [ ] Two detuned saw pads: +5 cents and -5 cents
  - [ ] Slow phaser: rate 0.1 Hz
- [ ] Automate reverb send: 20% -> 60% across runtime
  - [ ] Pads dissolve into space
- [ ] LPF at 6 kHz to keep warm and behind the mix
- [ ] **TEST:** Solo pads at the 1:00 mark and the 4:00 mark -- confirm audibly different reverb density
- [ ] **VERIFY:** Pads sit BEHIND the breaks in the mix -- if the pads dominate, lower by 2 dB or cut 1-2 kHz by 3 dB

#### Sound Design: Field Recordings

- [ ] Now compositional, not just texture
  - [ ] Creaking wood
  - [ ] Wind through a structure
  - [ ] Distant metallic resonance
- [ ] Time creaking to hit on beat 3 of every 4th bar
- [ ] Level: -12 dB -- audible, identifiable, integrated
- [ ] **TEST:** Can a listener identify "that is wood creaking" and "that is wind" without being told? If not, they are too quiet or too processed
- [ ] **VERIFY:** Creaking hits beat 3 accurately -- scrub to 3 different points in the track and confirm rhythmic alignment
- [ ] **VERIFY:** Field recordings do not introduce unwanted low-end rumble -- HPF each recording at 100 Hz if needed

#### Sound Design: Break Programming

- [ ] Ghost snare notes: velocity 30-40% on every 16th around main hits
  - [ ] Goal: density without volume
- [ ] Vinyl-crackle layer at -20 dB across entire break bus
- [ ] **TEST:** Mute ghost notes -- the beat should feel sparse and naked without them
- [ ] **TEST:** Mute vinyl crackle -- the breaks should feel sterile without it
- [ ] **VERIFY:** Ghost note velocity does not exceed 45 -- check in the MPC piano roll

#### Sound Design: Bass

- [ ] Continue Reese from Track 2
  - [ ] Add sub-octave sine (-1 octave from root)
  - [ ] Sub-octave level: -6 dB relative to Reese
    - [ ] Goal: deepens low end without mud
- [ ] **TEST:** Solo bass with sub-octave added -- confirm the low end feels deeper, not boomy
- [ ] **TEST:** Check on a frequency analyzer -- sub-octave should show a clean peak at the fundamental, not broad low-end energy

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Stacked pads | -5 dB | 200 Hz - 6 kHz | Wide (80% L/R) |
| Field recordings | -12 dB | 500 Hz - 8 kHz | Placed in stereo field |
| Breaks + ghosts | -4 dB | 80 Hz - 10 kHz | Center |
| Reese + sub | -4 dB | 30 - 600 Hz | Mono |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -7 to -6 LUFS -- similar energy to Track 2
- [ ] **TEST:** Compare Track 2 and Track 3 back-to-back -- Track 3 should feel deeper and wider, not louder

#### Transition Out

- [ ] 16-bar slow build
  - [ ] Field recordings rise 6 dB
  - [ ] White noise riser: HP sweep 200 Hz -> 8 kHz over 16 bars
- [ ] Beat 1 of Track 4: everything cuts except sub
  - [ ] Sub sustains for 1 bar, then Amen hits
- [ ] **TEST:** Play last 16 bars of Track 3 into Track 4 -- the energy shift should feel like a release, not a shock
- [ ] **VERIFY:** White noise riser does not clip the master -- check peak meter during the riser loudest point
- [ ] **VERIFY:** The 1-bar sub sustain into Track 4 Amen creates anticipation, not confusion -- if it feels too long, shorten to half a bar

---

## Act II: Descent

*Energy rises, peaks emotionally, then collapses into halftime intimacy.*

---

### Track 4: Moss on Stone -- Jungle/DnB Hybrid, 170 BPM

**Concept:** *First real punch. Primal energy breaking through the contemplative opening.*

#### Sound Design: Amens

- [ ] Chop Amen break in MPC Chop mode (threshold-based)
  - [ ] Manually clean chop points
- [ ] Program classic jungle pattern:
  - [ ] Double-time kick hits
  - [ ] 32nd-note snare rolls on fills every 8 bars
- [ ] Parallel distortion:
  - [ ] Duplicate break track
  - [ ] Tube saturate copy: drive at 70%
  - [ ] HPF at 1 kHz on distorted copy
  - [ ] Blend distorted at -8 dB under clean
    - [ ] Goal: aggression without destroying transients
- [ ] **TEST:** Solo each chop point -- confirm no clicks at slice boundaries (if present, nudge slice point or add 2 ms fade)
- [ ] **TEST:** Play clean Amen solo, then add distorted layer -- the character should change but transients should remain sharp
- [ ] **VERIFY:** 32nd-note snare rolls are tight -- listen at half speed in MPC to confirm timing is precise
- [ ] **VERIFY:** Parallel distortion HPF at 1 kHz is working -- solo the distorted track and confirm no low-end mud

#### Sound Design: Bass

- [ ] Switch from Reese to square-wave sub
  - [ ] Slight overdrive
  - [ ] Short decay: 300 ms
  - [ ] Retrigger on every kick hit
- [ ] Mono, hard LPF at 150 Hz
  - [ ] Goal: percussive, gut-punch bass
- [ ] **TEST:** Play bass and kick together -- the retrigger should lock them in sync with no flamming
- [ ] **VERIFY:** Bass is entirely below 150 Hz on a frequency analyzer -- nothing leaking above
- [ ] **TEST:** Listen on a system with good sub -- the bass should hit the chest physically

#### Sound Design: Stabs

- [ ] Minor 9th chord stabs
  - [ ] Source: funk sample or detuned supersaw
- [ ] Tight gate: 50 ms decay
- [ ] Reverb send only -- no reverb on dry signal
  - [ ] Goal: presence without wash
- [ ] **TEST:** Mute the reverb send -- stabs should sound dry and punchy but present
- [ ] **VERIFY:** Gate is cutting cleanly at 50 ms -- no tail or bleed after the stab

#### Sound Design: Transition Element

- [ ] Pitched-down vocal chop ('the old ways')
  - [ ] Bitcrusher: 12-bit, 22 kHz sample rate
- [ ] Enters at 2:00 mark, repeats every 8 bars
- [ ] **VERIFY:** Vocal chop is intelligible despite bitcrushing -- the words should be recognizable
- [ ] **TEST:** Mute the vocal chop -- then unmute -- it should add narrative depth, not clutter

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Amen (clean) | 0 dB (ref) | Full spectrum | Center |
| Amen (dist parallel) | -8 dB | 1 kHz+ | Slight wide |
| Square sub | -2 dB | 30 - 150 Hz | Mono |
| Stabs | -6 dB | 800 Hz - 6 kHz | 30% L/R alternating |
| Vocal chop | -10 dB | 200 Hz - 3 kHz | Center |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -7 to -6 LUFS -- significant energy jump from Act I
- [ ] **TEST:** Compare Track 3 ending to Track 4 opening back-to-back -- the energy contrast should be dramatic but not jarring

#### Transition Out

- [ ] Amens thin to single repeating snare hit
  - [ ] Bass drops out
- [ ] 4 bars of just snare + reverb tail
  - [ ] Track 5 warm pad floods in underneath
- [ ] **TEST:** Play the transition -- confirm the snare reverb tail sustains long enough to fill the 4 bars without silence
- [ ] **VERIFY:** Track 5 pad entry is audible under the snare reverb -- if masked, raise pad entry by 2 dB

---

### Track 5: Cracked Glaze -- Liquid DnB, 174 BPM

**Concept:** *A breath after jungle chaos. Warm but fractured -- the emotional peak.*

#### Sound Design: Lead Melody

- [ ] Female vocal sample
  - [ ] Time-stretch to 150% in MPC Warp mode (complex algorithm)
  - [ ] Artifacts appear: pitch wobbles, granular stutters
  - [ ] DO NOT FIX the artifacts -- they are the 'cracks'
- [ ] Layer underneath: clean quantized sine-wave melody
  - [ ] Follows same phrase as vocal
    - [ ] Contrast between broken vocal and pure sine IS the track
- [ ] **TEST:** Solo the stretched vocal -- confirm artifacts are musical (wobbles and texture), not broken (clicks and dropouts). If broken, try a different warp algorithm
- [ ] **TEST:** Solo the sine melody alone -- it should sound too clean, too perfect, almost sterile
- [ ] **VERIFY:** When both play together, the vocal imperfections are highlighted by the sine purity -- this contrast must be audible

#### Sound Design: Pads

- [ ] String-ensemble patch, MPC multi-layer sampling:
  - [ ] Velocity layer 1 (pp): solo cello sample
  - [ ] Velocity layer 2 (mf): string quartet
  - [ ] Velocity layer 3 (ff): full orchestra hit
- [ ] Play dynamically to shift between intimate and expansive
- [ ] **TEST:** Play the same note at velocity 20, 64, and 127 -- confirm three distinctly different timbres
- [ ] **VERIFY:** Velocity crossfade between layers is smooth -- no abrupt timbral jumps at the boundaries

#### Sound Design: Breaks

- [ ] Clean, minimal two-step
  - [ ] Snare on 2 and 4
  - [ ] Ghost hi-hats at low velocity
- [ ] No fills, no drama in the drums
  - [ ] All emotion comes from other elements
- [ ] **TEST:** Play the full mix, then mute everything except the breaks -- the drums alone should feel boring. That is correct.
- [ ] **VERIFY:** No unintentional fills or variations crept in during programming

#### Sound Design: Bass

- [ ] Sine + triangle wave blend
  - [ ] Half-bar sustain
  - [ ] Gentle sidechain
  - [ ] LPF at 400 Hz
    - [ ] Goal: this bass hums, it does not hit
- [ ] **TEST:** Does the bass feel like a warm blanket under the mix? If it feels punchy, increase attack time or lower LPF to 300 Hz
- [ ] **VERIFY:** Sidechain is gentle -- the duck should be 2-3 dB max, not a noticeable pump

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Stretched vocal | -3 dB | 800 Hz - 6 kHz | Center |
| Sine melody | -8 dB | 1 - 4 kHz | Center |
| Strings (vel-layer) | -5 dB | 300 Hz - 8 kHz | Wide (90% L/R) |
| Breaks | -6 dB | 100 Hz - 10 kHz | Center |
| Bass | -4 dB | 40 - 400 Hz | Mono |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -7 to -6 LUFS
- [ ] **TEST:** Listen to this track with eyes closed for the full duration -- does it create an emotional response? If not, revisit the vocal/sine contrast and string dynamics

#### Performance

- [ ] Pull back physically during this track
  - [ ] Less movement
  - [ ] Less Q-Link manipulation
- [ ] Let the music sit -- give the crowd space to close their eyes
- [ ] **VERIFY:** Rehearse this track 3 times keeping your hands off the controls -- build the muscle memory of restraint

#### Transition Out

- [ ] Vocal repeats a single syllable
  - [ ] Pitch down: -2 semitones over 8 bars
- [ ] LP filter closes on full mix: 6 kHz -> 400 Hz
  - [ ] Beat drops out 2 bars before Track 6
- [ ] **TEST:** The pitch-down on the vocal should feel like the track is falling asleep, not breaking
- [ ] **VERIFY:** The 2-bar gap between beat dropout and Track 6 entry feels like held breath, not dead air
- [ ] **VERIFY:** LP filter at 400 Hz leaves only bass and muffled pads -- confirm the sonic character matches "a radio in the next room"

---

### Track 6: Worn Thread -- Halftime Drop, 87 BPM Feel

**Concept:** *Tempo halves. Dusty, lo-fi, intimate. A deliberate pause. Tension through restraint.*

#### Sound Design: Tempo Handling

- [ ] MPC stays at 174 BPM grid
  - [ ] Halftime feel: program drums on every other beat
    - [ ] Kick on bar 1 beat 1
    - [ ] Snare on bar 2 beat 1
  - [ ] Maintains sync for Act III tempo-double
- [ ] **VERIFY:** Play Track 5 into Track 6 -- confirm the MPC does not change tempo. The halftime feel comes from programming, not a tempo change
- [ ] **TEST:** Tap along to Track 6 -- your body should naturally halve to 87 BPM even though the grid is 174

#### Sound Design: Drums

- [ ] Entire drum bus through lo-fi chain:
  - [ ] Bitcrusher: 14-bit, 32 kHz
  - [ ] Tape saturation: drive 25%
  - [ ] Sample-rate reducer: to taste
    - [ ] Goal: sounds like a cassette in the next room
- [ ] **TEST:** A/B the lo-fi chain on and off -- the processed version should sound distant and warm, not crunchy or harsh
- [ ] **VERIFY:** Drums still have a clear transient on the snare hit despite lo-fi processing -- if the snare disappears, reduce bitcrusher depth to 15-bit

#### Sound Design: Texture (Piano)

- [ ] Solo piano, processed to sound cheap-mic'd:
  - [ ] Aggressive HPF at 500 Hz
  - [ ] Narrow bandpass: 1-3 kHz
  - [ ] Pink noise at -24 dB underneath
- [ ] Play: root notes and 5ths only, sparse
  - [ ] Every note should feel earned
- [ ] **TEST:** The piano should sound like a lo-fi recording, not a modern studio piano -- if it sounds too clean, increase HPF to 600 Hz
- [ ] **VERIFY:** Pink noise is inaudible in isolation at -24 dB but adds air when layered -- mute and unmute to confirm subtle presence

#### Sound Design: Sub Bass

- [ ] Inaudible rumble: sine at 35-40 Hz
  - [ ] Barely hitting meters
  - [ ] Long attack: 200 ms (swells in after each note)
    - [ ] Goal: audience feels unease without knowing why
- [ ] **TEST:** Listen on monitors without sub -- you should NOT hear the sub bass. Turn on the sub -- you should feel it in your body
- [ ] **VERIFY:** Sub does not clip or distort -- at 35 Hz even small overs can damage speakers. Confirm clean on a meter

#### Sound Design: Foley Layer

- [ ] Footsteps
- [ ] Fabric rustling
- [ ] A door closing
- [ ] Level: -18 dB
- [ ] Pan footsteps L -> R slowly across stereo field
  - [ ] Goal: the sound of a person in a quiet room
- [ ] **TEST:** Close your eyes and listen to the foley solo -- can you visualize someone moving through a room? If not, adjust panning speed or add more spatial reverb
- [ ] **VERIFY:** Foley does not have any sudden loud transients that break the intimate atmosphere -- compress or manually ride any spikes

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Lo-fi drums | -4 dB | 200 Hz - 6 kHz (reduced BW) | Center |
| Piano (degraded) | -3 dB | 500 Hz - 3 kHz | Slight left (30%) |
| Sub rumble | -14 dB | 30 - 50 Hz | Mono |
| Foley | -18 dB | 1 - 8 kHz | Moving L/R |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -10 to -9 LUFS -- this should be the QUIETEST track in the set
- [ ] **TEST:** This track at venue volume should feel uncomfortably quiet compared to Track 5 -- that discomfort is the point. Resist the urge to make it louder.

#### Transition Out

- [ ] No transition -- Track 7 starts with a full bar of silence
  - [ ] Then halftime bass drops in
  - [ ] The pause IS the transition
- [ ] **VERIFY:** The silence between Track 6 and Track 7 is TRUE silence -- no reverb tails, no noise floor, no hiss. Absolute zero.
- [ ] **TEST:** Time the silence -- it should be exactly 1 bar at 174 BPM (approximately 1.4 seconds)

---

## Act III: Rupture

*Darkness deepens, then detonates. Halftime menace -> full-tempo shockwave -> neurofunk climax.*

---

### Track 7: Uneven Ground -- Halftime DnB, 87 BPM Feel

**Concept:** *Stays low but darker, heavier. The ground lurches underfoot.*

#### Sound Design: Sub Bass (Star Element)

- [ ] Program sub pattern with pitch bends:
  - [ ] Drop root by a semitone on beat 3
  - [ ] Slide back up by beat 1
  - [ ] MPC pitch envelope: attack 0, decay 400 ms, sustain at destination
    - [ ] The lurch IS the track identity
- [ ] Parallel distortion for harmonics:
  - [ ] Clean signal stays
  - [ ] Distorted copy at -10 dB
  - [ ] HPF at 200 Hz on distorted copy only
    - [ ] Goal: harmonics audible on small speakers
- [ ] **TEST:** Play the sub on a phone speaker -- you should hear the distortion harmonics even though the fundamental is inaudible on a phone
- [ ] **VERIFY:** The pitch bend lands on the semitone accurately -- use a tuner to confirm the lowest pitch is exactly Db
- [ ] **TEST:** The lurch should feel physical and unsettling -- if it feels musical/pleasant, increase the pitch bend range to a whole tone

#### Sound Design: Drums

- [ ] Halftime continues
- [ ] Add industrial percussion layers:
  - [ ] Anvil hits
  - [ ] Sheet metal
  - [ ] Processed hammer impacts
  - [ ] Alt: synthesize with short FM tones (carrier 80 Hz, mod 400 Hz)
- [ ] Quantize hard -- rigidity contrasts with lurching bass
- [ ] **TEST:** Solo drums and bass together -- the rigid drums against the lurching bass should create tension. If they feel like they agree, the contrast is insufficient.
- [ ] **VERIFY:** Industrial percussion samples have no unwanted resonant frequencies -- sweep a narrow EQ boost across each sample to find and cut any ringing

#### Sound Design: Atmosphere

- [ ] Dark drone: two oscillators a tritone apart (D and Ab)
  - [ ] Heavy reverb: 4s decay, 80% wet, 100% diffusion
  - [ ] Creates subconscious harmonic tension
- [ ] Level: -10 dB, wide stereo
- [ ] **VERIFY:** The tritone interval is correct -- play D and Ab together on a keyboard first to confirm the dissonant quality
- [ ] **TEST:** Mute the drone during playback -- the track should lose its menacing quality

#### Sound Design: Risers/FX

- [ ] Reverse cymbal crashes pitched down 1 octave
- [ ] Use as transition markers every 16 bars
- [ ] **VERIFY:** Reverse cymbals peak exactly on beat 1 of every 16th bar -- scrub to 3 different markers and confirm

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Lurching sub | -2 dB | 30 - 120 Hz | Mono |
| Sub harmonics (par) | -10 dB | 200 Hz - 2 kHz | Mono |
| Industrial perc | -5 dB | 500 Hz - 8 kHz | Center + hard pans |
| Tritone drone | -10 dB | 100 Hz - 2 kHz | Wide (90%) |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -9 to -8 LUFS -- slightly louder than Track 6 but still restrained
- [ ] **TEST:** This track should feel heavier than Track 6 despite similar volume -- the heaviness comes from the sub and drone, not loudness

#### Transition Out

- [ ] Sub holds lowest pitch (Db)
  - [ ] Filtered noise sweep builds over 8 bars
- [ ] Last beat: everything cuts
  - [ ] Half second of dead silence
  - [ ] Track 8 explodes at full tempo
- [ ] **VERIFY:** The silence gap is exactly a half second -- too long kills momentum, too short does not let the silence register
- [ ] **TEST:** This is the most critical transition in the set. Rehearse it 5 times minimum.
- [ ] **VERIFY:** Noise sweep does not clip the master at its peak

---

### Track 8: Ash Garden -- Dark DnB, 174 BPM

**Concept:** *Tempo doubles back. Biggest energy shift in the set. Scorched earth.*

#### Sound Design: Impact of Tempo Return

- [ ] Silence before beat 1 is critical -- do not fill it
- [ ] First hit = ALL of these simultaneously on beat 1:
  - [ ] Kick
  - [ ] Snare
  - [ ] Distorted bass stab
  - [ ] White noise burst
- [ ] Peak at -2 dBTP -- loudest single transient in the entire set
  - [ ] Audience physically reacts
- [ ] **VERIFY:** Meter the first hit -- confirm true peak is between -3 and -1 dBTP
- [ ] **TEST:** Play the Track 7 -> 8 transition at full monitoring volume. Did you flinch? Good.

#### Sound Design: Bass ('Scorched')

- [ ] Neuro-style resampled bass -- multi-pass process:
  - [ ] Pass 1: Program bass phrase in MPC
  - [ ] Pass 2: Bounce to audio, reload as sample
  - [ ] Pass 3: Pitch-shift, reverse sections, add distortion
  - [ ] Pass 4: Re-chop, repeat passes 2-3 again
    - [ ] Each pass adds harmonic complexity and grit
    - [ ] Result: a bass that sounds like it has been through fire
- [ ] LPF automation: 400 Hz - 4 kHz in 1-bar cycles
- [ ] **TEST:** A/B the original bass phrase (Pass 1) against the final resampled version -- the difference should be dramatic
- [ ] **VERIFY:** Despite heavy processing, the bass still has a clear fundamental pitch -- if it has become pure noise, reduce distortion on the final pass
- [ ] **TEST:** Play the bass with the breaks -- confirm the LPF automation syncs to the bar grid

#### Sound Design: Breaks

- [ ] Layer two breaks:
  - [ ] Clean funk break (Think) -- full frequency, for groove
  - [ ] Distorted Amen (tube sat, drive 80%) at -6 dB -- for aggression
- [ ] Parallel compression on layered result:
  - [ ] Ratio: 10:1
  - [ ] Attack: 0.1 ms
  - [ ] Release: 50 ms
  - [ ] Blend: 40%
- [ ] **TEST:** Solo the clean break, then add the distorted layer -- aggression should increase without changing the groove
- [ ] **VERIFY:** Parallel compression is not squashing dynamics -- bypass and confirm the compressed version is louder but not flatter
- [ ] **TEST:** Check for phase issues between the two break layers -- collapse to mono and listen for thinning

#### Sound Design: Distortion Textures

- [ ] White noise through resonant bandpass filter
  - [ ] Automate sweep: 500 Hz - 6 kHz in 8-bar arcs
- [ ] Level: -12 dB
  - [ ] This is the 'ash' -- it coats everything
- [ ] **TEST:** Mute the noise texture -- the mix should feel cleaner but also emptier, less dangerous
- [ ] **VERIFY:** Bandpass resonance does not create painful frequency spikes -- listen on headphones and sweep manually first

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Layered breaks | 0 dB (ref) | Full spectrum | Center |
| Neuro bass | -1 dB | 40 Hz - 4 kHz | Mono <200, mvmt above |
| Noise texture | -12 dB | 500 Hz - 6 kHz (sweep) | Wide |
| Impact hits | -2 dBTP | Full spectrum | Center |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -7 to -6 LUFS
- [ ] **TEST:** Compare Track 8 loudness to Track 4 -- they should be comparable, Track 8 can be slightly louder

#### Transition Out

- [ ] Breaks drop out elements in order:
  - [ ] Hi-hats removed (2 bars)
  - [ ] Kick removed (2 bars)
  - [ ] Only snare + bass remain
- [ ] Snare rolls accelerate into 32nd-note fill
  - [ ] Fill slams into Track 9 beat 1
- [ ] **TEST:** Each element removal should be noticeable -- if it is not, that element was too quiet
- [ ] **VERIFY:** 32nd-note snare fill timing is metronomically tight -- listen at half speed to confirm

---

### Track 9: Kintsugi Bass -- Neurofunk, 176 BPM

**Concept:** *Peak intensity. Bass breaks apart and rebuilds mid-phrase. Gold in the cracks.*

#### Sound Design: The 'Kintsugi' Bass Technique

- [ ] Program 8-bar bass phrase
- [ ] At bar 5: introduce deliberate 'break'
  - [ ] Bass cuts to silence for an 8th note
  - [ ] New bass timbre fills the gap:
    - [ ] Different waveform
    - [ ] Heavier distortion
    - [ ] +2 dB louder than original
  - [ ] The repair is louder and more present than the original
- [ ] Repeat with variations: different break points, different repair timbres
  - [ ] Each break-and-repair = another golden seam
- [ ] **TEST:** Solo the bass -- does the repair timbre feel like a deliberate upgrade, or just a different sound? It must feel BETTER than what it replaced.
- [ ] **VERIFY:** The silence gap is exactly one 8th note -- too long breaks the groove, too short is inaudible
- [ ] **TEST:** Play the 8-bar phrase 4 times in a row -- each break-repair should occur at a different point
- [ ] **VERIFY:** Repair sections are measurably +2 dB louder -- meter both original and repair sections to confirm

#### Sound Design: MPC Execution

- [ ] Audio track with manual chop points
  - [ ] Bass phrase as one audio region
  - [ ] Slice at break points
  - [ ] Alternate bass samples on second audio track fill gaps
    - [ ] Gives precise control over break-repair timing
- [ ] **VERIFY:** No clicks or pops at chop boundaries -- zoom in on each slice point and add 1-2 ms crossfades if needed
- [ ] **TEST:** Play the two audio tracks solo'd together -- confirm timing alignment is sample-accurate at splice points

#### Sound Design: Drums

- [ ] Tight, machine-like, programmed
- [ ] Kick: four-to-the-floor at 176 BPM
  - [ ] Relentless feel in DnB context
- [ ] Snare on 2 and 4
  - [ ] Layered click transient: +3 kHz shelf on separate click layer
- [ ] Hi-hats: 16th notes, alternating open/closed
  - [ ] Velocity: closed = 60, open = 90
- [ ] **TEST:** Solo drums -- at 176 BPM four-to-the-floor the kick should feel almost techno-like in its relentlessness
- [ ] **VERIFY:** Click transient layer is aligned to snare hits within 1 ms -- zoom in on the waveform to confirm
- [ ] **TEST:** Hi-hat velocity alternation should create a subtle swinging feel -- if flat, increase the velocity difference (closed=50, open=100)

#### Sound Design: Modulation

- [ ] Automate everything in 2-bar cycles:
  - [ ] Filter cutoff on bass
  - [ ] Reverb send on snare
  - [ ] Pan position on hi-hats: 20% L to 20% R
- [ ] Constant motion prevents ear fatigue at this intensity
- [ ] **VERIFY:** All three automations are running simultaneously in different phase relationships -- stagger start points by half a bar each
- [ ] **TEST:** Listen to 60 seconds of Track 9 -- does it feel fatiguing? If yes, reduce one automation range

#### Mix Targets

| Element | Level | Frequency Focus | Pan |
|---------|-------|-----------------|-----|
| Bass (original) | -2 dB | 40 Hz - 3 kHz | Mono |
| Bass (repair) | 0 dB (louder) | 40 Hz - 5 kHz | Mono |
| Kicks | -1 dB | 40-200 Hz + 3-5 kHz click | Center |
| Snare + click | -3 dB | 200 Hz + 3-8 kHz | Center |
| Hi-hats | -8 dB | 6 - 14 kHz | Narrow sweep |

- [ ] **VERIFY:** Levels match table within +/- 1 dB
- [ ] **VERIFY:** Full mix reads -6 to -5 LUFS -- this is the LOUDEST track in the set
- [ ] **TEST:** Compare to Track 8 -- Track 9 should feel like another gear has been engaged
- [ ] **VERIFY:** True peak does not exceed -1 dBTP at any point

#### Performance

- [ ] Go hardest on Q-Links during this track
  - [ ] Sweep bass filter in real-time
  - [ ] Open delay feedback for half a bar, then cut
- [ ] XYFX is your instrument -- track is canvas, hands are brush
- [ ] **TEST:** Rehearse 3 specific XYFX gestures and lock them in through repetition

#### Transition Out

- [ ] Bass does one final break
  - [ ] Does NOT repair -- silence stretches for a full beat
  - [ ] Track 10 enters with a degraded signal, not a bang
- [ ] **TEST:** The unrepaired break should feel WRONG -- like something is missing. That absence is the emotional hook into Track 10.
- [ ] **VERIFY:** The silence is exactly one beat at 176 BPM (approximately 340 ms)

---

## Act IV: Acceptance

*The final statement. Commanding techstep surrenders to entropy. The circle closes.*

---

### Track 10: The Imperfect Signal -- Techstep DnB, 174 BPM

**Concept:** *Perfection was never the point. The signal degrades. The set ends in static and silence.*

#### Sound Design: Corrupted Transmission Layer

- [ ] Record spoken-word phrase (own voice or sampled)
  - [ ] Content: single sentence about impermanence
- [ ] Process through increasing degradation:

| Timestamp | Processing | Result |
|-----------|-----------|--------|
| 0:00 - 1:00 | Clean vocal + short reverb | Intelligible, present |
| 1:00 - 2:00 | Bitcrusher: 16-bit -> 12-bit | Subtle grit, still clear |
| 2:00 - 3:00 | SR: 44.1k -> 22k -> 11k | Aliasing, losing fidelity |
| 3:00 - 4:00 | Ring mod at 60 Hz added | Robotic, words blur |
| 4:00 - end | Full noise dissolution | Words gone, only texture |

- [ ] **TEST:** Play the vocal from 0:00 to end without the rest of the mix -- the degradation should feel like watching a photograph dissolve in water
- [ ] **VERIFY:** At 1:00 words are 100% intelligible. At 2:00 about 80%. At 3:00 about 40%. At 4:00 zero percent. Adjust timestamp boundaries if the curve is too fast or slow.
- [ ] **TEST:** Ask someone else to listen and write down what they hear at the 3:00 mark -- they should catch fragments but not full sentences

#### Sound Design: MPC Implementation

- [ ] Option A: Insert FX parameter locks per step
- [ ] Option B: Bounce progressive degradation versions
  - [ ] Crossfade between them on separate audio tracks
- [ ] **VERIFY:** Whichever method chosen, transitions between degradation stages are smooth -- no audible jumps between processing stages

#### Sound Design: Breaks

- [ ] Start full and commanding -- classic techstep two-step
- [ ] Over final 2 minutes, remove elements one at a time:
  - [ ] First: ghost notes removed
  - [ ] Then: hi-hats removed
  - [ ] Then: kick removed
  - [ ] Only snare remains
  - [ ] Snare reverb: automate decay 0.5s -> 4s over 2 minutes
- [ ] **TEST:** Listen to the last 2 minutes -- each element removal should be noticeable
- [ ] **VERIFY:** The snare reverb at 4s decay does not create a washy mess -- the tail should be a distinct echo fading into space
- [ ] **TEST:** After the kick is removed, does the track feel weightless? It should. That signals the end.

#### Sound Design: Bass

- [ ] Techstep growl -- FM synthesis
  - [ ] Slow modulator drift
- [ ] Reduce presence by 1 dB every 16 bars
  - [ ] By the end: barely audible
    - [ ] Sub memory carried only by room resonance
- [ ] **VERIFY:** Count the 16-bar sections and confirm the correct number of 1 dB drops to reach -16 dB by end
- [ ] **TEST:** At the final 30 seconds, mute the bass -- if you cannot tell the difference, the fade-out is working correctly

#### Sound Design: Final 30 Seconds

- [ ] Only degraded vocal-noise remains
- [ ] Fading reverb tail from last snare hit
- [ ] Sub fading below hearing threshold
- [ ] End on tape hiss -- same texture that opened Track 1
  - [ ] The snake eats its tail
  - [ ] DO NOT CUT EARLY -- let it reach true silence
- [ ] **TEST:** A/B the tape hiss from Track 10 ending with the tape hiss from Track 1 opening -- they should be the same sample or sonically identical
- [ ] **VERIFY:** The final audio output reaches true digital silence (all zeros) before the sequence ends -- zoom in on the waveform tail
- [ ] **TEST:** Play the last 60 seconds at full venue volume -- does the silence at the end feel like an ending or an awkward pause? It should feel final.
- [ ] **VERIFY:** No click, pop, or digital artifact at the very end of the last sample

#### Mix Targets (Opening -> Final 30 Seconds)

| Element | Opening | Final | Notes |
|---------|---------|-------|-------|
| Breaks | 0 dB | Removed | Peel away element by element |
| Bass | -2 dB | -16 dB | 1 dB reduction per 16 bars |
| Vocal/transmission | -8 dB | -6 dB | Relatively louder as mix thins |
| Reverb tails | -12 dB | -4 dB | Space becomes the music |
| Tape hiss | Silent | -12 dB | Callback to Track 1 |

- [ ] **VERIFY:** Opening levels match table within +/- 1 dB
- [ ] **VERIFY:** Track 10 opening reads -7 to -6 LUFS, final 30 seconds reads below -20 LUFS
- [ ] **TEST:** Play Track 9 ending into Track 10 opening -- energy should feel commanding but the degraded signal entry should signal that something has changed

---

## Arc Summary

| Act | Tracks | Arc | Energy |
|-----|--------|-----|--------|
| I: Awakening | 1-3 | Soft, granular, intimate, field-recorded | Low -> Med |
| II: Descent | 4-6 | Emotional peak, jungle, halftime restraint | High -> Low |
| III: Rupture | 7-9 | Dark rebuild -> neurofunk climax | Low -> Peak |
| IV: Acceptance | 10 | Commanding withdrawal, signal death | High -> Silence |

| Trk 1 | Trk 2 | Trk 3 | Trk 4 | Trk 5 | Trk 6 | Trk 7 | Trk 8 | Trk 9 | Trk 10 |
|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|
| LOW | MED | MED+ | HIGH | HIGH | LOW | LOW | HIGH | PEAK | FADE |

**The wabi-sabi philosophy lived as a rhythm journey:** *nothing is perfect (the cracks are the point), nothing is finished (the signal degrades), nothing is permanent (the set ends in the same dust it began with).*

### Full-Set Verification

- [ ] **TEST:** Play the entire set front-to-back without stopping (55-65 min) -- confirm every transition works and no sequence fails to advance
- [ ] **VERIFY:** LUFS readings across the set follow the energy curve: Track 1 (~-8), Tracks 2-3 (~-7), Track 4 (~-6), Track 5 (~-7), Track 6 (~-10), Track 7 (~-9), Track 8 (~-6), Track 9 (~-5), Track 10 (~-7 opening, fading to silence)
- [ ] **TEST:** Monitor MPC CPU usage throughout the full playback -- confirm no sequence causes dropouts or overloads
- [ ] **TEST:** Record the full set as a stereo WAV from MPC outputs -- listen back the next day with fresh ears for any issues you missed
- [ ] **VERIFY:** The recorded WAV matches what you heard live from the MPC -- no missing elements or level differences
- [ ] **TEST:** Play the recorded WAV on 3 different systems (headphones, monitors, car/bluetooth speaker) -- confirm the mix translates

---

## Performance Checklist

### Pre-Show (Home / Studio)

- [ ] Load all 10 sequences in Song mode
  - [ ] Verify sequence order: 1 through 10
  - [ ] All sequences: single play, no loop
- [ ] Verify Q-Link assignments (all 5 knobs)
  - [ ] Sweep each 0-100%, confirm range
- [ ] Test XYFX pad routing
  - [ ] X = filter, Y = reverb confirmed
- [ ] Run through all 10 transitions with headphones
- [ ] Set master output to -6 dB
- [ ] Export backup: MPC project file to USB
  - [ ] Export backup: individual stems (WAV 24-bit/48 kHz) to USB
  - [ ] Verify backup laptop can play stems through DJ mixer
  - [ ] **TEST:** Actually play 30 seconds of stems from the backup laptop -- confirm levels match MPC output
- [ ] Pack gear:
  - [ ] DI boxes (Radial ProD2 stereo or equivalent)
  - [ ] TRS cables (2x main + 1 spare)
  - [ ] USB stick with backups
  - [ ] Headphones
  - [ ] Power supply + surge protector
- [ ] **VERIFY:** Every item in the gear list is physically in the bag -- do a final count before leaving
- [ ] **TEST:** Power cycle the MPC, reload the project from scratch, and play the first transition -- confirm the project loads cleanly from a cold start

### Venue / Soundcheck

- [ ] Request booth monitor feed WITH sub
  - [ ] Verify sub present: play Track 6 or 7
  - [ ] **TEST:** Can you FEEL the sub rumble in Track 6? If not, request more sub in the booth monitor mix
- [ ] Cable run: MPC outs (TRS) -> DI boxes -> venue snake
  - [ ] Confirm DIs are full-range (not transformer-colored)
  - [ ] **TEST:** Play a full-range test tone or Track 9 through the DIs -- confirm no high-frequency rolloff compared to headphone output
- [ ] Line check with FOH engineer
  - [ ] Play Track 1 (quietest) for 30 sec
  - [ ] Play Track 9 (loudest) for 30 sec
  - [ ] Confirm no clipping at FOH during Track 9
  - [ ] **VERIFY:** Ask FOH engineer to confirm their input meters are clean on both quiet and loud material
- [ ] Verify MPC power is on clean circuit (no shared lighting)
  - [ ] **TEST:** Listen on headphones while someone flicks the venue lights on and off -- confirm no buzzing or interference in MPC output
- [ ] Test sequence advance: trigger Track 2 from Track 1 tail
- [ ] Set booth monitor volume, mark the knob position
  - [ ] **VERIFY:** Take a phone photo of the monitor knob position -- you can reset it if someone moves it before your set

### During Performance

- [ ] Song mode armed before starting
- [ ] Track 1: begin with XYFX at neutral center
- [ ] Monitor 8-bar transition windows on each track
- [ ] Track 5 -> 6: reduce physical movement for halftime
- [ ] Track 7 -> 8: verify silence gap is clean before tempo return
- [ ] Track 9: use XYFX aggressively for live expression
- [ ] Track 10 ending: let tape hiss fade to TRUE silence
  - [ ] Do not cut early
- [ ] **VERIFY:** After the final silence, wait 3 full seconds before stepping away from the MPC -- this signals to the audience that the set is intentionally over

### Set Timing

| Parameter | Target |
|-----------|--------|
| Total set length | 55 - 65 minutes |
| Average track length | 5.5 - 6.5 minutes |
| Transition duration | 30 - 60 seconds |
| Longest track (5 or 10) | 6 - 7 minutes |
| Shortest track (6) | 4.5 - 5 minutes |

- [ ] **VERIFY:** Time a full rehearsal run -- confirm total duration falls within 55-65 minutes
- [ ] **TEST:** If the set runs long, identify which tracks can be shortened by 30 seconds without losing their arc
- [ ] **TEST:** If the set runs short, identify which tracks benefit from an extra 8-bar loop
