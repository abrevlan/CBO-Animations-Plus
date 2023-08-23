# CBO Animations+

## Recommended Load Order

- Character Body Overhaul
- Physical Attributes
- **CBO Animations+**

## Notes

- I haven't tested this with `Coetus Anima` yet.

## Issues

- The `female_head` animations don't show and is replaced with the default `idle` animation instead.
  - They show up if you remove the `looping = no next_state = ""` attributes but they are not synced with the body animation.
  - If you also remove the same attributes with the `female_body`, the female's animation is now out of sync with the male's.
  - If you also try to remove the same attributes in the male equivalent assets both will become out of sync entirely.
- Possibly alignment issues when it comes to several blendshapes that come with CBO (will tackle those after I become more familiar with CK3's portrait system)

## Planned Features

- More positions (I have several already done but with the `female_head` issue I don't plan to release them yet)
- Breast/butt/stomach volume influenced animations
- Personality influenced animations

## Modder Notes

- All **.asset/.txt** files are formatted with tabs with 4 spaces. Please keep that in mind when viewing **.asset/.txt** files in this mod.
