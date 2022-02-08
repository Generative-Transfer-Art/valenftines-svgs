# valenftines-svgs

# Randomness
On `unrequited` hearts:
- each heart has a randomized rotate(x) value, where `-30 < x < 30` This rotation is set on mint and persists.
- all UNREQUITED valentines have a lightpink background: `#FFDBDB` (no randomness here)

On `requited` hearts, randomness is introduced through heart color
- heart color is assigned as a class, one of `.pink` `.blue` `.orange` `.green` `.purple` `.yellow` weighted equally. This includes the two partial hearts that are mostly out of the frame, with no messages.

# Variation
- REQUITED hearts are slightly different than their matches/copies
  - the original NFT gets its rainbow background as specified
  - the new match-of NFT has an inverted gradient: *swap only the hex values* on line 28 and line 30 (so the pattern ABCDA becomes ADCBA)

# Transformation
When `unrequited` upgrades to `requited`:
- on the first two hearts (FROM/TO), the class changes from `whiteheart` to `whiteheartoutline`
- on the rect (line 35), replace `class="lightpink"` with `fill="url(#rainbow)"`
- on message hearts, the `black` class is replaced with one of the color classes (i.e. `pink` or `orange`)
- on message heart text, the class changes from `whitetext` to `pinktext`

