# No Motion model

This model is just a simple representation
of the current geography.
This model is just used for comparison of results
with a real plate motion model.
For a list of models you can see <http://github.com/js-arias/geomodels>.

## Time frame

The model is valid for the whole Earth history
(i.e. 4500 million years).

## Pixelation

The model is available in two resolutions:
e180 (180 pixels at the equatorial ring),
and e120.
For reference,
Pixel IDs are stored as `pixel-ids-xxx.tab`,
in which `xxx` is used to indicate the resolution.

## File description

All files are prefixed as `nomotion-*`
usually followed by the pixelation resolution
and the kind of file.

### Plate motion model

The plate motion model consist in just listing all pixels
and set them as constant on time in the "two" time stages
(0 and 4500 million years).

The model is stored in the file `nomotion-motion-xxx.tab`
in which `xxx` is the pixel resolution.

### Landscape

Layers at present time are derived
from [NaturalEarth](https://www.naturalearthdata.com/)
and [NaturalEarth III](https://www.shadedrelief.com/natural3/index.html).

The only implemented layers are
land and water.

The model is stored in the file `nomotion-landscape-xxx.tab`,
in which `xxx` is the pixel resolution.

A color key,
which is compatible with color-blindness,
and can be used with `plates timepix map` command
is stored in the file `nomotion-landscape-key.tab`.
