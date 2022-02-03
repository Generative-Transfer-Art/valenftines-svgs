# valenftines-svgs

# Randomness
On `unrequited` hearts:
- each heart has a randomized rotate(x) value, where `-30 < x < 30` This rotation is set on mint and persists.

On `requited` hearts, randomness is introduced through heart color and background animation.
- heart color is assigned as a class, one of `.pink` `.blue` `.orange` `.green` `.purple` `.yellow` weighted equally. This includes the two partial hearts that are mostly out of the frame, with no messages.
- background rainbow animation has two variables, speed and scale
  - Speed
    - slow (80%) duration on lines 39 & 46 is `20s`
    - fast (20%) duration on lines 39 & 46 is `6s`
  - Scale
    - large (80%): `fr` animates from `0%` to `300%` (line 40) and `r` starts at `300%` (line 26) and animates from `300%` to `600%` (line 47)
    - small (20%): `fr` animates from `0%` to `50%` (line 40) and `r` starts at `50%` (line 26) and animates from `50%` to `100%` (line 47)


# Transformation
When `unrequited` upgrades to `requited`:
- on the first two hearts (FROM/TO), the class changes from `whiteheart` to `whiteheartoutline`
- on the rect (line 35), replace `class="lightpink"` with `fill="url(#rainbow)"`
- on message hearts, the `black` class is replaced with one of the color classes (i.e. `pink` or `orange`)
- on message heart text, the class changes from `whitetext` to `pinktext`
