# Timer (for OBS)

A simple and customizable timer that I use as an OBS browser source, Creative Commons licensed.

## How to Use

If you want to use my online version, use this link: `addiment.github.io/timer?h=HOURS&m=MINUTES&s=SECONDS`

The duration of the timer is set

Partially because I'm lazy, and partially because it makes things more convenient,
you can mix and match time formats in odd ways, like `m=90`, `s=200`, or `h=0.5`.
The order doesn't matter, but only the first of a given parameter will be recognized (at least, in my testing).

## Customization

When overriding most of these properties, you should probably use `!important`.

- The font size and weight are declared on the `body`. Use a monospace font for best results.
- `#clock` is a fairly basic div container. If you don't like the background, edit `#clock`'s properties
- `#clock` is a fairly basic div container. If you don't like the background, edit `#clock`'s properties
- `.separator::before` is how the colons are rendered. You can change the separator using the `content` and `color` properties.
- `#seconds-frac` is the fractional part of the seconds. 
- The `#clock` gets the `.elapsed` class when time is up.
- The `#timer` element has an animation when `#clock` has `.elapsed`, you can replace it with the `animation` property.

## Future features

- pausing/resuming
- sound effect (by URL)
- video/gfx
- switch scene on time up