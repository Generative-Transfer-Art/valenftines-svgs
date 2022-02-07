# valenftines-svgs

# Randomness
On `unrequited` hearts:
- each heart has a randomized rotate(x) value, where `-30 < x < 30` This rotation is set on mint and persists.
- the `.background` class is a randomly assigned color
  - 50% light pink: `#FFDBDB`
  - 20% blue: `#A2E2FF`
  - 10% purple: `#E8D1FF`
  - 10% yellow: `#FFF6AE`
  - 5% orange: `#FFD7AF`
  - 5% green: `#C8FFDF`

On `requited` hearts, randomness is introduced through heart color
- heart color is assigned as a class, one of `.pink` `.blue` `.orange` `.green` `.purple` `.yellow` weighted equally. This includes the two partial hearts that are mostly out of the frame, with no messages.

# Variation
- REQUITED hearts are slightly different than their matches/copies
  - the original NFT gets its rainbow background as specified
  - the new match-of NFT has an inverted gradient: *swap only the hex values* on line 28 and line 30

# Transformation
When `unrequited` upgrades to `requited`:
- on the first two hearts (FROM/TO), the class changes from `whiteheart` to `whiteheartoutline`
- on the rect (line 35), replace `class="lightpink"` with `fill="url(#rainbow)"`
- on message hearts, the `black` class is replaced with one of the color classes (i.e. `pink` or `orange`)
- on message heart text, the class changes from `whitetext` to `pinktext`

