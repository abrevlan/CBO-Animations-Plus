# CBO Animations+

## Recommended Load Order

- Character Body Overhaul
- Physical Attributes
- **CBO Animations+**

## Notes

- I haven't tested this with `Coetus Anima` yet.

## Issues

- Possible alignment issues when it comes to several blendshapes that come with CBO (will tackle those after I become more familiar with CK3's portrait system)

## Planned Features

- More positions ~~(I have several already done but with the `female_head` issue I don't plan to release them yet)~~
- Breast/butt/stomach volume influenced animations
- Personality influenced animations

## Modder Notes

- All **.asset/.txt** files are formatted with tabs with 4 spaces. Please keep that in mind when viewing **.asset/.txt** files in this mod.

## Animation Journal

### Entity State Quirks

- It seems entity states are `looping = yes` by default even without writing it in.
- `next_state = ""` is entirely ignored if you don't set `looping = no`.
- If a state in `(fe)male_body` has `looping = no`, the `(fe)male_head` needs to have a state with the same name for the animation to even show up.
  - `scripted_animation` blocks break from the same reason, altogether not playing even the body animation.

#### Royal Court

- States with `looping = no` are synchronized while those with `looping = yes` have some kind of randomization in both speed and starting time. After each state loop, the animation speed ramps up and then down repeatedly.
